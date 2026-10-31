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

## 📈 Key Business Insights
Based on the analysis of the retail sales data, the following insights were identified:

- **Regional Disparities:** The West and East regions generate significantly higher revenue compared to the Central and South regions. This suggests a need for targeted marketing or operational review in underperforming areas.
- **Product Focus:** Office equipment (specifically copiers and binding machines) and Technology products are the primary revenue drivers. Furniture and Office Supplies contribute minimally to profits.
- **Seasonal Trends:** Sales data exhibits strong seasonality with predictable peaks in November and December, correlating with holiday shopping behavior. This insight can inform inventory management and staffing decisions.
- **Shipping Preferences:** Analysis of shipping modes revealed that customers predominantly choose standard shipping options, indicating price sensitivity over speed.

These findings highlight the importance of strategic resource allocation and targeted marketing to maximize revenue and mitigate risks in underperforming segments.
## 💻 SQL Queries Used
Below is an example of the SQL logic used to extract regional sales performance:

```sql
SELECT 
  Region,
  SUM(Sales) as Total_Sales,
  COUNT(*) as Number_of_Orders,
  ROUND(AVG(Sales), 2) as Average_Order_Value
FROM `project.retail_sales_analysis.sales_data`
GROUP BY Region
ORDER BY Total_Sales DESC;
```

## 🚀 How to Replicate This Analysis
1. **Data Source:** This project uses the Superstore Sales Dataset (available on Kaggle).
2. **Cloud Setup:** Upload the dataset to your own Google Cloud BigQuery instance.
3. **Analysis:** Adapt the SQL queries provided in this repository to perform your own analysis.
4. **Visualization:** Export results to your preferred BI tool (e.g., Google Sheets, Tableau, Power BI) for visualization.

*Note: This project is for educational and portfolio purposes only.*

## 📬 Contact

Adil Loan

LinkedIn: www.linkedin.com/in/adil-loan
Email: adilloan123@gmail.com
Location: Varanasi, India
