# E-commerce-Sales

## 📊 Project Overview
This Power BI dashboard provides an interactive analysis of e-commerce sales performance across different regions, products, and customer segments.  
It enables stakeholders to monitor key business metrics such as revenue, sales quantity, and customer insights to make data-driven decisions.


## 🎯 Objectives
- Visualize total revenue, quantity sold, and average unit price.
- Analyze year-over-year (YoY) growth trends.
- Identify top-spending customers and best-selling products.
- Understand geographical sales distribution.
- Provide quick insights into overall business performance.


## 📁 Dataset Information
The dataset contains transactional records of an e-commerce business with columns such as:
- Order Date
- Country
- Customer Name
- Product Category
- Quantity Sold
- Unit Price
- Revenue
- Customer Complaints

(Data was cleaned and modeled in Power BI before visualization.)


## 📈 Dashboard Features
### Key Insights
- Total Revenue: $105M  
- Total Quantity Sold: 6M units  
- Average Unit Price: $17.6  
- Customer Count: 9,191   

### Visual Components
- KPI Cards: For revenue, quantity, and unit price performance.
- Line Chart: Monthly sales trends over time.
- Pie Chart: Top 5 customers by spending.
- Bar Chart: Top 5 products by quantity sold.
- Map Visualization: Geographical sales distribution across countries.


## 🧠 Insights Derived
- Highest sales revenue recorded in Bangladesh, India, and Lithuania.
- The CT” product category had the largest sales volume (2.36M units).
- Consistent monthly growth pattern, with slight dips in specific periods.
- Top customers account for a significant share of total revenue.


## 🛠️ Tools & Technologies
- **Power BI Desktop** – Data visualization and dashboard creation  
- Microsoft Excel  – Data preparation and cleaning  
- DAX– For custom calculations and KPIs  


## ⚙️ DAX Measures Used
Some key DAX measures include:
```DAX
Total Revenue = SUM(Sales[Revenue])
Total Quantity = SUM(Sales[Quantity])
Average Unit Price = DIVIDE([Total Revenue], [Total Quantity])
YoY Revenue Growth % = 
    DIVIDE(([Total Revenue] - [Last Year Revenue]), [Last Year Revenue])
Customer Count = DISTINCTCOUNT(Sales[CustomerID])
