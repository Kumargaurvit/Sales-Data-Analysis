# 📝 Project Title
Sales Data Analysis Dashboard - Superstore Sales Insights

# 🎯 Project Statement
This project aims to analyze and visualize sales data from a Superstore using PowerBI. It provides an interactive dashboard that offers critical insights into various performance metrics such as revenue, profit, customer segments and regional trends to support data-driven decision-making

# 🎯 Objective
- To identify sales and profit trends over time
- To understand customer behaviour across regions and segments
- To identify top-performing products and categories
- To forecast future sales and profits based on historical trends

# 🧰 Tech Stack Used
- Power BI - For data Visualization and dashboard creation
- Power Query (M) - For Data Cleaning and Transformation
- DAX (Data Analysis Expressions - For calculated measures and KPIs
- Excel/Csv - For Data Storage

# 🧰 Key DAX Measures
- Average Orders = Average Orders = VAR Orders2020 = CALCULATETABLE(VALUES('SuperStore_Sales_Dataset'[Order ID]),YEAR('SuperStore_Sales_Dataset'[Order Date]) = 2020)
                                    VAR Months2020 = CALCULATE(DISTINCTCOUNT('SuperStore_Sales_Dataset'[Month]),YEAR('SuperStore_Sales_Dataset'[Order Date]) = 2020)
                                    RETURN
                                    DIVIDE(COUNTROWS(Orders2020), Months2020)
