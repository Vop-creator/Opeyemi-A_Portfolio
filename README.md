# Electronic Sales Performance

I analyzed an electronic sales dataset in Power BI by cleaning and modelling the data, creating a custom Date table and DAX time-intelligence measures to reveal sales trends, channel performance, and profitability insights that support better business decisions.


## Project Type Flags

- [x] Exploratory Data Analysis (EDA)
- [x] Dashboard / Data Visualization
- [x]  ETL
- [x] Data Cleaning/ Modelling
- [x] End-to-End


## Table of Contents
1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Data Workflow](#4-data-workflow)
5. [Analysis & Metrics](#5-analysis--metrics)
6. [Key Insights](#6-key-insights)
7. [Recommendations](#7-recommendations)
8. [Assumptions & Limitations](#8-assumptions--limitations)
9. [Author](#9-author)



## 1. Project Overview

An electronics company was generating large amounts of sales data across different channels, product categories, and regions, but did not have a clear way to analyze overall performance. The goal of this project was to understand sales trends over time, identify the most profitable sales channels and product categories, and determine which regions were driving business growth. To address this, the dataset was cleaned and transformed in Power BI using Power Query, and a data model with a custom Date table and time-intelligence measures was created using DAX. The results were presented in an interactive Power BI dashboard that highlighted key insights such as strong year-on-year sales growth, the dominance of the reseller channel, high-margin product categories, and regional performance differences that could guide future expansion.


## 2. Objectives

- Determine overall sales performance across channels, product categories, and regions using an interactive Power BI dashboard.
- Identify the top three product categories contributing the highest revenue and profit margins.
- Quantify sales growth trends over time using time-intelligence measures such as Year-over-Year and Month-over-Month comparisons.
- Evaluate regional sales performance to determine which regions contribute most to overall revenue.


## 3. Project Scope & Tools

### Scope

 - **In Scope**: "Sales transaction data including revenue, product categories, sales channels, and regional performance. Analysis focuses on identifying sales trends, top-      performing categories, and regional contributions using Power BI visualizations"
 - **Out of Scope**: "Customer demographic information and marketing campaign data were excluded because the dataset only contains sales transactions, product categories, channels, and regions."
 - **Time Period**: Dec 2012 - Dec 2015
 - **Granularity**: Transaction-level sales records aggregated into monthly, category-level, and regional summaries for analysis.

### Tools & Technologies

 - Data Storage: CSV files
 - Data Processing: Power Query
 - Analysis: Power BI
 - Visualization: Power BI
 - Version Control: Git / GitHub
 - Documentation: Markdown


## 4. Data Workflow

  1. Source: "Monthly CSV sales exports from the company."
  2. Extraction: "Imported CSV file into Power BI."
  3. Cleaning/Transformation: "Removed Duplicates.
                Fixed missing values.
                Standardized data types and date formats in the datasets.
                Created Date table, Time intelligence measures."
  5. Modelling: Created a star-scheme realtionship beween the data
  6. Analysis: "Built dashboards to see trends, top channels, and profit margins."
  7. Output: "Summary report (PDF)

```
[Data Source(s)]
      ↓
[Extraction]
      ↓
[Cleaning & Transformation]
      ↓
[Analysis / Modelling / Querying]
      ↓
[Output / Visualisation / Reporting]
```


## 5. Analysis & Metrics

### Analytical Approach

I explored patterns in sales over time and across channels, product categories, and regions. Using Power BI, I calculated KPIs such as Total Sales, Profit, Profit Margin, Sales YTD, Sales SPLY, and Sales YoY %, then visualized them to identify growth trends, top performers, and regional opportunities.”

### Key Metrics Defined

 - `[Total Sales]`: It measures the total revenue generated from all sales transactions. It helps understand overall business performance and revenue generation.
 - `[Total Profit]`: It measures the total money earned after subtracting costs from sales. It shows the company’s profitability and efficiency.
 - `[Profit Margin]`: It measures profit as a percentage of total sales. It indicates how much revenue translates into actual profit, guiding pricing or product decisions.
 - `[Sales Year-to-Date (YTD)]`: It measures cumulative sales from the start of the year up to the current date. It reveals growth trends and progress toward yearly sales targets.
 - `[Sales Same Period Last Year (SPLY)]`: It measures sales during the same time period in the previous year. It allows year-over-year comparisons to evaluate business growth.
 - `[Sales Year-on-Year %]`: It measures the percent change in sales compared to the same period last year. It quantifies growth and highlights trends in a way that’s easy to compare across periods.

### Methods Used

- Dax Measure to calculate total sales, total profit, and profit margin.
- Trend analysis across months, comparing the sales of the current year to the same period last year to track sales growth and seasonal patterns.
- Sales comparison by sales channel, product category, and region.
- Time-intelligence calculations using DAX, including Sales YTD, Sales QTD, SPLY, and Sales YoY %.
- Transformation logic in Power BI, including creating a Date table and computing KPIs for interactive dashboards.


## 6. Key Insights

1. Reseller sales dominate the business, contributing ₦32.19M, more than double Online and Physical Store sales. This indicates that reseller relationships are critical and should be prioritized in strategic planning and incentives.
2. Computers are the top-selling product category, generating ₦22M in revenue, while Music products have the highest profit margin at 60.65%. This suggests the company should focus on both high-volume and high-margin products to maximize profits.
3. Sales peaked in October and were lowest in February, revealing strong seasonal patterns. Marketing campaigns and inventory management should focus on peak months, while low months could be targeted with clearance sales or operational optimizations
4. South East and South South regions account for the majority of sales, while the Federal and Northern zones underperform. This highlights untapped market opportunities and suggests that targeted promotions in underperforming regions could drive growth.
5. Total sales consistently outperformed the same period last year (SPLY), with a year-on-year growth of 39.76%, demonstrating strong business growth and validating the effectiveness of current sales channels and strategies.


## 7. Recommendations

  Priority: High
   - Recommendation: "Offer volume-based incentives or exclusive deals to resellers to secure                    and grow this channel."
   - Based on: Insight 1 - Resellers contribute the majority of revenue
   - Owner: Sales / Channel Management team
  
  Priority: High
   - Recommendation: "Increase inventory and marketing efforts in October–November to                             capitalize on peak sales."
   - Based on: Insight 3 - Sales peak in October and February is the lowest month.
   - Owner: Sales & Marketing team

  Priority: High
   - Recommendation: "Launch targeted campaigns in underperforming regions (Federal and                          Northern zones) to increase awareness and sales."
   - Based on: Insight 4 - South East and South South regions dominate sales; others                                  underperform.
   - Owner: Regional Sales / Marketing team

 Priority: Medium
   - Recommendation: "Promote high-margin products like Music and Cameras alongside top-                         volume products like Computers to maximize profitability."
   - Based on: Insight 2 - Computers have the highest sales volume; Music has the highest                             profit margin.
   - Owner: Product Management / Marketing team


## 8. Assumptions & Limitations

**Assumptions:**
 - All sales transactions in the dataset are complete and accurately recorded.
 - Dates and sales amounts are consistent and represent the true order and revenue information.

**Limitations**:
 - The dataset does not include customer demographic or marketing campaign data, so insights cannot account for buyer behavior or promotional impact.
 - Returns or refunds are not distinguished, so profit calculations assume all recorded sales contribute to revenue without adjustment for returns.
 - Regional comparisons may be affected by missing or underreported sales in some zones, limiting the accuracy of insights for those areas.




## 9. Author

**OPEYEMI PRECIOUS ALALADE**
Financial Data Analyst

- 🔗 [www.linkedin.com/in/opeyemialaladeprecious]
- 💼 [Portfolio or GitHub profile URL]
- 📧 [opalalalde@gmail.com]



