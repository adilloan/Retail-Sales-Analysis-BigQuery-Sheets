# Retail Sales Analysis Dashboard

## 📊 Project Overview
This project performs a comprehensive analysis of retail sales data to identify revenue trends, top-performing products, and regional sales performance. The primary objective was to demonstrate proficiency in cloud data management, SQL querying, and data visualization while deriving actionable business insights.

**Live Dashboard:** [Insert Your Google Sheets Link Here]

## 🛠 Tools & Technologies
- **Data Storage & Querying:** Google Cloud BigQuery (SQL)
- **Data Visualization:** Google Sheets
- **Data Source:** Superstore Sales Dataset (Kaggle)
- **Project Management:** GitHub

## 🔍 Methodology
1. **Data Ingestion:** Uploaded raw CSV data to Google Cloud BigQuery, ensuring data integrity and security.
2. **Data Extraction:** Executed complex SQL queries to aggregate and analyze sales data by region, product, time period, and customer segment.
3. **Data Visualization:** Exported query results to Google Sheets to build an interactive dashboard with charts and trend analysis.
4. **Insight Generation:** Identified key business insights including seasonal trends, regional performance disparities, and product-level revenue drivers.

## 📈 Key Findings
- **Regional Performance:** The West region generates the highest revenue, followed by the East. The South region shows the lowest sales volume, indicating a potential market for expansion or a need for strategic review.
- **Product Strategy:** Office equipment (copiers, binding machines) and Technology products are the primary revenue drivers. Furniture and Office Supplies show lower performance.
- **Seasonal Trends:** Sales data exhibits strong seasonality with significant peaks in November and December, correlating with holiday shopping behavior.
- **Shipping Preferences:** Analysis of shipping modes revealed customer preferences that could inform logistics and pricing strategies.

## 💻 SQL Queries Used
Below is an example of the SQL logic used to extract regional sales performance:

```sql
SELECT 
  Region,
  SUM(Sales) as Total_Sales,
  COUNT(*) as Number_of_Orders,
  ROUND(AVG(Sales), 2) as Average_Order_Value
FROM `YOUR_PROJECT_ID.retail_sales_analysis.sales_data`
GROUP BY Region
ORDER BY Total_Sales DESC;
```

##🚀 How to Use This Project

View the Live Dashboard: Click the link above to interact with the Google Sheets dashboard.
Replicate the Project:
Download a similar dataset from Kaggle.
Upload it to your own Google Cloud BigQuery instance.
Adapt the SQL queries provided in this README for your analysis.
Visualize the results in your preferred BI tool.

##📬 Contact

Adil Loan

LinkedIn: www.linkedin.com/in/adil-loan
Email: adilloan123@gmail.com
Location: Varanasi, India
