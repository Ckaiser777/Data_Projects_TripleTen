# Zomato Restaurant Performance Analysis — Research Plan

## 1. Project Objective
The objective of this project is to evaluate restaurant performance on the Zomato platform using the provided CSV datasets. The analysis focuses on understanding how restaurants differ in revenue generation, order volume, and average order value (AOV), as well as how these performance metrics vary across cuisines, cities, and time.

---

## 2. Research Questions
1. Which restaurants generate the highest total revenue?  
2. Which restaurants receive the highest number of orders?  
3. What is the average order value (AOV) across restaurants?  
4. How does restaurant performance vary by cuisine?  
5. How does restaurant performance vary by city?  
6. How does restaurant revenue change over time?

---

## 3. Hypotheses
1. Higher-rated restaurants generate more revenue.  
2. Certain cuisines consistently outperform others in total revenue.

---

## 4. Data Model and Fields Used

### A. Restaurant → Orders (Primary Analytical Join)
**Join:** `orders.r_id = restaurant.id`

**Fields Used:**
- restaurant.id  
- restaurant.name  
- restaurant.city  
- restaurant.cuisine  
- restaurant.rating  
- orders.sales_amount  
- orders.sales_qty  
- orders.order_date  

---

### B. Restaurant → Menu (Descriptive Only)
**Join:** `restaurant.id = menu.r_id`

**Fields Used:**
- menu.price  

---

### C. Menu → Food (Descriptive Only)
**Join:** `menu.f_id = food.f_id`

**Fields Used:**
- food.item  
- food.veg_or_non_veg  

---

## 5. Data Preparation

### A. Data Cleaning
- Convert `order_date` to a valid date type  
- Ensure `sales_amount` is numeric  
- Standardize city names  
- Normalize cuisine categories  
- Handle missing or non-numeric ratings  

---

### B. Data Transformations
- Use `orders.sales_amount` as the revenue field  
- Aggregate revenue and orders at:  
  - Restaurant level  
  - City level  
  - Cuisine level  
- Create categorical bins for:  
  - Rating tiers  
  - Menu size (optional, descriptive only)

---

### C. Feature Engineering
- Average Order Value (AOV)  
- Revenue by cuisine  
- Revenue by city  
- Time-based fields (day of week, month, year)

---

## 6. Planned Visualizations

### A. Restaurant Performance
- Total Revenue by Restaurant (bar chart)  
- Total Orders by Restaurant (bar chart)  
- Average Order Value (AOV) (bar chart or KPI)

### B. Cuisine and City Performance
- Revenue by Cuisine (bar chart or treemap)  
- Revenue by City (map or bar chart)

### C. Time-Based Performance
- Revenue Over Time (line chart)

### D. Supporting Descriptive Visuals
- Menu price distribution  
- Menu variety by restaurant  
- Vegetarian vs. non-vegetarian item distribution  

---

## 7. Scope and Limitations

### Included
- Restaurant-level revenue and order analysis  
- AOV analysis  
- Cuisine-level and city-level performance analysis  
- Time-series analysis using `order_date`  
- Descriptive menu and food insights  

### Excluded
- Item-level revenue analysis  
- Item-level popularity analysis  
- Customer segmentation  
- Delivery time analysis  
- Hourly or time-of-day analysis  
- Sentiment or review text analysis  

---

## 8. Deliverables
1. **Tableau Dashboard** — Summary of restaurant performance across revenue, orders, AOV, cuisine, city, and time.  
2. **Story Pages** — Supporting descriptive analysis of menu and food data.  
3. **Written Summary** — Key insights and recommendations.  
4. **Research Plan (PDF)** — This document.

