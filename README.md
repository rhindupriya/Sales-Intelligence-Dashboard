# Sales Analytics Dashboard Project - Power BI + Excel

## Project Objective
Design a professional Sales Analytics Dashboard in Power BI using Excel data sources. The dashboard helps businesses analyze sales performance, customer behavior, profit trends, product performance, and regional performance.

## Business Problems Solved
- Identify revenue growth trends and weak sales months.
- Track profit margin and detect low-margin categories or products.
- Compare regional, state, and city performance.
- Understand top products and customer buying behavior.
- Support business decisions for sales strategy, inventory planning, and customer retention.

## Dataset Fields
The Excel source should contain these columns:

- Order ID
- Product Name
- Category
- Customer Name
- Region
- State
- City
- Sales Amount
- Profit
- Quantity
- Order Date
- Ship Date
- Payment Mode

The main dataset is included in both formats:

- `data/sales_data_complete.csv`
- `data/Sales_Analytics_Dashboard_Data.xlsx`

The current dataset was expanded from `Sales_Dashboard_Big_Dataset.pdf` and contains 8,100 records across 2000-2026. A small sample CSV is also included at `data/sample_sales_data.csv`.

## Dashboard Pages

## Website Dashboard
An interactive website version is included at `website/index.html`. It reads `data/sales_data_complete.csv`, cleans duplicate/null records in the browser, and calculates DAX-style measures for total sales, total profit, total orders, profit margin, average order value, YoY deltas, forecasting, regional analysis, product rankings, payment behavior, and customer segmentation across 2000-2026.

To run it locally:

```bash
python -m http.server 8010
```

Then open:

```text
http://localhost:8010/sales_analytics_powerbi_project/website/index.html
```

### 1. Executive Overview
- Total Sales
- Total Profit
- Total Orders
- Profit Margin %
- Monthly Growth %
- Monthly Sales Trend
- Year-over-Year Sales Comparison

### 2. Product Performance
- Category-wise Sales
- Top 10 Products by Sales
- Sales, Quantity, and Profit by Product
- Drill-down from Category to Product Name

### 3. Customer Insights
- Customer segmentation by total sales and order frequency
- Top customers by revenue
- Repeat vs one-time customers
- Average order value

### 4. Regional Performance
- Region-wise Profit
- State/City drill-down
- Regional sales contribution
- Payment mode behavior by region

### 5. Profitability Analysis
- Sales vs Profit scatter plot
- Profit margin by category and region
- Loss-making or low-margin products
- High-sales but low-profit outliers

## Filters and Slicers
- Year
- Region
- Category
- Payment Mode
- State / City optional drill filters

## Advanced Analytics
- Sales forecasting using Power BI Analytics pane on the monthly line chart.
- Year-over-year comparison using DAX time intelligence.
- Dynamic drill-down from Region to State to City and Category to Product.
- DAX measures for KPI cards and trend calculations.

## Tools Used
- Excel for data cleaning and source preparation
- Power Query for ETL operations
- Power BI for dashboard design and visualization
- DAX for business metrics and KPI calculations

## Expected Outcome
The dashboard gives actionable insights for:

- Revenue growth
- Product performance
- Customer retention
- Regional sales strategy
- Profitability improvement
