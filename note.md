# Supermarket Sales EDA — Methodology and Key Findings

## 1. Methodology

This exploratory data analysis was performed on a supermarket sales dataset containing **1,000 transactions and 17 columns**.

The analysis followed these main steps:

1. Loaded the dataset using Pandas.
2. Inspected the dataset structure and data types.
3. Checked data quality by identifying missing values and duplicate records.
4. Converted the `Date` column to datetime format.
5. Extracted `Hour` from the `Time` column and `Month` from the `Date` column.
6. Used `groupby()` and aggregation functions to calculate total sales and order counts by Branch, Product line, Customer type, and Gender.
7. Calculated average order value for branches, product lines, and gender groups.
8. Analyzed hourly sales to identify the busiest hour overall and separately for each branch.
9. Analyzed monthly sales to identify sales patterns over time.
10. Created a bar chart, pie chart, and line chart for the required visualizations.
11. Performed additional analysis using gross margin percentage, a Branch × Product line heatmap, and customer ratings.

## 2. Data Quality

The dataset contains **1,000 rows and 17 columns**.

There are **no missing values** and **no duplicate records**.

The `Date` and `Time` columns were originally stored as text/object data. The `Date` column was converted to datetime format, while the hour was extracted from `Time` for time-based analysis.

## 3. Key Findings

### Branch Performance

- **Branch C** generated the highest total sales at approximately **USD 110.57K**.
- **Branch A** had the highest number of orders with **340 transactions**.
- Branch C had the highest average order value at approximately **USD 337.10**.
- Branch A and Branch B had very similar total sales, both around **USD 106.20K**.

Although Branch A had more orders than Branch C, Branch C generated more total sales because its average order value was higher.

### Product Line Performance

- **Food and beverages** was the highest-revenue product line, generating approximately **USD 56.14K**.
- **Health and beauty** generated the lowest total sales at approximately **USD 49.19K**.
- **Home and lifestyle** had the highest average order value at approximately **USD 336.64**.
- **Fashion accessories** had the highest number of orders among the product lines with **178 transactions**.

### Customer Type

- Member customers accounted for **501 transactions**, while Normal customers accounted for **499 transactions**.
- Members generated approximately **USD 164.22K** in sales.
- Normal customers generated approximately **USD 158.74K** in sales.
- The two customer groups are almost evenly distributed, with Members generating slightly higher total sales.

### Gender

- Female customers accounted for **501 transactions** and generated approximately **USD 167.88K** in sales.
- Male customers accounted for **499 transactions** and generated approximately **USD 155.08K** in sales.
- Average order value was approximately **USD 335.10** for Female customers and **USD 310.79** for Male customers.

### Sales by Hour

- The overall busiest sales hour was **19:00**, generating approximately **USD 39.70K** in sales.
- Another strong period occurred around **13:00**, generating approximately **USD 34.72K** in sales.

### Peak Sales Hour by Branch

The peak sales hour was also analyzed separately for each branch:

- **Branch A:** 11:00, with approximately **USD 11.35K** in sales.
- **Branch B:** 19:00, with approximately **USD 16.26K** in sales.
- **Branch C:** 19:00, with approximately **USD 13.11K** in sales.

This shows that customer purchasing patterns vary across branches. Branch B and Branch C experience their highest sales in the evening, while Branch A reaches its peak around late morning.

### Monthly Sales

Monthly sales were analyzed using the month extracted from the `Date` column.

**January** recorded the highest total sales, at approximately **USD 116K**.

### Gross Margin

- The gross margin percentage was approximately **4.76% across all product lines**.
- Food and beverages generated the highest gross income at approximately **USD 2.67K**.
- Health and beauty generated approximately **USD 2.34K** in gross income.
- Since the gross margin percentage is the same across product lines, differences in gross income mainly reflect differences in sales volume.

### Branch and Product Line Analysis

The heatmap shows that sales performance varies depending on the combination of branch and product line.

- The strongest branch-product combination was **Branch C — Food and beverages**, with approximately **USD 23.77K** in sales.
- The lowest combination was **Branch A — Health and beauty**, with approximately **USD 12.60K** in sales.
- Branch A performed particularly well in Home and lifestyle.
- Branch C performed particularly well in Food and beverages and Fashion accessories.

### Customer Ratings

- The overall average customer rating was **6.97 out of 10**.
- Branch C had the highest average rating at approximately **7.07**.
- Branch A followed with approximately **7.03**.
- Branch B had the lowest average rating at approximately **6.82**.

# Business Insights

### **1. Focus on Branch C**

Branch C generated the highest total sales and had the highest average order value. Although it had fewer orders than Branch A, customers spent more per transaction.

This suggests that Branch C has stronger higher-value purchasing behavior. Management could study its product mix and customer behavior and apply successful practices to other branches.

### **2. Use Different Strategies for Each Branch**

The peak sales hour differs by branch. Branch A reaches its highest sales at **11:00**, while Branch B and Branch C peak at **19:00**.

Therefore, staffing, promotions, and product availability could be planned according to each branch's specific peak period instead of using the same schedule for all branches.

### **3. Strengthen Food and Beverages**

Food and beverages generated the highest total sales at approximately **USD 56.14K**.

The business could maintain strong stock availability for this product line and consider promotions, bundles, or cross-selling strategies to increase sales further.

### **4. Investigate Health and Beauty**

Health and beauty generated the lowest total sales at approximately **USD 49.19K**.

The business could investigate customer demand and consider additional promotions, improved product placement, or product bundles to improve the performance of this category.

### **5. Encourage Higher-Value Purchases**

Home and lifestyle has the highest average order value at approximately **USD 336.64**.

The business could analyze which products contribute to these higher-value transactions and use similar strategies in other product lines.

### **6. Maintain Member Engagement**

Member and Normal customers are almost evenly distributed, but Members generate slightly higher total sales.

Loyalty programs and targeted member promotions could help increase repeat purchases and strengthen customer retention.

### **7. Improve Branch B Customer Experience**

Branch B has the lowest average customer rating at approximately **6.82**, compared with **7.07** for Branch C.

The business could investigate customer feedback, service quality, product availability, and other operational factors at Branch B.

### **8. Plan Around Strong Sales Periods**

The overall peak sales hour is **19:00**, while **13:00** is another strong period.

The business could increase staffing and ensure product availability during these high-demand periods.
