# FashionWave Retail Sales Analysis | Power BI

## Project Overview

FashionWave is a retail business operating across 50 stores in India. This project analyzes two years of retail transaction data to evaluate sales performance, product profitability, discount effectiveness, store-level performance, customer segments, and weekend versus weekday sales patterns.

The objective is to transform raw transaction data into actionable business insights using **Power BI, Power Query, DAX, and data visualization**.

The analysis focuses on identifying revenue opportunities, protecting profit margins, improving store performance, and developing more effective customer and promotional strategies.

## Business Objectives

- Analyze overall sales, profit, and profitability.
- Identify product categories contributing the most revenue and profit.
- Compare weekend and weekday sales performance.
- Evaluate the relationship between discounts and profit margins.
- Identify high-performing and underperforming stores.
- Analyze new versus returning customer performance.
- Recommend data-driven actions to improve retail performance.

## Tools & Technologies

- **Power BI Desktop** — data modeling, DAX measures, and interactive dashboards.
- **Power Query** — data cleaning and transformation.
- **DAX** — KPI calculations and analytical measures.
- **Microsoft Excel / CSV** — transaction data preparation and validation.
- **GitHub** — project documentation and portfolio management.

## Dataset Overview

The analysis uses a transaction-level retail dataset covering January 2023 to December 2024.

- **Transactions:** 100,000
- **Stores:** 50
- **Product categories:** Clothing, Accessories, and Shoes
- **Customer segments:** New and Returning, with an Unknown category retained for missing customer information
- **Payment methods:** Cash, Card, and Digital

### Key Fields

| Field | Description |
|---|---|
| InvoiceNo | Transaction identifier |
| Date | Transaction date |
| StoreID | Store identifier |
| ProductID | Product identifier |
| Category | Product category |
| Quantity | Units purchased |
| UnitPrice | Selling price per unit |
| Discount | Discount rate applied |
| CostPerUnit | Cost to the business per unit |
| CustomerType | New or Returning customer |
| PaymentMode | Payment method |

*Note: The dataset used for this portfolio case study is a simulated dataset created for analytical practice. Findings represent the dataset and should not be interpreted as actual FashionWave business results.*

## Data Preparation

The data preparation process included:

1. Reviewing the dataset structure, column types, and data quality.
2. Identifying missing values in Discount and CustomerType.
3. Replacing missing discount values with 0% for the analysis.
4. Categorizing missing customer information as Unknown rather than assuming a customer segment.
5. Validating numeric fields used in revenue, cost, and profitability calculations.
6. Creating analytical measures and a Day Type classification for weekend versus weekday analysis.

## Key Performance Indicators (KPIs)

The dashboard evaluates the following KPIs:

| KPI | Calculation / Purpose |
|---|---|
| Total Sales | Quantity × Unit Price × (1 − Discount), summed across transactions |
| Total Profit | Net Sales − Total Cost |
| Profit Margin % | Total Profit ÷ Total Sales |
| Average Order Value (AOV) | Total Sales ÷ Distinct Invoice Count |
| Units Sold | Sum of Quantity |
| Discount Impact | Comparison of profit margins across discount levels |
| Weekend vs Weekday Sales Ratio | Weekend Sales ÷ Weekday Sales |

## Executive Summary

| KPI | Result |
|---|---:|
| Total Sales | ₹24.35 Cr |
| Total Profit | ₹8.06 Cr |
| Profit Margin | 33.1% |
| Average Order Value | ₹2,435 |
| Units Sold | 203.6K |
| Transactions | 100,000 |

*Values are rounded for presentation.*

## Key Business Insights

### 1. Product Category Performance

- **Shoes** generated approximately ₹13.13 Cr in sales, contributing around 53.9% of total revenue, making it the leading category by sales and profit.
- **Clothing** generated approximately ₹6.97 Cr in sales and recorded the highest unit volume, with about 73.3K units sold.
- **Accessories** generated approximately ₹4.25 Cr in sales and had the lowest category profit margin, at around 31.5%.

**Business implication:** Protect the performance of Shoes, use Clothing's unit volume to explore complementary selling opportunities, and review Accessories pricing, costs, and discounting.

### 2. Weekend vs Weekday Sales

- Weekend sales were approximately ₹6.93 Cr, compared with ₹17.42 Cr on weekdays.
- Weekend sales were approximately 0.40 times weekday sales.
- Weekends represented about 28.5% of total revenue.
- Average sales per calendar day were nearly equal: weekend sales per day were only around 0.6% lower than weekday sales per day.

