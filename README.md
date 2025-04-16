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
    - Order Year: Extracted from the Order Date.
    - Order Month: Month component of the Order Date.
    - Order Day of Week: Day name (e.g., Monday, Tuesday) derived from the Order Date.
    - Order YearMonth: Combined year and month in YYYY-MM format for monthly trend analysis.
    - Shipping Time: Calculated as the number of days between Ship Date and Order Date, indicating delivery duration.
- Standardization:
    - Ensured consistent formatting for string fields (e.g., title-cased category names).
    - Verified and enforced numerical data types for columns such as Sales, Quantity, Discount, and Profit.
    - Converted all date-related fields to datetime objects for compatibility with time series functions.

---

## III. Analysis of Each Chart

### 📊 1.Region and State Sales Analysis
![Image](https://github.com/user-attachments/assets/2a83497f-4beb-484a-b590-9da4da1a9cab)

**Comments:**
- The graph compares sales and profit across different regions. The East Region leads with the highest sales, represented by the tall blue bars, though its profit margin is relatively lower, as indicated by the smaller orange bars. The West Region follows closely, showing strong sales and a higher profit margin, with its orange bar being more substantial compared to East. The Central and South Regions perform less well, with Central slightly outperforming South in both sales and profit.
- While the East drives the most revenue, its profit margin isn't as high as the West's, which combines good sales with a better profit margin. The South has the weakest performance, suggesting room for improvement in both sales and profitability, while the Central region sits in the middle.
- In short, the East is the revenue leader, but the West shows stronger profitability. The Central and South regions should be analyzed further to boost their performance, particularly in terms of profit.

![Image](https://github.com/user-attachments/assets/82b234d8-02c3-4896-9870-f039847f4d01)

**Comments:**
- The graph shows the Top 10 states with the highest profit, with California leading the way by a large margin. California's profit far exceeds the others, followed by New York and Washington, which also show substantial profits, though not as high as California's. The states like Michigan, Virginia, and Indiana continue to contribute well, but their profits start to dip compared to the top three.
- At the lower end of the top 10, Delaware generates the least profit, though still showing positive results. The graph clearly highlights California as the dominant contributor to profits, with the other states trailing behind.
- In short, California stands out as the top performer, while other states, particularly Delaware, show relatively lower profits.

---

### 📊 2. Monthly Sales Analysis
![Image](https://github.com/user-attachments/assets/d5efbccd-74c8-40e3-95a1-5e8455368909)

**Comments:**
- This graph shows the total sales by month across multiple years, with sales in dollars on the vertical axis and months on the horizontal axis. The months are represented by shades of blue, with the darker shades indicating higher sales.
- From the graph, we can see that December leads the way with the highest sales, followed by November. These months show a sharp increase in sales compared to the rest of the year, indicating strong seasonal sales, likely due to holidays and promotions.
- The months of March, June, and September also see notable spikes in sales, though they do not reach the levels seen in November and December. Meanwhile, the earlier months of the year, such as January and February, have relatively low sales, with January showing the smallest figures.
- In short, December and November are the peak sales months, while the earlier months show slower.


![Image](https://github.com/user-attachments/assets/a9fb75f7-8c7d-4921-81bd-6e28da741bf1)

**Comments:**
- This heatmap shows monthly sales data from 2014 to 2017, with each cell representing sales for a specific month and year. The color intensity indicates the level of sales, with darker shades representing higher sales.
- From the heatmap, we can observe the following key trends:
    - 2017 stands out with the highest sales, particularly in November and December, where the color is darkest, indicating peak sales.
    - 2016 also shows strong performance, especially in November and December, which are similarly highlighted with high sales.
    - 2014 and 2015 show generally lower sales throughout the year, with 2014 having consistently low numbers in the early months and gradually improving towards the end of the year.
- Key observations include:
    - The months of November and December consistently show high sales across all years, suggesting strong year-end performance, likely due to holiday seasons and promotions.
    - Mid-year months (June, July, August) also see higher sales compared to the earlier months, particularly in 2017.
    - January typically shows lower sales, especially in 2014 and 2015.
- In summary, November and December are the peak sales months each year, while earlier months like January tend to show lower sales. The sales growth is particularly evident in 2017, with much higher numbers compared to previous years."

---

### 📊 3. Sales Analysis by Category
![Image](https://github.com/user-attachments/assets/7747d534-cf9c-4a08-ae86-65cf012c51ae)

**Comments:**
- The pie chart illustrates sales distribution by category. From the chart, we can see that Technology leads with the highest share at 36.4%, followed closely by Furniture, which accounts for 32.3% of total sales. Office Supplies contributes 31.3% to the overall sales.
- This shows that Technology and Furniture are the dominant categories, while Office Supplies has a slightly smaller but still significant share of sales.
- In summary, Technology is the largest revenue generator, followed by Furniture, with Office Supplies making up a similar portion but slightly trailing behind.

---

### 📊 4. Sales Analysis by Sub-Category
![Image](https://github.com/user-attachments/assets/c299731c-90a7-4e1f-8549-9031994cab51)

**Comments:**
- The bar chart illustrates sales by sub-category. From the chart, we can clearly see that Phones lead with the highest sales, followed closely by Chairs and Storage. These three sub-categories dominate the sales, with Phones reaching over $300,000 in sales, while Chairs and Storage are also strong performers.
- Other notable sub-categories include Tables and Binders, which also contribute significantly to sales, though not as much as the top three. On the lower end, we see sub-categories like Art, Envelopes, and Fasteners, which have much smaller sales figures.
- In summary, Phones, Chairs, and Storage are the highest-grossing sub-categories, while the rest of the sub-categories contribute much less to the overall sales.

---

### 📊 5. Monthly Profit Analysis
![Image](https://github.com/user-attachments/assets/13c7524b-a781-48b6-8379-8ec80c861d76)

**Comments:**
- This line graph shows the monthly profit trend from 2014 to 2017. We can see significant fluctuations in profit throughout the years, with sharp spikes and dips.
- Notably, there are periods of very high profits, particularly around the middle of the year, such as in 2015-06 and 2017-08, where profits surpass $10,000. However, there are also several months where profits drop significantly, reaching as low as $0 in certain months.
- In general, the profit pattern is irregular, indicating that factors like seasonality, promotions, or other market conditions might be influencing the performance. The upward trend towards the end of the period suggests improving profitability as the months progress, particularly in 2017.
- In summary, the profit trend shows volatility with occasional spikes and slumps, but there seems to be improvement as time goes on, particularly toward the final years.

---

### 📊 6. Profit Analysis by Category
![Image](https://github.com/user-attachments/assets/f13028b6-cd38-4db2-b469-f2ab986c8814)

**Comments:**
- The pie chart shows the profit distribution by category. From the chart, we can see that Technology contributes the largest share of profits, accounting for 50.8%. Office Supplies follows with 42.8%, making up a significant portion of the overall profit as well. On the other hand, Furniture contributes a much smaller portion, with only 6.4% of the total profit.
- This indicates that Technology is the most profitable category, while Furniture generates the least profit. Office Supplies stands in between, contributing a solid amount to the total profits.
- In summary, Technology is the clear leader in terms of profitability, while Furniture needs further attention to boost its profit generation.

---

### 📊 7. Profit Analysis by Sub-Category
![Image](https://github.com/user-attachments/assets/d1e0f64e-e792-442b-b898-10c4d18e2f12)

**Comments:**
- This bar chart shows the profit by sub-category. From the chart, we can clearly see that Phones generate the highest profit, with over $40,000, followed by Chairs and Storage, which also perform strongly with significant profits, though not as high as Phones.
- The sub-category Copiers stands out with a sharp rise in profit, much higher than other sub-categories, reaching just over $50,000. Tables, Binders, and Machines contribute moderate profits, but they pale in comparison to the leading categories.
- On the lower end of the chart, sub-categories like Paper, Art, Envelopes, and Labels have significantly lower profits, with some even dipping into negative territory, especially Fasteners.
- In summary, Phones and Copiers are the top performers in terms of profit, while other sub-categories, especially in the office supplies and stationery areas, show lower profitability

---

### 📊 8. Sales and Profit Analysis by Customer Segment
![Image](https://github.com/user-attachments/assets/3c24d9f6-ccff-4563-a95e-beb658af7b80)

**Comments:**
- This bar chart presents sales and profit analysis by customer segment. We can see that the Consumer segment leads by a large margin, with sales significantly higher than the profit, indicating a high volume of transactions but relatively lower profit margins.
- The Corporate segment follows with decent sales, but the profit is notably higher compared to the Consumer segment, which suggests a better profit margin on corporate sales. Finally, the Home Office segment has the smallest sales and profit figures, with sales slightly higher than profits, showing a more balanced but smaller-scale performance.
- In summary, Consumer drives the most sales, but Corporate offers higher profitability, while Home Office shows the least performance in both sales and profit

---

### 📊 9. Shipping time vs profit
![Image](https://github.com/user-attachments/assets/ede905bf-49be-46ba-a11c-6dcc77d9ebfa)

**Comments:**
- This bar chart presents sales and profit analysis by customer segment. We can see that the Consumer segment leads by a large margin, with sales significantly higher than the profit, indicating a high volume of transactions but relatively lower profit margins.
- The Corporate segment follows with decent sales, but the profit is notably higher compared to the Consumer segment, which suggests a better profit margin on corporate sales. Finally, the Home Office segment has the smallest sales and profit figures, with sales slightly higher than profits, showing a more balanced but smaller-scale performance.
- In summary, Consumer drives the most sales, but Corporate offers higher profitability, while Home Office shows the least performance in both sales and profit

---

### 📊 10. Sales-to-Profit Ratio Analysis
![Image](https://github.com/user-attachments/assets/21657c7b-e34b-41bc-8064-c940842a6c48)

**Comments:**
- This line graph illustrates the average profit based on delivery time (number of days). We observe a significant fluctuation in profit as the delivery time changes.
- Initially, with 0 and 1 day delivery, the average profit is relatively low at around $25, but it spikes to about $40 on the 2-day delivery. After that, there is a sharp decline back to lower profit levels before gradually increasing again from 4 to 7 days of delivery.
- The highest profit is seen at the 2-day delivery, which suggests that customers might be willing to pay more for faster delivery, but overall, longer delivery times tend to show a steady increase in profit.
- In summary, 2-day delivery seems to offer the highest profit, but longer delivery times gradually improve the average profit as well, indicating a correlation between delivery time and profit margins

---

### 📊 11. Dashboard
![Image](https://github.com/user-attachments/assets/e9c98033-c958-4597-a7c0-5aff511ddcae)

---

## IV. Overall Conclusion

1. Region
- The East region leads in sales but has a relatively low profit margin.
- The West shows both strong sales and high profitability, making it the most efficient region.
- Central and South underperform, with South in particular requiring improvement.

2. State
- California stands out as the top-performing state with significantly higher profit than all others.
- New York and Washington also generate strong profits, though still behind California.
- The remaining top 10 states contribute steadily, but their performance should be reviewed individually.

3. Time Trends
- November and December consistently see peak sales, likely driven by holiday seasons and promotions.
- January records the lowest sales, especially in earlier years (2014–2015).
- 2017 shows clear growth in both sales and profit, indicating improved performance over time.

4. Category/Sub-category
- Technology is the top-performing category in both sales and profit.
- Furniture has high sales but low profit, suggesting a need to adjust pricing or cost structures.
- Office Supplies contributes moderately across the board.
- Phones and Copiers are the most profitable sub-categories.

5. Customer Segment
- The Consumer segment generates the most sales but with low profit margins.
- Corporate segment has better profit efficiency.
- Home Office contributes the least in both sales and profit, requiring a tailored strategy for growth.

6. Shipping Time
- 2-day delivery yields the highest average profit.
- Longer delivery times (4–7 days) also show increasing profitability, possibly linked to larger or bulk orders.

---

## V. Strategic Recommendations
1. Regional Strategy
- Optimize cost structures in the East to improve profit margins.
- Expand efforts in the West, where both sales and profit are strong.
- Reassess the strategy in the South, focusing on distribution channels, product offerings, and customer support.

2. Product Strategy
-Continue strong investment in Technology, especially Phones and Copiers.
- Re-evaluate the Furniture category: consider product improvement, cost reduction, or pricing adjustments.
- Reduce investment in sub-categories with negative profits (e.g., Fasteners, Envelopes) unless they serve a strategic purpose.

3. Seasonal Growth
- Prioritize marketing and promotions during November–December, the peak sales period.
- Boost Q1 sales through new year campaigns, discounts, or product bundles.

4. Customer Segment Strategy
- Maintain the Consumer base to ensure high sales volume, while improving profit margins via fast shipping or upselling.
- Enhance service to Corporate clients with specialized solutions that leverage their higher profitability.

5. Shipping & Logistics
- Optimize the 2-day delivery process to capitalize on its high-profit potential.
- Analyze longer delivery orders with high profit to identify whether they come from bulk or corporate sales → develop targeted incentives.
