# -ADDIDAS-U.S-SALES-ANALYSIS-PERFORMANCE
# Adidas US Sales Performance Analysis

## Project Overview

This project analyzes Adidas US sales data covering January 2020 to December 2021. The objective is to evaluate sales performance, operating profitability, product performance, retailer contributions, regional performance and sales channel effectiveness.

The analysis identifies key business trends, highlights areas of strong and weak performance, and provides actionable recommendations to support better business decisions.

An important part of this project was validating and correcting sales calculations before conducting the final analysis to improve the reliability of the reported results.

## Business Objectives

The project aims to answer the following business questions:

1. What are the total sales, operating profit, units sold and operating profit margin?
2. Which product categories generate the highest and lowest sales?
3. Which retailers contribute the most and least to total sales?
4. Which regions and states generate the highest and lowest sales?
5. Which sales method performs best in terms of sales and operating profitability?
6. How does sales performance change over time?
7. What business actions can Adidas take to improve sales and profitability?

## Tools and Technologies

- Microsoft Excel
- Power Query
- Power BI
- DAX

## Dataset Information

| Description | Details |
|---|---|
| Dataset | Adidas US Sales |
| Total Records | 9,648 |
| Original Columns | 13 |
| Countries | United States |
| Analysis Period | January 2020 – December 2021 |
| Retailers | 6 |
| Product Categories | 6 |
| Sales Methods | 3 |
| Regions | 5 |

### Key Dataset Columns

- Retailer
- Retailer ID
- Invoice Date
- Region
- State
- City
- Product
- Price per Unit
- Units Sold
- Total Sales
- Operating Profit
- Operating Margin
- Sales Method

## Data Validation and Correction

During the validation process, a significant calculation inconsistency was identified in the original Total Sales column.

Out of 9,648 records:
- 5,762 records had sales figures consistent with Price per Unit multiplied by Units Sold.
- 3,886 records had sales figures exactly 10 times higher than the calculated amount.
- 4 records had zero units sold.

### Correction Methodology

The affected sales figures were recalculated using:

**Total Sales = Price per Unit × Units Sold**

Operating profit was then recalculated using:

**Operating Profit = Corrected Total Sales × Operating Margin**

The original sales and operating profit values were retained in separate columns to maintain an audit trail.

Other validation checks identified:
- No missing values in the 13 original business columns.
- No exact duplicate business records.
- No negative unit quantities or unit prices.
- Retailer ID was not a reliable unique identifier because some IDs were associated with multiple retailer names.
- City names occurring in multiple states require State and City to be considered together.

**Important assumption:** The correction assumes Price per Unit represents the actual selling price per unit. This interpretation should be confirmed against the original dataset source before the figures are treated as audited financial results.

## Key Performance Indicators

| KPI | Corrected Result |
|---|---:|
| Total Sales | $120.17M |
| Operating Profit | $47.22M |
| Units Sold | 2.48M |
| Operating Profit Margin | 39.30% |

Operating Profit Margin was calculated using:

**Operating Profit Margin = Total Operating Profit / Total Sales × 100**

The overall margin uses total operating profit divided by total sales, rather than a simple average of individual transaction margins.

## Key Findings and Business Insights

### 1. Product Performance

- Men's Street Footwear was the highest-performing product, generating approximately **$27.68 million** in sales.
- Women's Athletic Footwear recorded the lowest sales at approximately **$14.32 million**.
- Men's Street Footwear also recorded the highest operating profit margin among the product categories, approximately **42.01%**.
- Men's Athletic Footwear recorded the lowest product operating profit margin at approximately **36.14%**.

**Business Insight:** Men's Street Footwear is a major contributor to Adidas sales and profitability, while Women's Athletic Footwear represents an opportunity for further investigation.

### 2. Retailer Performance

- West Gear generated the highest sales at approximately **$32.41 million**.
- Amazon recorded the lowest sales at approximately **$10.10 million**.
- Sports Direct recorded the highest retailer operating profit margin at approximately **43.23%**.
- Walmart recorded the lowest retailer operating profit margin at approximately **37.15%**.

**Business Insight:** West Gear is the strongest retailer by sales, while Sports Direct demonstrates the strongest operating profitability relative to its sales.

