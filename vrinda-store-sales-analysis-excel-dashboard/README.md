# Vrinda Store Sales Analysis Dashboard (Excel)

## 📌 Project Objective
Analyze annual sales data of Vrinda Store to understand customer behavior, identify key revenue drivers, and generate actionable insights to improve business performance in 2023.

---

## ❓ Business Problems Solved
- Compare *sales vs orders* over time
- Identify *highest performing month*
- Analyze *gender-based purchasing behavior*
- Understand *order status distribution*
- Find *top contributing states*
- Analyze *age group vs gender trends*
- Identify *top-performing sales channels*

---

## 📊 Dataset Overview
The dataset contains transactional sales data with the following fields:

- Order ID, Customer ID
- Gender, Age
- Order Date
- Product Category & SKU
- Quantity & Sales Amount
- Order Status (Delivered, Cancelled, Returned, Refunded)
- Sales Channel (Amazon, Flipkart, Myntra, etc.)
- Location (City, State, Pincode)

---

## 🧹 Data Cleaning
- Standardized Gender values (M → Men, W → Women)
- Converted text-based quantities to numeric values
- Verified and cleaned currency/amount columns
- Removed inconsistencies and ensured data integrity

---

## ⚙️ Data Processing (Feature Engineering)
- Created *Age Group column*:
  - Senior (>50)
  - Adult (30–49)
  - Teenager (<30)
- Extracted *Month* from date using:
  ```excel
  =TEXT(Date,"mmm")

---

## 📈 Data Analysis (Pivot Tables)
- Sales vs Orders (Monthly trend with combo chart)
- Sales by Gender (Men vs Women)
- Order Status Distribution
- Top 5 States by Sales
- Age Group vs Gender Analysis (% contribution)
- Sales Contribution by Channel

---

## 📊 Dashboard Features
- Interactive Excel dashboard
- Slicers:
  - Month
  - Channel
  - Category
- Dynamic filtering across all charts using report connections
- Clean and structured visual layout

---

## 🔍 Key Insights
- Women contribute ~65% of total sales
- Maharashtra, Karnataka, and Uttar Pradesh contribute ~35% of revenue
- Adult age group (30–49 years) contributes ~50% of orders
- Amazon, Myntra, and Flipkart contribute ~80% of total sales

---

## 💡 Business Recommendations
- Target women customers (30–49 age group)
- Focus marketing in top-performing states
- Increase ad spend on Amazon, Myntra, Flipkart
- Use offers and discounts to maximize conversions

---

## 🛠 Tools Used
- Microsoft Excel
  - Pivot Tables & Pivot Charts
  - Slicers & Dashboarding
  - IF, TEXT functions
  - Data Cleaning Techniques

---

## 🚀 Skills Demonstrated
- Data Cleaning & Preparation
- Feature Engineering
- Pivot Table Analysis
- Data Visualization
- Dashboard Design
- Business Insight Generation