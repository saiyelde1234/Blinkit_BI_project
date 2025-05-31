🔍 1. Requirement Gathering / Business Understanding Engaged stakeholders (marketing, sales, supply chain) to understand expectations.

Clarified key questions to answer through the dashboard:

Which item types are the most profitable?

How does fat content affect sales and ratings?

Do older or newer outlets perform better?

What’s the distribution of sales across cities?

📂 2. Data Walkthrough & Data Connection Analyzed the structure of datasets (item master, sales data, outlet information).

Identified fields such as Item_Type, Outlet_Size, Fat_Content, Sales, and Rating.

Connected the data to Power BI using Excel as a source.

🧹 3. Data Cleaning / Data Quality Check Standardized Fat_Content categories ("Low Fat", "Regular", "High Fat").

Handled missing values in Outlet_Size and Item_Weight.

Verified data types (Sales as decimal, Outlet_Establishment_Year as date).

Removed duplicate records and outliers (negative sales or ratings above 5).

🧠 4. Data Modeling Applied Star Schema design:

Fact Table: Sales

Dimension Tables: Items, Outlets

Built relationships:

Item_ID connected Item and Sales tables.

Outlet_ID connected Outlet and Sales tables.

Enabled effective filtering and slicing in visuals.

⚙️ 5. Data Processing & DAX Calculations Created meaningful DAX measures for KPIs:

Total Sales = SUM(Sales[Sales_Amount])

Average Sales = AVERAGE(Sales[Sales_Amount])

Number of Items = DISTINCTCOUNT(Items[Item_ID])

Average Rating = AVERAGE(Items[Rating])

Also added:

Year = YEAR(Outlet_Establishment_Year)

Time intelligence measures (YTD, MOM growth) – optional for advanced dashboards.

🗂️ 6. Dashboard Layout Planning Divided the dashboard into:

Summary Cards Section (Top KPIs)

Sales Analysis Section

Outlet & Geography Section

Customer Feedback/Ratings Section

Planned use of filters/slicers for: Outlet Type, Item Type, Location

📊 7. Charts Development & Formatting 🧈 Total Sales by Fat Content Chart Type: Donut Chart

Purpose: Show sales breakdown by fat content.

Tooltips: Include Avg Sales, Avg Rating for each segment.

🍔 Total Sales by Item Type Chart Type: Bar Chart

Purpose: Highlight best-selling item types.

Insight: Identify which categories drive the most revenue.

🏪 Fat Content by Outlet for Total Sales Chart Type: Stacked Column Chart

Purpose: Compare fat content preferences across outlets.

🏢 Sales by Outlet Establishment Year Chart Type: Line Chart

Purpose: Analyze how outlet age affects sales performance.

🏬 Sales by Outlet Size Chart Type: Donut/Pie Chart

Purpose: Discover how store size correlates with revenue.

🗺️ Sales by Outlet Location Chart Type: Funnel Map

Purpose: Visualize geographical sales performance.

🧾 All Metrics by Outlet Type Chart Type: Matrix Card

Purpose: Compare key metrics side-by-side across outlet types.

🧠 8. Insights Generation Key insights from the analysis:

Low Fat items had higher sales and customer ratings.

Medium Outlet Sizes yielded the highest total sales.

Item Type "Frozen Foods" and "Snack Foods" dominated sales.

Outlets established after 2010 showed faster sales growth.

Urban outlet locations generated more consistent and high-volume sales.

💡 9. Final Dashboard Development Developed an interactive Power BI dashboard with:

Responsive filters for outlet, item, and location.

Bookmark buttons for switching between sales and customer views.

Conditional formatting to highlight performance anomalies.

📈 Benefits of This Project Enables data-driven decision-making for marketing, operations, and inventory teams.

Helps Blinkit optimize inventory distribution and tailor product strategy by outlet.

Identifies underperforming outlets and product types to focus improvement efforts.

Provides a scalable reporting solution for real-time performance tracking.

✅ Conclusion The Blinkit Sales & Customer Insights Dashboard built in Power BI provides a powerful, data-driven approach to understanding and improving sales performance, customer satisfaction, and outlet operations.

Through careful data preparation, modeling, and visual storytelling, the dashboard delivers clear insights across various dimensions—such as fat content, item type, outlet size, and location. Key KPIs like Total Sales, Average Sales, Number of Items Sold, and Customer Ratings are made actionable through dynamic and interactive visuals.

Key outcomes of this project:

Identified top-performing item categories and fat content preferences.

Discovered that medium-sized outlets in urban locations drive higher sales.

Revealed a strong correlation between outlet establishment year and revenue trends.

Enabled Blinkit to make informed decisions around product planning, outlet expansion, and customer engagement.

By integrating all business-critical metrics in one interactive platform, this project not only meets the analytical needs of the business but also sets a foundation for continuous performance monitoring and strategic growth. Power BI’s flexibility ensures this dashboard can be expanded or adapted as business priorities evolve.

![Screenshot 2025-05-29 223721](https://github.com/user-attachments/assets/9ae47c99-bcea-4563-b263-3c92dd57ea94)
