Global Superstore Data Analysis Dashboard
A comprehensive Power BI project designed to analyze and visualize the performance of a global retail chain. This dashboard provides deep dives into sales trends, profitability, regional performance, and product categories to support data-driven decision-making.

📊 Project Overview


The dashboard consists of five interactive sections:

Main: An interactive landing page.

Overview: High-level KPIs including Total Sales ($12.64M) and Total Cost.

Data Analysis: Correlation analysis (Sales vs. Profit) and monthly performance trends.

Regional Analysis: Breakdown of performance across global markets and cities.

Product Analysis: Insights into the best-performing categories and specific products.

🗂️ Data Information
Source: The dataset was obtained from Kaggle.

Dataset Topic: Global Superstore Sales.

Domain: Retail, E-commerce, and Supply Chain Management.

Dataset Columns
The final cleaned dataset includes the following fields:

Order Details: Row ID, Order ID, Order Date, Ship Date, Ship Mode, Order Priority.

Customer Details: Customer ID, Customer Name, Segment.

Location: City, State, Region, Region2.

Product Details: Product ID, Product Name, Category, Sub-Category.

Financial Metrics: Sales, Quantity, Profit, Shipping Cost, Cost, Unit Cost, Unit Price.

Time Analysis: Year, weeknum.

🛠️ Data Cleaning & Transformation
To ensure the data was structured for meaningful analysis, I performed the following ETL processes:

1. Column Optimization
I removed redundant or irrelevant columns to improve model performance:

Removed: Discount, 记录数 (Record Count), Market, and Market2.

2. Custom Calculations
Using Power Query Custom Columns, I added essential financial metrics not present in the raw data:

Cost: Calculated to track total expenditure per order.

Unit Price: Established the price point for individual items.

Unit Cost: Established the base cost per individual item.

3. Regional Grouping
The original dataset contained fragmented regions. I performed a Group By operation to consolidate them into four primary logical regions for better high-level reporting:

Asia Pacific

Latin America

North America

Europe & Africa

🧠 DAX & Measures
To power the numerous KPI cards seen throughout the dashboard, I utilized DAX (Data Analysis Expressions) to create dynamic measures:

Aggregations: Calculated Total Sales, Total Profit, Average Sales, and Average Profit to display real-time values in cards.

Top Performers: Developed measures to dynamically identify the Top Category, Top Sub-Category, and Top City based on sales and profit volume.

Gauges: Created measures for the Profit and Average Cost gauges to visualize performance against targets.

📈 Key Insights
Top Region: North America leads the global market in total sales volume.

Profit Drivers: The Technology category is the primary driver for both revenue and profit.

Shipping Trends: Standard Class is the most utilized ship mode, accounting for over 60% of total shipments.

Star Product: The Apple Smart Phone, Full Size stands out as the top product by name.
