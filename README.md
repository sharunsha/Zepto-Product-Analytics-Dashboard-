Zepto Product Analytics Dashboard — SQL + Power BI
Business Problem
Zepto leadership lacked visibility into which product categories drove the most revenue, how stock-outs were impacting sales, and whether their discount strategy was actually profitable.
Tools Used
MySQL · Python (Pandas) · Power BI (DAX, Power Query) · Excel
Dataset

3,732 unique product SKUs across Zepto's full catalog
Attributes: Category, MRP, Selling Price, Discount %, Quantity, Stock Status


What I Did
1. SQL Data Cleaning & Transformation

Converted string values to numeric types for calculations
Removed corrupted records, null values, and outliers
Standardized percentage symbols, currency formats, and inconsistent units
Built optimized analytical tables for Power BI integration

2. SQL Analysis

Used INNER JOIN and LEFT JOIN to combine product, category, pricing, and stock datasets
Applied GROUP BY + HAVING to identify high-performing and underperforming segments
Used SUM, COUNT, AVG subqueries to calculate revenue contribution by category
Built derived summary tables to streamline dashboard reporting

3. Power BI Dashboard

Built interactive dashboard with slicers, drill-through, and KPI cards
Tracked: Total Revenue, Active Products, Out-of-Stock count, Discount Items


Key KPIs
MetricValueTotal Revenue₹12.23 BillionActive Products4,000+ SKUsOut-of-Stock Products453 (12% of catalog)Discounted Items29,000+

Key Findings

The Quantity Paradox: High-volume products don't always generate the most revenue — premium, lower-quantity items often outperform in total margin contribution
12% Stock-Out Rate: 453 products unavailable at any given time, directly causing lost sales and customer dissatisfaction
Discount ROI varies by category: Blanket discounting is ineffective — some categories show strong volume lift, others show minimal response
Beverages was the top revenue-driving category at ₹12Bn+

Business Recommendations

Implement predictive inventory alerts for top 20% revenue-generating SKUs
Shift from blanket discounting to category-specific promotional strategy
Reweight inventory planning from volume metrics to revenue contribution metrics


Dashboard Preview



How to Run

Run the SQL scripts in MySQL to clean and prepare the data
Open Zepto_Dashboard.pbix in Power BI Desktop
Refresh the data source connection

GitHub Repo
github.com/sharunsha/Zepto-Product-Analytics-Dashboard-
