# Pizza Sales Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Recommendation](#recommendation)
### Project Overview

This data analysis project aims to provide insights into the sales performance of Pizza Company over the past year. By analyzing various aspects of the sales data, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the company's performance.

### Data Sources

Sales Data: The primary dataset used for this analysis is the "pizza_sales.csv" 

### Tools

- SQL Server - Data cleaning & Analysis
-  PowerBI - Creating reports


### Data Cleaning/Preparation

In the initial data preparation phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting

### Exploratory Data Analysis

EDA involved exploring the sales data to answer key questions, such as:

- Which top 5 sellers by Revenue?
- What is the total Pizzas Sold by Pizza Category?
- What are the Average Pizzas Per Order?

### Data Analysis

Include some interesting code/features worked with
  
  ```sql
  SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_order_Value
  FROM pizza_sales
  ```

  ```sql
  SELECT DATENAME(DW, order_date) AS order_day, COUNT(DISTINCT order_id) AS total_orders 
  FROM pizza_sales
  GROUP BY DATENAME(DW, order_date)
  ```

### Results/Findings

The analysis results are summarized as follows:
1. Orders are highest on Weekend, Friday and Saturday evenings.
2. There are Maximum orders from the months of July and January
3. Classic Category contributes to Maximum sales & total orders
4. Large-size pizza contributes to Maximum sales

### Recommendation

Based on the analysis, we recommend the following actions:
- Focus on expanding and promoting classic Category
- Focus on expanding and promoting Large size

  



   


  







