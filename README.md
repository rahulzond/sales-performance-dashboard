# Sales Performance Dashboard

Interactive Excel dashboard that tracks sales KPIs, monthly trends, category and rep performance, and customer segment mix — with a live region filter that drives every chart and metric.

## Problem statement

Sales teams need a quick way to see how revenue is performing across regions, products, and reps without digging through raw transaction data. This project turns a flat sales log into a self-service dashboard where a single filter selection updates every KPI and chart instantly.

## Screenshot

![Dashboard screenshot](screenshot.png)

*(Replace `screenshot.png` with an actual screenshot of the Dashboard sheet before uploading — see instructions below.)*

## Features

- **Interactive region filter** — a dropdown (All / North / South / East / West) drives every table and chart on the dashboard using dynamic `SUMIFS` / `COUNTIFS` formulas, simulating drill-down BI behavior natively in Excel
- **KPI cards** — Total Sales, Total Orders, Total Units Sold, Average Order Value, Top Category
- **Monthly sales trend** — 12-month line chart to spot seasonality
- **Category breakdown** — bar chart comparing revenue across product categories
- **Sales rep performance** — bar chart with conditional color-scaling to flag top and bottom performers
- **Customer segment split** — pie chart showing Retail vs Wholesale vs Online revenue share
- Fully formula-driven — no hardcoded values, so the dashboard recalculates live when data changes

## Tools used

- Microsoft Excel (formulas: `SUMIFS`, `COUNTIFS`, `INDEX`/`MATCH`, `IF`, `TEXT`)
- Data validation (dropdown-based filter control)
- Conditional formatting (color scales)
- Native Excel charts (line, bar, pie)

## Dataset

Sample dataset of 400 simulated sales transactions (Aug 2025 – Jul 2026) across 4 regions, 4 product categories, 6 sales reps, and 3 customer segments. Columns: Order ID, Date, Region, Category, Product, Sales Rep, Customer Segment, Payment Method, Units Sold, Unit Price, Sales Amount (calculated), Month (calculated).

## Key insights

*(Replace with your own findings once you explore the dashboard — a couple of examples below)*

- Electronics and Home Appliances together account for over 65% of total revenue
- [Region] shows the highest average order value but lowest order volume, suggesting an opportunity to grow order frequency there
- [Top rep] outperforms the team average by X%

## How to use

1. Download `Sales_Performance_Dashboard.xlsx`
2. Open the **Dashboard** sheet
3. Use the **Filter by Region** dropdown (cell B4) to view metrics for a specific region, or "All" for company-wide totals
4. Replace the **Raw Data** sheet with real transaction data to reuse this dashboard for any sales dataset with the same structure

## Files

- `Sales_Performance_Dashboard.xlsx` — the full workbook (Raw Data + Dashboard sheets)
- `screenshot.png` — dashboard preview image
