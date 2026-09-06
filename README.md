📊 Maven Fuzzy Factory Analytics

🔎 Project Overview

Maven Fuzzy Factory Analytics is an end-to-end data analytics and
business intelligence project built using SQL, Python, and Microsoft
Power BI.

The project analyzes a direct-to-consumer e-commerce business selling
premium plush-toy products. It transforms raw transactional and website
data into an interactive Power BI dashboard covering sales
performance, marketing effectiveness, product profitability, customer
activity, refunds, and geographic distribution.

The objective is to demonstrate a complete analytics workflow --- from
data cleaning and validation to SQL analysis and executive-level
business intelligence reporting.

🗂️ Dataset

The Maven Fuzzy Factory dataset covers the period:

19 March 2012 -- 19 March 2015

Table                 Records / Details

Website Sessions                472,871
Website Pageviews             1,048,575
Orders                           32,313
Order Items                      40,025
Refunds                           1,731
Products                              4

Core Data Areas

🖱️ Website traffic and sessions

📄 Website pageviews and funnel activity

🛒 Orders and transactions

📦 Order-level product information

💸 Refund activity

🧸 Product catalogue and profitability

🔧 Data Cleaning & Preparation

A structured Python/pandas pipeline was developed to prepare the raw
data for analysis.

Key Data Preparation Steps

✅ Parsed and standardized inconsistent datetime formats

✅ Handled missing UTM attribution fields

✅ Standardized categorical values such as channels and device types

✅ Verified referential integrity across the six core tables

✅ Identified potential outliers using the IQR method

✅ Added geographic enrichment for analytical visualization

✅ Prepared clean datasets for SQL and Power BI analysis

🐍 Python & 🗄️ SQL Analysis

Python

A Python/pandas cleaning workflow was created in:

PYTHON_CLEANING.ipynb

The notebook handles data preparation, validation, transformation, and
export of cleaned datasets.

SQL

The cleaned data was loaded into SQLite and analyzed using:

SQL_QUERY.ipynb

The analysis contains 26 analytical SQL queries covering:

Traffic attribution

Conversion and funnel performance

Revenue trends

Marketing channel performance

Product profitability

Refund analysis

Geographic performance

Running totals and ranking analysis

Advanced SQL techniques include:

Common Table Expressions (CTEs)

ROW_NUMBER()

Window functions

Running SUM()

Aggregations and conditional analysis

📈 Power BI Dashboard

The Power BI report presents the analysis through an interactive
multi-page dashboard.

1. 🏠 Home Page

A landing page providing navigation to the major analytical sections of
the report.

2. 📊 Overview Dashboard

Provides an executive-level summary of business performance, including:

Total Revenue

Total Orders

Conversion Rate

Profit Margin

Year-over-year trends

Marketing channel mix

Device distribution

Geographic contribution

3. 📣 Sales & Marketing Dashboard

Analyzes:

Marketing channel performance

Campaign effectiveness

Session-to-order conversion funnel

Revenue contribution

Channel and campaign comparisons

Drill-down analysis

4. 🧸 Product & Geo Dashboard

Analyzes:

Product revenue

Product profitability

Refund rates

Geographic revenue distribution

Country and regional performance

Interactive geographic visualization

📖 Analytical Story Flow

The report follows a structured business-analysis narrative:

1. Landing Overview
↓
2. Business Performance Trends
↓
3. Marketing Channel Effectiveness
↓
4. Product Profitability
↓
5. Geographic Insights & Refund Analysis

This structure allows users to move from high-level KPIs to detailed
operational insights.

🔍 Key Business Insights

📈 Overall Performance

Total Revenue: approximately $1.94M

Total Profit: approximately $1.22M

Overall Conversion Rate: 6.83%

📣 Marketing

Google Search (gsearch) is the dominant traffic channel,
contributing approximately 67% of sessions and revenue in the
analyzed dataset.

🧸 Product Performance

The Original Mr. Fuzzy remains the strongest-performing product
based on revenue and profit contribution.

💻 Device Performance

Desktop users account for approximately 69% of sessions, compared
with 31% from mobile devices.

🌎 Geographic Distribution

The United States contributes approximately 75% of traffic,
while the United Kingdom contributes approximately 25%.

💸 Refunds

Refunds represent approximately 4.32% of order items, with total
refund value of approximately $85,338.69.

🛠️ Technology Stack

Technology             Purpose

Python             Data cleaning and transformation
Pandas             Data manipulation and preparation
SQL / SQLite       Analytical querying
Power BI           Interactive dashboard and visualization
Jupyter Notebook   Python and SQL analysis workflow
GitHub             Version control and project documentation

🚀 How to Use the Project

Power BI Dashboard

Download the .pbix dashboard file from this repository.

Open it using Power BI Desktop.

Navigate through the report pages.

Use slicers, filters, and drill-down functionality to explore the
analysis.

Reproducing the Analysis

To reproduce the analytical workflow:

Obtain the raw Maven Fuzzy Factory datasets.

Run PYTHON_CLEANING.ipynb.

Generate the cleaned datasets.

Run SQL_QUERY.ipynb.

Review the analytical outputs.

Connect the prepared data to Power BI.

Refresh the dashboard.

🔮 Future Improvements

Potential extensions to the project include:

🔄 Automating the Python → SQLite → Power BI refresh pipeline

📈 Adding time-series revenue and conversion forecasting

🎯 Integrating advertising-spend data for true ROAS analysis

🧩 Building customer segmentation using RFM analysis

🗺️ Replacing simulated geographic enrichment with verified
geolocation data

☁️ Publishing the dashboard through Power BI Service

⚡ Implementing automated data-refresh and monitoring workflows

📁 Suggested Repository Structure

MAVEN-FUZZY-FACTORY-DATA-ANALYSIS/
│
├── 📊 MAVEN FUZZY FACTORY DASHBORAD.pbix
├── 🐍 PYTHON_CLEANING.ipynb
├── 🗄️ SQL_QUERY.ipynb
├── 📁 data/
│   ├── customers.csv
│   ├── orders.csv
│   ├── order_items.csv
│   ├── refunds.csv
│   ├── website_sessions.csv
│   └── website_pageviews.csv
│
├── 📄 PROJECT_REPORT.pdf
└── README.md

👤 Author

Taru Sharma

🔗 GitHub: https://github.com/taruattri0014

📧 Contact: taruattri14@gmail.com

⭐ Project Highlights

End-to-End Analytics • Data Cleaning • SQL • Python • Power BI •
Business Intelligence • Data Visualization

DASHBORADS:
<img width="1248" height="730" alt="Screenshot 2026-08-29 192227" src="https://github.com/user-attachments/assets/18952e8b-419a-4806-9758-6c5784b492d8" />

<img width="1235" height="728" alt="Screenshot 2026-08-29 192306" src="https://github.com/user-attachments/assets/67c1f073-92da-4a32-b8fb-22a934772627" />

<img width="1235" height="728" alt="Screenshot 2026-08-29 192306" src="https://github.com/user-attachments/assets/7525a4a4-a5ea-4c26-92b8-ffafea0098a3" />

<img width="1235" height="728" alt="Screenshot 2026-08-29 192306 - Copy (2)" src="https://github.com/user-attachments/assets/e190e9eb-c29c-44aa-8d04-eca66e529219" />





