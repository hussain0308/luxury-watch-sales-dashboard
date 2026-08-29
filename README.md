Luxury Watch Sales Analytics Dashboard

An interactive sales analytics dashboard for the luxury watch market (Rolex, Patek Philippe, Audemars Piguet, Richard Mille), built with Excel and Power BI.

📊 What it does

The dashboard tracks 1,800 sales transactions across 11 watch models, with a dropdown to select any individual watch and instantly view its revenue, units sold, average sale price, and sales trend over time.

🔍 Key finding

Rolex sells in high volume at a lower price point, while Richard Mille sells far fewer units but at a much higher price per piece — both strategies contribute significantly to total revenue ($94.95M), just through very different sales patterns.

🗂️ Data model

Structured as a star schema:

Fact table — fctSales: transaction-level Quantity, Revenue, Sale Price, Region, Retailer Type, Customer Segment
Dimension table — dimWatch: Brand, Model, Category, Base Price, Material, Launch Year
Dimension table — dimDate: Day, Month, Quarter, Year breakdown
Metrics table — dedicated table holding all DAX measures (Total Revenue, Total Quantity, Total Orders, Avg Sale Price, Avg Revenue per Order)

Features:

4 KPI cards (Total Revenue, Total Quantity, Total Orders, Avg Sale Price) that update based on the selected watch
Dynamic trend chart with Year / Quarter / Month / Day toggle
Watch selector slicer for per-model drill-down
🛠️ Tools used
Excel — initial data structuring
Power BI — data modeling (star schema), DAX measures, interactive dashboard design
DAX — Total Revenue, Total Quantity, Total Orders, Avg Sale Price, Avg Revenue per Order, dynamic Chart Title
📁 Files
data/dimWatch.csv — watch dimension table
data/dimDate.csv — date dimension table
data/fctSales.csv — sales fact table
dashboard/watch_sales_dashboard.pbix — Power BI dashboard file
📌 Note on data

This dataset is synthetically generated for this portfolio project, modeled on realistic luxury watch market patterns (pricing tiers, sales volume, seasonality). It does not represent actual brand sales figures.

#DataAnalytics #PowerBI #Excel #DataVisualization
