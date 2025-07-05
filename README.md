📊 Atliq Sales Insights: Sales Data Analysis Dashboard
🛠️ Overview
A Power BI dashboard project analyzing Atliq’s sales data (using dataset from Codebasics YouTube channel).
Designed to provide clear, actionable insights for decision-makers in a visually appealing and structured manner.

🎯 Objective
To enhance sales growth by:

Identifying high and low revenue customers & markets.

Analyzing sales trends over time.

Supporting data-driven decisions for product distribution, pricing, and customer management.

🚀 Key Features
✅ Revenue Analysis

Revenue by Zone

Revenue by Market

Revenue Trend over time

Last 5 Years Revenue (Overall and by Zone)

Revenue Growth Products (by Zone, Market, Customer)

✅ Sales Quantity Analysis

Sales Quantity by Zone

Sales Quantity by Market

✅ Customer Insights

Top 5 Customers by Revenue

Identify High Revenue Generating Customers

Identify Less Revenue Generating Customers

✅ Product Insights

Top 5 Products by Revenue

Return Product Quantity by Zone & Customer

✅ Market Insights

Identify Low Sales Markets

✅ Sales Growth Analysis

Monthly Sales Growth vs Previous Years

🧮 Key DAX Measures Used
Revenue = SUM('Sales transactions'[norm_sales_amount])

Revenue LY = CALCULATE([Revenue], SAMEPERIODLASTYEAR('sales date'[date]))

Revenue Contribution % = DIVIDE([Revenue], CALCULATE([Revenue], ALL('sales products'), ALL('sales customers'), ALL('sales markets')))

Sales Qty = SUM('sales transactions'[sales_qty])

Total Profit Margin = SUM('Sales transactions'[Profit_Margin])

Profit Margin % = DIVIDE([Total Profit Margin], [Revenue], 0)

Profit Margin Contribution % = DIVIDE([Total Profit Margin], CALCULATE([Total Profit Margin], ALL('sales products'), ALL('sales customers'), ALL('sales markets')))

💡 Insights Enabled
✅ Optimize inventory & distribution using monthly growth trends.
✅ Target low-sales markets for improvement.
✅ Leverage top customers and products for focused sales strategies.
✅ Improve pricing strategies using customer contribution analysis.

📂 Tools Used
Power BI (Data Modeling, DAX, Dashboard Building)

Sample dataset from Codebasics YouTube Sales Analysis Project

