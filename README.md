
📊 Power BI Project – Maven Fuzzy Factory Analytics

🔎 Overview
This project leverages SQL, Python, and Power BI to analyze the Maven Fuzzy Factory dataset — a direct-to-consumer e-commerce business selling premium plush-toy products. The dashboard provides interactive insights into sales, marketing channels, product performance, and geographic distribution. The goal is to showcase an end-to-end analytics workflow, from raw data cleaning through to business intelligence reporting.

🗂 Dataset
Maven Fuzzy Factory is a real-world-style e-commerce dataset covering 19 March 2012 – 19 March 2015. It contains data about:

Website Sessions 🖱️ (472,871 records)
Pageviews 📄 (1,048,575 records)
Orders 🛒 (32,313 records)
Order Items 📦 (40,025 records)
Refunds 💸 (1,731 records)
Products 🧸 (4 products)

🔧 Data Cleaning & Preparation
✅ Parsed inconsistent datetime formats across all tables
✅ Filled missing UTM attribution fields (utm_source, utm_campaign, utm_content)
✅ Standardized categorical text (channel names, device types)
✅ Verified referential integrity across all six tables (zero orphan records)
✅ Detected outliers using the IQR method on price, COGS, and refund fields
✅ Added simulated geographic enrichment (country, state/region, city) mapped to U.S. Census regions

🐍 Python + 🗄️ SQL Analysis
✅ Built a Python/pandas cleaning pipeline (PYTHON_CLEANING.ipynb)
✅ Loaded cleaned data into SQLite and ran 26 analytical SQL queries (SQL_QUERY.ipynb)
✅ Queries cover traffic attribution, funnel behavior, revenue trends, product profitability, and refund analysis
✅ Used window functions (ROW_NUMBER, running SUM) and CTEs for advanced analysis

📈 Dashboards
1️⃣ Home Page
📌 Landing screen with navigation to all report pages.

2️⃣ Overview Dashboard
📌 Headline KPIs (Revenue, Orders, Conversion Rate, Profit Margin) with year-over-year trends, channel mix, and device/country split.

3️⃣ Sales & Marketing Dashboard
📌 Channel and campaign performance, session-to-order funnel, and revenue targets with drill-down capability.

4️⃣ Product & Geo Dashboard
📌 Product profitability, refund rates, and geographic revenue distribution via an interactive map.

📖 Report Flow
The report walks users through a data-driven story:

1. Landing Overview
2. Business Performance Trends
3. Marketing Channel Effectiveness
4. Product Profitability
5. Geographic Insights & Refund Analysis

🔍 Key Insights
✨ Google Search (gsearch) is the dominant traffic channel, driving ~67% of sessions and revenue
✨ Overall conversion rate stands at 6.83%, generating $1.94M in total revenue and $1.22M in profit
✨ The Original Mr. Fuzzy remains the top-performing product by revenue and profit
✨ Desktop sessions (69%) significantly outperform mobile (31%) in volume
✨ United States contributes ~75% of traffic, with the United Kingdom making up the remaining ~25%
✨ Refunds account for 4.32% of order items, worth $85,338.69 in total

🚀 How to Run
1. Download the .pbix file from this repository.
2. Open it in Power BI Desktop.
3. Navigate through the dashboards using the page tabs and slicers.
4. (Optional) Re-run PYTHON_CLEANING.ipynb and SQL_QUERY.ipynb to regenerate the cleaned data and query outputs from the raw CSVs.

🔮 Future Improvements
🔄 Automate the data refresh pipeline (Python → SQLite → Power BI Service)
📈 Add revenue and conversion-rate forecasting using time-series models
🎯 Integrate real advertising-spend data to calculate true ROAS by channel
🧩 Build customer segmentation (RFM analysis) using session and order history
🗺️ Replace simulated geography with real geolocation data

🏆 Author
👤 Taru Sharma
🎓 BCA, Panipat Institute of Engineering & Technology (PIET)
📧 Contact: [your email here]
🌐 GitHub: [your GitHub profile link here]
