# Customer Shopping Behavior Analysis Project

Welcome to the Data Warehouse and Analytics Project repository! 🚀<br />
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

-------------------------------------------------------------------------------------

## 📖 Overview

End-to-end analytics pipeline turning raw shopping transactions into business insights:

+ Python (Jupyter): data cleaning, EDA, feature engineering, export of clean tables

+ PostgreSQL: persistent storage, SQL for KPIs and slice-and-dice analysis

+ Power BI: [interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiOTAzMGJhNGMtYjMxZi00ZWRiLTlmN2EtOWU5NDAzODVlM2QyIiwidCI6IjEzZTNiMTg2LWM0NDYtNGFhYi05YzZkLTlhYjliYjc2ODE2YyIsImMiOjh9)
 for storytelling and decision support
  
----------------------------------------------------------------------------------

## 🚀 Pipeline

![Flow: CSV → Python (clean/engineer) → PostgreSQL (raw → core → mart) → Power BI (DAX + visuals)](https://github.com/koteeshv08/customer_behavior_analysis/blob/main/docs/flowchart.png)


1. Raw Data → Python (Jupyter)

   Standardize schema (snake_case), handle missing values, engineer features (e.g., age_group, frequency metrics).

   Output: cleaned CSV/DF for DB load.

2. Python → PostgreSQL

   Bulk-load to fact_purchases + dimension lookups.

   Create indexes and views for dashboard performance.

3. PostgreSQL → Power BI

   Connect via native PostgreSQL connector.

   DAX measures for revenue, AOV, repeat-rate; visuals for segments, products, shipping, discounts.

------------------------------------------------------------------------------------------

## What’s Included

notebook/ – the Jupyter workflow (EDA → clean → export)

db/ – sample queries (revenue by gender, top products, subscriber impact)

dashboard/ – Power BI .pbix file (update connection and refresh)

------------------------------------------------------------------------------------------

## Reproduce

Run the notebook to generate cleaned outputs and load to PostgreSQL.

Execute schema and helper views in db/schema.sql.

Open the .pbix, point to your DB, click Refresh.

------------------------------------------------------------------------------------------

## 🛠️ Tech Stack

Python • Pandas • SQL • PostgreSQL • Power BI

-------------------------------------------------------------------------------------------

## 👋 Contact

Koteesh — Data Analytics & BI

LinkedIn: https://www.linkedin.com/in/t-v-koteesh/

Email: koteesh85@gmail.com
