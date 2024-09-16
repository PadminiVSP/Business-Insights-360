Overview:
This project focuses on the analysis of hardware peripherals sales across multiple dimensions: region, product, and country. The goal is to provide insightful business metrics and key performance indicators (KPIs) to support decision-making and forecasting.

Data Sources:
Tables used:
dim_customer: Contains customer-related information such as customer IDs, names, and regions.
dim_product: Holds product details including product categories, subcategories, and product IDs.
dim_date: A standard date dimension table used for time-based analysis.
fact_monthly_sales: Stores historical monthly sales data with metrics like sales volume, revenue, and cost.
fact_forecast_sales: Contains forecasted sales data, including future sales predictions and targets.
Data Modeling:
Data Model: A star schema is used for efficient querying and reporting.
Fact Tables:
fact_monthly_sales (historical data)
fact_forecast_sales (forecasted data)
Dimension Tables:
dim_customer, dim_product, dim_date
Aggregated Fact Table: Created by merging and appending sales data in Power Query, simplifying analysis by consolidating actual and forecasted sales into a single fact table.
Key Performance Indicators (KPIs):
The following DAX measures were created to track business performance:

NET PROFIT: Calculated as total revenue minus total expenses.
GROSS MARGIN: Gross revenue minus cost of goods sold.
NET PROFIT %: The percentage of net profit relative to total revenue.
GROSS MARGIN %: The percentage of gross margin relative to total revenue.
YOY (Year-over-Year): Sales growth comparing the current period with the same period in the previous year.
YOY CHANGE %: Percentage change in sales compared to the previous year.
FORECAST ACCURACY: Measure of how accurate the sales forecasts are compared to actual sales.
NET ERROR: Difference between forecasted and actual sales.
ABS ERROR: Absolute difference between forecasted and actual sales.
Tools & Techniques:
Power Query: Used for data extraction, transformation, and loading (ETL). Aggregated and cleaned the data to form the final fact table by merging historical and forecasted sales.
DAX: Dynamic measures and calculations were created for analyzing performance metrics such as profitability, margin, and sales forecasts.
Data Modeling: Implemented a star schema for optimal performance in handling large sales datasets, ensuring efficient querying for analysis.
Insights & Analysis:
The model enables multi-dimensional analysis of sales across regions, products, and countries, helping the business understand which markets and products perform best.
Forecast accuracy measures provide valuable insights into the reliability of sales predictions, enabling better future planning and inventory management.
