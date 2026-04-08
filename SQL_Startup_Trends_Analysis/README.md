# WORK IN PROGRESS #

# SQL Startup Trends Analysis

## Project Overview
This project explores startup ecosystem trends using SQL across multiple business domains including funding, acquisitions, investor behavior, employee education, and geographic investment patterns. The goal is to replicate a real BI workflow by transforming raw relational data into insights that support executive decision‑making for venture capital, marketing, and strategy teams.

The analysis includes 10 tasks covering data cleaning, aggregation, joins, window functions, conditional logic, and multi‑table relationships.

---

## Dataset & Tables Used
The project uses several relational tables, including:

- **company** — company metadata, category, country, funding totals, status  
- **funding_round** — funding events, amounts, dates  
- **acquisition** — acquisition details, price, terms, dates  
- **people** — employees and influencers  
- **education** — employee degree information  
- **fund** — investor fund activity  
<img width="679" height="487" alt="image" src="https://github.com/user-attachments/assets/492c61d5-92b0-48d6-8ec3-f321596852e1" />


---

## Key Business Questions Answered

### **1. Startup Landscape**
How many companies have closed down?

### **2. Sector Funding Analysis**
How much funding have US‑based news companies historically raised?

### **3. Cash Acquisition Trends**
How much money was spent on cash‑based acquisitions from 2011–2013?

### **4. Influencer Identification**
Which individuals have Twitter handles starting with “Silver”?

### **5. Finance Influencers**
Which influencers have “money” in their handle and last names starting with “K”?

### **6. Geographic Funding Patterns**
Which countries attract the most venture capital?

### **7. Funding Round Volatility**
Which dates show large variation between smallest and largest funding rounds?

### **8. Fund Activity Classification**
Classify funds into high, middle, and low activity based on number of companies invested in.

### **9. Investment Strategy by Activity Level**
Do high‑activity funds participate in more funding rounds per company?

### **10. Employee Education & Startup Failure**
Do failed startups with only one funding round have employees with fewer degrees?

---

## SQL Techniques Demonstrated
- Multi‑table joins  
- Aggregations & grouping  
- Conditional logic with CASE  
- HAVING clause filtering  
- Window functions  
- Subqueries & nested logic  
- Data type casting  
- Pattern matching with LIKE  
- CTE‑style logic

---

## Folder Structure

```SQL_Startup_Trends_Analysis/
├── README.md
├── queries/
│   ├── 01_closed_companies.sql
│   ├── 02_us_news_funding.sql
│   ├── 03_cash_acquisitions_2011_2013.sql
│   ├── 04_silver_twitter_handles.sql
│   ├── 05_money_handles_lastname_k.sql
│   ├── 06_country_funding_totals.sql
│   ├── 07_funding_round_volatility.sql
│   ├── 08_fund_activity_classification.sql
│   ├── 09_avg_rounds_by_activity.sql
│   ├── 10_employee_education_failed_startups.sql
│
├── screenshots/
│   ├── task1_closed_companies.png
│   ├── task6_country_funding.png
│   ├── task7_volatility.png
│   ├── task10_education.png
│
└── outputs/
```
## Sample Output (Screenshots)

Below are example outputs from selected SQL tasks.

### Task 1 — Closed Companies Count
![Closed Companies](./screenshots/task1_closed_companies.png)

### Task 6 — Country Funding Totals
![Country Funding](./screenshots/task6_country_funding.png)

### Task 7 — Funding Round Volatility
![Funding Volatility](./screenshots/task7_volatility.png)

### Task 10 — Employee Education Analysis
![Education Analysis](./screenshots/task10_education.png)


---

## How to Use This Project
1. Open the `queries/` folder  
2. Run each SQL file in order (01 → 10)  
3. Review outputs results to the `outputs/` folder  
4. Use insights to support BI dashboards or reporting  

---

## Next Steps
- Add visualizations in Tableau or Power BI  
- Build a dashboard summarizing funding, acquisitions, and geographic trends  
- Expand analysis with employee‑level segmentation or time‑series forecasting  

---

## Author
**Connor Kaiser**  
Business Intelligence Analyst  
LinkedIn: *your link here*
