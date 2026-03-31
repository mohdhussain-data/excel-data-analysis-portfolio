# Data Science Salary Dashboard (Excel)

## 📌 Project Overview
This project is an interactive Excel dashboard designed to analyze global data science job salaries based on user-selected filters.

The dashboard allows dynamic exploration of salary trends by **job title, country, and employment type**, helping identify compensation patterns and hiring insights in the data science job market.

---

## 🎯 Objective
To build a dynamic and user-driven dashboard that answers:

- What is the median salary for a specific role?
- How do salaries vary across countries?
- Which job roles pay the highest?
- What job platforms contribute the most listings?
- How does employment type impact salary?

---

## 🧾 Dataset
- Source: Data Science Job Salary dataset
- Contains:
  - Job Title
  - Salary (Yearly Avg)
  - Country
  - Employment Type
  - Company Name
  - Job Platform
  - Skills

---

## 🧹 Data Preparation

### 1. Table Creation
- Converted raw dataset into an Excel Table (SalaryData)
- Enables dynamic updates and structured referencing

### 2. Data Cleaning
- Standardized inconsistent values
- Cleaned job_schedule_type column
- Removed mixed values like:
  - "Full-time and Part-time"
  - "Contract, Full-time"

### 3. Helper Columns
- Extracted clean lists using:
  - UNIQUE()
  - FILTER()
  - SEARCH()

- Example:
  ```excel
=UNIQUE(FILTER(SalaryData[job_schedule_type],
 (NOT(ISNUMBER(SEARCH("and",SalaryData[job_schedule_type])))) *
 (NOT(ISNUMBER(SEARCH(",",SalaryData[job_schedule_type]))))
))

---

## 🎛️ Dashboard Features

### 1. Dynamic Filters
- Job Title
- Country
- Employment Type
- Built using:
  - Data Validation Dropdowns
  - Cleaned helper data

### 2. KPI Cards
- Median Salary
- Top Job Platform
- Total Job Count

### 3. Visualizations
- Salary by Job Role
  - Horizontal bar chart
  - Shows highest paying roles

- Global Salary Distribution
  - Filled Map Chart
  - Displays salary spread across countries

- Employment Type Analysis
  - Bar chart comparing:
    - Full-time
    - Part-time
    - Contract
    - Internship

---

## 🧠 Core Logic (Calculation Engine)
- Median Salary Calculation
  ```excel
=IFERROR(
MEDIAN(
IF(
(SalaryData[job_title]=B2)*
(SalaryData[job_country]=C2)*
(SalaryData[job_schedule_type]=D2),
SalaryData[salary_year_avg]
)
),
"No Data Found"
)
- Uses array filtering logic
- Dynamically updates based on user input

---

## 📊 Key Insights
- Senior roles (Data Scientist, ML Engineer) offer highest salaries
- Salary varies significantly across countries (US highest)
- Full-time roles dominate job listings
- Certain platforms (e.g., Indeed) contribute majority listings

---

## 🚀 Skills Demonstrated
- Excel Dashboard Design
- Data Cleaning & Transformation
- Dynamic Formulas (IF, MEDIAN, FILTER, UNIQUE)
- Data Validation & UI Design
- Map Charts & Advanced Visualizations
- Structured Data Modeling

---

## ⚠️ Limitations
- Dataset is static (not real-time)
- Some countries have limited data points
- Salary averages may not reflect current market changes

---

## 🔥 Conclusion
This project demonstrates the ability to build interactive, business-focused dashboards in Excel using real-world datasets.
It replicates how analysts:
- Clean messy data
- Build dynamic filters
- Extract insights
- Present findings visually