### 3. Regional Performance

| Region | Total Sales |
|---|---:|
| West | $36.44M |
| Northeast | $25.08M |
| Southeast | $21.37M |
| South | $20.60M |
| Midwest | $16.67M |

- West generated the highest regional sales, contributing approximately **30.32%** of total sales.
- Midwest recorded the lowest regional sales.
- South achieved the highest regional operating profit margin at approximately **44.76%**.
- West recorded the lowest regional operating profit margin at approximately **35.73%**.

**Business Insight:** The West leads in revenue generation, but the South converts a larger proportion of its sales into operating profit.

### 4. State Performance

- New York recorded the highest state sales at approximately **$8.67 million**.
- California followed with approximately **$8.58 million**.
- Nebraska recorded the lowest state sales at approximately **$728,838**.
- Alabama recorded the highest state operating profit margin at approximately **54.44%**.

**Business Insight:** Sales performance varies considerably across states. Nebraska's low sales do not necessarily indicate weak profitability, as its operating profit margin was approximately 43.47%.

### 5. Sales Method Performance

| Sales Method | Total Sales | Operating Profit | Margin |
|---|---:|---:|---:|
| Online | $44.97M | $19.55M | 43.48% |
| Outlet | $39.54M | $14.91M | 37.72% |
| In-store | $35.66M | $12.76M | 35.78% |

- Online generated the highest sales and operating profit among the three sales methods.
- Online also recorded the highest operating profit margin at approximately **43.48%**.
- In-store recorded the lowest sales and operating profit margin.

**Business Insight:** Online sales are an important contributor to both revenue and operating profitability in the dataset.

### 6. Monthly Sales Trends

- July 2021 recorded the highest monthly sales at approximately **$10.37 million**.
- July 2021 also generated the highest monthly operating profit at approximately **$4.10 million**.
- December 2020 recorded the lowest monthly sales at approximately **$1.08 million**.
- June 2020 recorded the lowest monthly operating profit at approximately **$307,046**.

**Business Insight:** July 2021 was the strongest month in the dataset, while December 2020 and June 2020 recorded weaker results on sales and operating profit respectively.

**Time-period limitation:** The dataset contains 1,302 records for 2020 and 8,346 records for 2021. The unequal record coverage means year-over-year comparisons should be interpreted cautiously.

## Business Recommendations

Based on the findings, the following recommendations are proposed:

### 1. Strengthen Product Strategy
- Maintain the availability of high-performing products, particularly Men's Street Footwear.
- Investigate the lower sales contribution of Women's Athletic Footwear.
- Review product pricing, demand and promotional performance to identify opportunities for improvement.

### 2. Improve Retailer Performance
- Maintain strong business relationships with West Gear.
- Investigate the factors contributing to Amazon's lower sales contribution.
- Study Sports Direct's operating profitability and identify practices that could benefit other retail partners.

### 3. Optimize Regional Performance
- Maintain strong market coverage in the West.
- Investigate opportunities to improve sales in the Midwest.
- Study the South's higher operating profit margin to identify potentially transferable business practices.

### 4. Expand Online Sales Opportunities
- Explore opportunities to grow the online sales channel.
- Maintain the outlet channel while monitoring its profitability.
- Investigate the lower operating profit margin recorded by in-store sales.

### 5. Improve Inventory and Sales Planning
- Use monthly sales trends to plan inventory ahead of stronger sales periods.
- Prepare for periods such as July, which recorded the highest sales.
- Investigate weaker months to identify opportunities for improved sales planning.

## Conclusion

The corrected analysis shows that Adidas generated approximately **$120.17 million in sales**, **$47.22 million in operating profit**, and an overall operating profit margin of **39.30%** under the stated calculation assumption.

Men's Street Footwear was the leading product by sales, West Gear was the leading retailer, the West was the highest-performing region by revenue, and Online was the strongest sales method by both revenue and operating profit margin.

The findings highlight opportunities to strengthen product performance, improve regional and retailer results, and expand the online sales channel.

The project demonstrates the importance of data validation, accurate calculations, business-focused analysis and communicating actionable insights.

---