**Business implication:** The lower total weekend revenue is partly explained by there being fewer weekend days. The opportunity is to increase weekend sales through targeted promotions, product availability, and customer engagement rather than assuming weekend demand is significantly weaker.

### 3. Discount Effectiveness and Profitability

The analysis indicates a clear association between higher discount levels and lower profit margins.

| Discount Level | Profit Margin |
|---|---:|
| No Discount | 40.5% |
| Low: 1–15% | 33.4% |
| Mid: 16–25% | 23.7% |
| High: 26–30% | 14.9% |

**Business implication:** Use moderate discounts selectively, evaluate the incremental sales generated by promotions, and reserve deeper discounts for controlled clearance or specific strategic objectives. These comparisons show an association, not proof that discounts alone caused the margin differences.

### 4. Store Performance

- The five highest-sales stores averaged approximately ₹5.79 million in sales.
- The five lowest-sales stores averaged approximately ₹4.02 million.
- Average sales for the top five stores were around 43.8% higher than for the bottom five.

**Business implication:** Investigate transaction volume, product availability, assortment, local demand, and marketing execution at lower-performing stores. These are hypotheses to validate because the dataset does not include store footfall, staffing, or local marketing expenditure.

### 5. Customer Segmentation

- Returning customers contributed approximately 57.0% of total revenue.
- New customers contributed approximately 42.6% of total revenue.
- Returning customers had an average order value of approximately ₹2,451, compared with ₹2,413 for new customers.

**Business implication:** Strengthen retention through loyalty initiatives, repeat-purchase campaigns, and relevant cross-selling. For new customers, prioritize post-purchase engagement and conversion to a second purchase.

### 6. Payment Mix

- Card payments contributed approximately 45.3% of revenue.
- Digital payments contributed approximately 37.2%.
- Cash payments contributed approximately 17.5%.

**Business implication:** Continue supporting convenient digital and card payment experiences while maintaining payment options that serve different customer preferences.

## Strategic Recommendations

### Short-Term Priorities

1. Review discounts above 15% for profitability and business justification.
2. Develop targeted weekend campaigns and measure their incremental performance.
3. Investigate the sales-volume gap between high- and low-performing stores.
4. Use complementary product recommendations to support cross-category sales.
5. Launch repeat-purchase campaigns for returning customers and follow-up journeys for new customers.

### Longer-Term Priorities

1. Monitor store performance using sales, profit, margin, and transaction KPIs together.
2. Build category-level pricing and promotional strategies based on profitability.
3. Track campaign performance against a baseline or control group where possible.
4. Establish recurring reporting for sales trends, customer segments, and discount effectiveness.

## Power BI Dashboard

The Power BI report brings together the following analytical views:

- Executive sales and profitability overview
- Product category performance
- Weekend versus weekday comparison
- Monthly sales trends
- Discount and profit margin analysis
- Store performance comparison
- Customer segmentation
- Payment mix and product volume

The report file is available in the `PowerBI` folder.

## Project Deliverables

- **Power BI report:** Interactive analytical report and KPI measures.
- **Presentation:** Summary of the analysis, key insights, and recommendations.
- **README:** Business context, methodology, KPIs, and findings.

## Repository Structure

```text
## Repository Structure

```text
fashionwave-retail-sales-analysis/
│
├── Dataset/
│   └── fashionwave_sales.csv
│
├── PowerBI/
│   └── FashionWave_Retail_Sales_Analysis.pbix
│
├── Presentation/
│   └── FashionWave_Retail_Sales_Analysis_Final.pptx
│
├── Dashboard/
│   └── dashboard-preview.png
│
└── README.md
```

**Folder Guide**

- `Dataset/` — Source transaction data used in the analysis.
- `PowerBI/` — Power BI report containing the dashboard, data model, and analytical measures.
- `Presentation/` — Final presentation summarizing the analysis, business insights, and recommendations.
- `Dashboard/` — Optional preview image of the completed dashboard.
- `README.md` — Project overview, methodology, KPIs, key findings, and recommendations.
```

*The dashboard preview is optional. Update the file names in this structure to match the files you actually upload.*

## Conclusion

This project demonstrates how Power BI can turn transaction-level retail data into business-focused insights. The analysis highlights the importance of category performance, discount discipline, store-level investigation, customer retention, and targeted weekend growth initiatives.

The overall recommendation is to **grow sales while protecting profitability**, using measurable promotional strategies and ongoing performance monitoring.

---

**Project Type:** Retail Business Intelligence & Sales Analytics  
**Primary Tool:** Microsoft Power BI  
**Skills Demonstrated:** Data Cleaning, Power Query, DAX, KPI Development, Profitability Analysis, Customer Segmentation, Data Visualization, and Business Recommendations