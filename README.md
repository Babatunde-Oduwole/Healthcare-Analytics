# Healthcare Analysis
![istockphoto-1373659740-612x612](https://github.com/Babatunde-Oduwole/Healthcare-Analytics/assets/167521089/30ea3d7a-101f-4b34-82ac-55238289e6c4)


## Table of Contents

- [Project Introduction](#Project-Introduction)
- [Data Source](#Data-Source)
- [Tools](#Tools)
- [Data Cleaning/Preparation](#Data-Cleaning/Preparation)
- [Exploratory Data Analysis (EDA)](#Exploratory-Data-Analysis)
- [Data Analysis](#Data-Analysis)
- [Findings](#Findings)
- [Recommendations](#Recommendation)
- [Limitations](#Limitations)

### Project Introduction


This business intelligence report aims to provide insight into the sales performance of a retail sales company over the past years, by analyzing various aspect of the sales data, identify trends, make data driven recommendations and gain a deeper understanding of the business performance. 

### Data Source

The primary dataset used for this analysis is the 'sales_dataset.csv' file, containing detailed information about sales made by the company.

### Tools

1. Excel - Data Cleaning
2. MySQL - Data Analysis
3. Power BI - Visualization

### Data Cleaning/Preparation

In the initial data preparation phase, the following tasks were performed:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

### Exploratory Data Analysis (EDA)

EDA involved exploring the sales data to answer key questions, such as:

1. What was the total revenue?
2. What was the cost of sales?
3. What the the profit?
4. What was the profit margin?
5. What was the revenue for each month?
6. What was the revenue from each country?
7. What product generated the highest revenue?
8. What segment generated the highest revenue?
9. What was the revenue by discount band?

### Data Analysis

Some of the interesting code/features worked with include:

```sql
SELECT product, sales
FROM sales_data;
```

```sql
UPDATE sales_data 
SET segment = COALESCE(segment, 0);
```

### Findings
Below are some of the finding discovered after analysis:
1. The company's profit margin have been steadily increasing over the past years, with a noticeable peak during the month of August.
2. The product "Paseo" was the best-performing product in terms of sales and revenue.
3. When analysing the customer segment, it was discovered that the "Government" was the best customer with the high lifetime value (LTV) and should be targeted for marketing efforts.


### Recommendations

Based on the analysis, the following recommendations are suggested for actions:

1. Invest in marketing and promotions during peak sales seasons to maximize revenue.
2. Focus on expanding and promoting Paseo.
3. Implement a customer segmentation strategy to target high-LTV customers effectively.

### Limitations

I had to remove all zero values from all columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both product and revenue figures.


