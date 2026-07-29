📊 Super Store Sales Dashboard (Power BI):

📌 Project Overview: This project presents an interactive Sales Dashboard built using Power BI to analyze retail data from a Super Store dataset. The dashboard provides insights into sales performance, profitability, customer segments, and return behavior, helping stakeholders make data-driven decisions.

🎯 Objectives:

-Analyze overall sales and profit performance
-Identify top-performing categories and sub-categories
-Track monthly trends (Year-over-Year)
-Understand customer segment contribution
-Detect patterns in product returns
-Perform geographical analysis of sales and profit

📊 Key KPIs & DAX Formulas:

Total Sales = SUM('SuperStore_Sales_Dataset'[Sales])

Total Profit = SUM('SuperStore_Sales_Dataset'[Profit])

Profit Margin = 
DIVIDE(
    SUM('SuperStore_Sales_Dataset'[Profit]),
    SUM('SuperStore_Sales_Dataset'[Sales])
)

Average Delivery Days = 
AVERAGEX(
    'SuperStore_Sales_Dataset',
    DATEDIFF(
        'SuperStore_Sales_Dataset'[Order Date],
        'SuperStore_Sales_Dataset'[Ship Date],
        DAY
    )
)

Return Rate = 
DIVIDE(
    SUM('SuperStore_Sales_Dataset'[Returns]),
    COUNT('SuperStore_Sales_Dataset'[Order ID])
)


📈 Dashboard Features:

📅 Year-over-Year Analysis for Sales & Profit
🌍 Geographical Map showing Sales and Profit by State
🍩 Segment Analysis using donut chart
📦 Category & Sub-Category Breakdown
🔁 Return Analysis by Category
💳 Payment Mode Distribution
🎛️ Region Filter (Central, East, South, West)

🛠 Tools & Technologies:

-Power BI Desktop
-DAX (Data Analysis Expressions)
-CSV Dataset (Super Store Sales Data)

📸 Dashboard Preview:

<img width="1328" height="746" alt="image" src="https://github.com/user-attachments/assets/c1e6ac96-a74c-442d-b64f-52f59ad4b07c" />


🚀 Future Improvements

Add interactive KPI cards with custom design
Include drill-through and tooltip pages
Implement forecasting for sales trends
Enhance return analysis with deeper segmentation
Optimize dashboard for mobile view

