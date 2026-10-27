# RetailPulse — Sales & Business Performance Analytics

An industry-style Data Analyst portfolio project using **Excel + Power BI + Power Query + DAX**.

## Project Goal

Analyze retail sales, profit, customers, products, regions, sales channels, payments and returns to identify business trends and actionable opportunities.

## Tools

* Microsoft Excel
* Power Query
* Power BI Desktop
* DAX
* Python (optional dataset generator)

## Project Workflow

1. Generate/import `Data/Sales\_Data.xlsx`
2. Clean and validate the data in Excel (Refer to the - 'Excel Data_Cleaning_Steps.md in Documentation Folder).
3. Load the cleaned tables into Power BI.
4. Build a star-schema data model.
5. Created the DAX measures in `PowerBI/DAX\_Measures.dax`.
6. Build the five dashboard pages:

   * Executive Overview
   * Sales Analysis
   * Product Analysis
   * Customer Analysis
   * Regional Performance
7. Add slicers for Date, Region, Category, Sales Channel and Customer Segment.
8. Document key findings and recommendations.

## Dataset -25000+ Rows Data

The included workbook contains:

* `Sales\_Data`: transaction-level data
* `Products`: product master
* `Customers`: customer master
* `Regions`: region/state/city mapping
* `Date`: calendar table

## Power BI Model

Recommended relationships:

* `Date\[Date]` 1 → \* `Sales\_Data\[Order\_Date]`
* `Products\[Product\_ID]` 1 → \* `Sales\_Data\[Product\_ID]`
* `Customers\[Customer\_ID]` 1 → \* `Sales\_Data\[Customer\_ID]`
* `Regions\[State]` 1 → \* `Sales\_Data\[State]`

## Suggested KPIs

* Total Sales
* Total Profit
* Total Orders
* Total Customers
* Total Quantity
* Average Order Value
* Profit Margin
* Return Rate
* YoY Growth

## 📌 Key Business Insights & Recommendations
* Top Revenue Drivers: Electronics category and Western Region generated the highest overall sales.
* Profitability Focus: Specific low-margin items identified for pricing/discount optimization.
* Customer Segment: High-value customers contribute over 50% of the revenue.
* Returns Management: State/Category lines with high return rates require quality check.