# Data Storytelling Report: Analysis of E-commerce Sales Performance

---

### 📅 Data Timeframe: 2014 - 2017  
### 👨‍💼 Source: Dataset Superstore (Global Superstore)

---

## I. Introduction

This report uses data from Global Superstore to analyze the company's sales performance across various dimensions: region, time, product categories, and customer segments. The goal is to help the business identify strengths, weaknesses, and optimize sales operations. The data includes information on sales, profit, product categories, shipping time, regions, and customer segmentation.

---

## II. Data Analysis Process
### 1. Data Loading and Exploration
- Dataset: Sample - Superstore.csv (9,994 rows × 21 columns)
- The dataset contains transactional records including order details, customer information, sales performance, and shipping data.
- No missing values were found in the dataset, indicating it is complete and ready for analysis.
- Data types were reviewed and adjusted where necessary. Specifically:
    - Order Date and Ship Date columns were converted to appropriate datetime formats for temporal analysis.

### 2. Data Cleaning and Feature Engineering
To enhance analytical capabilities, several new features were created:
- Temporal Features:
    - Order Year: Extracted from the Order Date
    - Order Month: Month component of the Order Date
    - Order Day of Week: Day name (e.g., Monday, Tuesday) derived from the Order Date
    - Order YearMonth: Combined year and month in YYYY-MM format for monthly trend analysis
    - Shipping Time: Calculated as the number of days between Ship Date and Order Date, indicating delivery duration
- Standardization:
    - Ensured consistent formatting for string fields (e.g., title-cased category names)
    - Verified and enforced numerical data types for columns such as Sales, Quantity, Discount, and Profit
    - Converted all date-related fields to datetime objects for compatibility with time series functions

---

## III. Analysis of Each Chart

