# Superstore Returns Root-Cause Analysis

## Project Overview
This analysis examines product return behavior across categories, states, time periods, customer segments, and sub-categories to identify where returns are most concentrated and what factors may be driving them. Return rate was selected as the primary metric because it normalizes return volume relative to total orders, revealing patterns that raw return counts obscure. A dashboard and Story were developed to help stakeholders explore these patterns interactively and drill down into specific drivers.

---

## Methodology
- **Return Flag:** Created a `Returned Flag` field (1 for returned orders, 0 otherwise).
- **Return Rate Metric:** Calculated return rate as `AVG(Returned Flag)` across different dimensions.
- **Data Preparation:** Joined Orders and Returns tables and built reusable measures for return analysis.
- **Visualization:** Developed views for category, state, customer, time, and sub-category profitability.
- **Storytelling:** Combined all sheets into a Tableau Story that walks stakeholders through the return problem step-by-step.

---

## Project Structure
- **Data Preparation:** Joined tables, created the Returned Flag, and defined return-rate calculations.
- **Exploratory Analysis:** Reviewed return patterns by category, sub-category, state, customer, and time.
- **Low-Fidelity Mockups:** Sketched layout options to determine the most effective narrative flow.
- **Dashboard Development:** Built visuals including:
  - Sales vs Returns
  - Return Rate by Customer
  - Return Rate by State and State Comparison
  - Return Rate by Category
  - Return Rate Over Time by Category
  - Sales vs Profit by Sub-Category
  - Return Rate by Region + Sales
- **Interactivity:** Added filters and drill-downs to support flexible exploration.
- **Story:** Combined all sheets into a structured narrative for executive readability.

---

## Key Insights
- Return rate is the most reliable metric for comparing performance across states, customers, and product groups.
- Technology shows the highest category-level return rate, but sub-category analysis reveals the true drivers.
- Return issues are concentrated in a small group of sub-categories, including Machines, Fasteners, Chairs, Appliances, Phones, and Copiers.
- Several western states show elevated return behavior, with Utah emerging as the highest-return state.
- A small group of customers contributes disproportionately to total returns, indicating behavioral or expectation-driven factors.
- Seasonal patterns show a clear early-fall spike in return rates across multiple categories.
- Some high-sales sub-categories generate weak or negative profit once returns are factored in, highlighting pricing or cost-structure issues.

---

## Tools Used
Tableau (Story, interactive dashboard, return-rate modeling)

---

## View This Project
[Link to Tableau Public Story goes here]
