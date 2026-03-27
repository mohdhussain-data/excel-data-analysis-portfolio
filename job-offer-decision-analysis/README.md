# Job Offer Decision Analysis Dashboard (Excel)

## Overview
Decision-support model built in Excel to evaluate and rank multiple job offers using weighted criteria. Converts subjective preferences into a structured, quantitative comparison.

---

## Objective
- Compare multiple job options using consistent criteria  
- Apply priority-based weights  
- Compute weighted scores and rankings  
- Identify best and worst options  
- Support decision-making with clear insights  

---

## Project Structure

### 1. `raw_data` (Input Layer)
- Job roles evaluated on a 1–5 scale across:
  - Salary  
  - Growth  
  - Work-Life Balance  
  - Stability  
  - Skills Alignment  
  - Company Reputation  

---

### 2. `calculations` (Logic Layer)
- Weight assignment per factor  
- Weighted score = Rating × Weight  
- Total score per job  
- Ranking using `RANK`  
- Best/Worst job using `INDEX + MATCH`  

---

### 3. `analysis` (Dashboard Layer)
- KPI Metrics:
  - Best Job  
  - Worst Job  
  - Top Score  
  - Score Gap  
  - Decision Confidence  
- Ranking table  
- Factor contribution breakdown  
- Charts:
  - Job comparison  
  - Key driver analysis  

---

## Key Insights
- Service-based SQL Data Analyst role ranks highest due to strong performance in high-weight factors (Skills, Salary, Growth)  
- MNC Data Analyst role is competitive but weaker in Growth and WLB  
- Startup role ranks lowest due to low Stability and Salary  
- Skills and Salary drive most of the decision weight  
- Narrow score gap indicates close competition  

---

## Recommendations
- Select Service Company role for overall value  
- Choose MNC if Stability is prioritized  
- Consider Startup only if flexibility outweighs risk  
- Re-evaluate if weights (priorities) change  

---

## Tools & Functions
- Microsoft Excel  
- `SUM`, `RANK`, `INDEX`, `MATCH`  
- Absolute and relative referencing  

---

## Outcome
- Built a fully dynamic, formula-driven decision model  
- Demonstrated structured analytical thinking  
- Translated subjective choices into measurable insights