### 📊 1.Region and State Sales Analysis
![Image](https://github.com/user-attachments/assets/260cb69c-6544-4f73-bed9-4ed1eb7baccf)

**Observations:**
- West and East regions generate the highest sales.
- South has decent sales but relatively low profit.
- Central region shows negative profit – indicates inefficiency.

**Recommendations:**
- Calculate profit margin per region to assess efficiency.
- Investigate causes of Central region's losses (e.g., discounts, shipping costs).
- Consider reallocating marketing budget to high-performing regions.

![Image](https://github.com/user-attachments/assets/400e459a-bdf0-4a97-b4c9-e1520dc6edd4)

**Observations:**
- California leads by a large margin in profit.
- High-population states tend to dominate.
- Significant disparity in profitability across states.

**Recommendations:**
- Benchmark top-performing states to identify best practices.
- Analyze low-performing states to adjust strategy or reduce investment.
- Add sales data to compare revenue vs. profit for each state.

---

### 📊 2. Monthly Sales Analysis
![Image](https://github.com/user-attachments/assets/7c825283-c8ca-41d4-bdc6-a9f65b033d16)

**Observations:**
- Sales peak in November and December.
- March and July show the lowest sales.
- Clear seasonality pattern influenced by holidays.

**Recommendations:**
- Prepare targeted campaigns during low-performing months.
- Launch seasonal promotions in Q4 to maximize holiday sales.
- Break down by year to detect long-term trends or outliers.

![Image](https://github.com/user-attachments/assets/24a2fd6d-fd21-4e4f-8cc0-48c4e8e63694)

**Observations:**
- Sales have increased over the years.
- Growth is not uniform across all months.
- 2017 shows a notable boost in monthly sales.

**Recommendations:**
- Add year-over-year growth percentages for deeper analysis.
- Compare heatmaps for profit and sales to check correlation.
- Investigate what happened in 2017 (e.g., new product launches or policies).

---

### 📊 3. Sales Analysis by Category
![Image](https://github.com/user-attachments/assets/7747d534-cf9c-4a08-ae86-65cf012c51ae)

**Observations:**
- Technology accounts for the largest share of sales.
- Office Supplies and Furniture have similar shares.
- Tech products are key drivers of total revenue.

**Recommendations:**
- Analyze profit by category to assess profitability, not just revenue.
- Consider bundling lower-performing categories with top ones.
- Explore customer segmentation within each category.

---

### 📊 4. Sales Analysis by Sub-Category
![Image](https://github.com/user-attachments/assets/ced86ec3-12f8-48fe-aded-78533f577dc2)

**Observations:**
- Phones and Chairs are the top-selling sub-categories.
- Fasteners and Labels have the lowest sales.
- Sales are unevenly distributed among sub-categories.

**Recommendations:**
- Focus inventory and marketing on top sub-categories.
- Evaluate phasing out or optimizing low-demand items.
- Use sub-category trends to plan promotions.

---

### 📊 5. Monthly Profit Analysis
![Image](https://github.com/user-attachments/assets/13c7524b-a781-48b6-8379-8ec80c861d76)

**Observations:**
- Profit peaks in November, aligns with sales trend.
- Some months show high sales but low profit – possible discount impact.
- Profit is more volatile than sales across months.

**Recommendations:**
- Monitor discount strategies in high-sales months to maintain profit.
- Investigate cost structure differences month-to-month.
- Forecast profit using historical patterns for better planning.

---

### 📊 6. Profit Analysis by Category
![Image](https://github.com/user-attachments/assets/f13028b6-cd38-4db2-b469-f2ab986c8814)

**Observations:**
- Technology has the highest profit margin.
- Furniture shows lower profit despite decent sales.
- Office Supplies provide stable but moderate profit.

**Recommendations:**
- Promote tech products more aggressively to drive profit.
- Reassess pricing or cost structure in Furniture category.
- Consider profitability when planning future product expansion.

---

### 📊 7. Profit Analysis by Sub-Category
![Image](https://github.com/user-attachments/assets/09a98262-d267-4000-ab60-cec8486d1b96)

**Observations:**
- Copiers and Phones are most profitable.
- Tables and Bookcases result in losses.
- Not all high-sales sub-categories are profitable.

**Recommendations:**
- Prioritize sub-categories with strong profit margins.
- Reevaluate pricing, sourcing, or positioning of loss-making products.
- Align marketing spend with profitability, not just sales.

---

### 📊 8. Sales and Profit Analysis by Customer Segment
![Image](https://github.com/user-attachments/assets/3c24d9f6-ccff-4563-a95e-beb658af7b80)

**Observations:**
- Consumer segment contributes the most sales.
- Corporate and Home Office segments are smaller but still valuable.
- Profit margins vary slightly across segments.

**Recommendations:**
- Tailor marketing campaigns to each customer segment.
- Analyze CLV (Customer Lifetime Value) by segment.
- Offer loyalty programs to high-value segments.

---

### 📊 9. Shipping time vs profit
![Image](https://github.com/user-attachments/assets/1e573d5a-cb46-4ffb-9438-371ccdbaca05)

**Observations:**
- Longer shipping times correlate with lower profit.
- Same-day and second-day deliveries yield better margins.
- Standard class shipping may incur hidden costs.

**Recommendations:**
- Promote faster delivery options to increase customer satisfaction and profit.
- Analyze fulfillment cost across shipping types.
- Consider partnerships with logistics providers to optimize costs.

---

### 📊 10. Sales-to-Profit Ratio Analysis
![Image](https://github.com/user-attachments/assets/21657c7b-e34b-41bc-8064-c940842a6c48)

**Observations:**
- Some sub-categories have low profit-to-sales ratios.
- Indicates high cost or poor pricing strategy.
- Efficiency varies greatly across categories.

**Recommendations:**
- Identify ideal profit-to-sales ratio benchmarks.
- Redesign pricing or cost structure in inefficient categories.
- Monitor ratio over time to track performance.

---

## IV. Overall Conclusion

The analysis reveals:
- Revenue has grown steadily over the years, especially during the end-of-year period (November–December), clearly indicating the seasonal influence on consumer purchasing behavior.
- Not all product categories with high revenue generate good profit — some items like Binders and Tables are incurring losses, highlighting the need to evaluate both revenue and cost simultaneously.
- Customer segments differ in value and profitability — the Consumer group brings in high revenue, while the Corporate segment yields better profit margins.
- Shipping costs and delivery time directly affect profitability, indicating the need for a logistics strategy aligned with order value.
- Some states and regions show untapped potential, presenting opportunities to expand market reach and reallocate resources effectively.

---

## V. Strategic Recommendations
- Optimize product mix: Eliminate loss-making products and focus on high-profit items.
- Prepare for peak season: Manage inventory and budget effectively for the end-of-year period.
- Expand market presence: Strengthen presence in untapped regions with potential.
- Personalize customer service: Tailor services based on different customer segments.
- Optimize logistics: Adjust shipping strategy and reduce transportation costs.
