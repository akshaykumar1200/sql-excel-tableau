# Sales Analysis Dashboard

This project provides an interactive dashboard for analyzing sales data, focusing on revenue, units sold, and profit across various dimensions such as time, location, and product categories. Built with Tableau, this dashboard visualizes key metrics to assist stakeholders in understanding business performance and trends.

## Dashboard Overview

### 1. Summary Section
   - **Total Units**: Displays the total units sold.
   - **Profitability at a Glance for TX**: Highlights total revenue and profitability in Texas, with options to filter by year (2016-2018).

### 2. Revenue Analysis
   - **Revenue/Year**: A bar chart showing revenue distribution by year (2016-2018).
   - **Revenue/Month**: A line chart indicating monthly revenue trends, allowing insights into seasonality and monthly fluctuations.

### 3. Geographic Analysis
   - **Revenue/State Map**: A geographic map showing revenue distribution by state, providing a visual of where sales are concentrated.
   - **Revenue/Store**: A pie chart representing revenue share by store, helping identify top-performing locations.

## Usage

1. **Filtering Options**: Use year and state filters to customize the view according to specific timeframes or regions.
2. **Insights Extraction**: Compare yearly and monthly revenues, observe trends, and analyze geographic and store-specific performance.

## Requirements

- **Tableau Desktop**: The dashboard is built using Tableau Desktop, which is required to open and interact with the `.twb` file.
- **Data Source**: The dashboard is connected to a dataset with fields such as order ID, customer details, product information, and sales metrics.

## How to Run

1. Download the `.twb` file and open it in Tableau.
2. Ensure data sources are properly connected or imported.
3. Use interactive filters to explore different aspects of the sales data.

## Key Insights

- Identifies top revenue-generating years and months.
- Highlights profitable regions and stores, especially in Texas.
- Provides a quick view of overall sales performance and trends.


## Summary Section:

Displays key metrics like total units sold and profit for a selected state (e.g., Texas) and year range (2016-2018). It provides a quick overview of performance.
### Revenue Analysis:

Revenue/Year: A bar chart that shows annual revenue for each selected year, allowing a comparison across years.
Revenue/Month: A line chart tracking monthly revenue trends, helpful for identifying seasonal patterns or monthly fluctuations in revenue.

### Geographic Analysis:
Revenue/State Map: A map visual that displays revenue by state, giving a geographical perspective on sales distribution.
Revenue/Store: A pie chart showing revenue contribution by store (e.g., Rowlett Bikes), useful for identifying top-performing stores


## SQL query:

### SELECT Clause:

Selects columns such as order_id, customer details, city, state, order_date, and aggregated values (total_units and revenue).
Joins customer first and last names as 'customer', and staff first and last names as 'sales_rap'.
### Table Joins:

Uses JOIN statements to pull relevant information across multiple tables: orders, customers, order items, products, categories, brands, stores, and staff.
Each join condition specifies a common identifier to connect tables accurately.
### Aggregations and Calculations:

SUM(ite.quantity) calculates the total units per order.
SUM(ite.quantity * ite.list_price) calculates total revenue.
### GROUP BY Clause:

Groups by key fields like order_id, customer and staff names, city, state, order_date, product_name, and other relevant columns.
Ensures aggregation applies accurately across each unique order.

This query gathers detailed sales information per order, integrating customer, product, store, and sales representative details, with computed totals for units and revenue. Let me know if you'd like this translated to a README format for GitHub!







