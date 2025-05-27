**📊 Project Title:**
**End-to-End Sales Analytics Dashboard Using Power BI.**

An end-to-end Power BI project analyzing company sales, customer, and product data from 2023 to 2025. The goal of this project was to uncover trends in revenue, product performance, customer behavior, and geographic sales—providing data-driven insights for business decision-making and strategic planning.

This project demonstrates the complete data analysis process using Power BI only, from importing raw Excel/CSV files, transforming and modeling data using Power Query, and creating insightful visualizations using DAX and interactive dashboard features.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🎯 Objective:**

To build an interactive Power BI dashboard that helps stakeholders:

Monitor sales performance and revenue trends

Identify top-performing products and underperforming categories

Analyze customer segmentation and purchasing behavior

Track geographic sales to identify expansion opportunities


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧰 Tools Used:**

**Power BI:**	Data transformation, modeling, visualization
**Power Query:**	Cleaning and transforming raw datasets
**DAX:**	Creating custom KPIs and measures
**Excel/CSV:**	Raw data files used for import

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**📋 Key Performance Indicators (KPIs)**

**1. For Transaction Performance:** Net Sales, Total Quantity,Net Avg Order Value.

**2. For Customer Purchase Behavour:**  Total Customers, Single Order Customers, Repeat Customers 

**3. For Retension & Value KPI's:**  Lifetime Value, Repeate Rate, Purchase Frequency.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧼 Data Transformation (Power Query)**

Removed duplicates and blank rows

Changed data types (e.g., dates, numbers)

Merge columns (e.g., first/last names into full name )

Created calculated columns (e.g., Total Quantity, Net Sales)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧠 DAX Measures:**

**For Transaction Performance:**
Net Sales = SUM(Subtotal Price)
Total Quantity = SUM(Quantity)
Net Avg Order Value = AVERAGE(Subtotal Price)

**For Customer Purchase Behavour:**
Total Customers = DISTINCTCOUNT(Customer Id)
Single Order Customers = CALCULATE(COUNTROWS(VALUES(Customer Id)), FILTER(VALUES(Customer I), CALCULATE(DISTINCTCOUNT(Order Number)) = 1 ))
Repeat Customers = CALCULATE(COUNTROWS(VALUES(Customer Id)), FILTER(VALUES(Customer Id), CALCULATE(DISTINCTCOUNT(Order Number)) > 1 ))

**For Retension & Value KPI's:**
Lifetime Value = [Net Sales] / [Total Customers]
Repeate Rate = [Repeat Customers] / [Total Customers]
Purchase Frequency = DISTINCTCOUNT(Order Number) / [Total Customers]

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🎛️ Filters and Slicers in the Dashboard:**

Select Measure : For Net Sales, Total Quantity, Total Customers and Repeat Customers.

Payment Gateways.

Region

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**📈 Dashboard Features:**

Line charts: Net Sales, Total Quantity, Total Customers and Repeat Customers Trend Over Time.

Bar charts: City, Product type and Hours Overview by Net Sales, Total Quantity, Total Customers and Repeat Customers.

Map visualization: Regional overview by Address and Location breakdown by Net Sales, Total Quantity, Total Customers and Repeat Customers

Donut/pie charts: Net Sales, Total Quantity, Total Customers and Repeat Customers by Gateway Payment Method

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🔍 Key Insights:**

📊 Revenue grew steadily year-over-year, with a notable spike during Q4 promotions.

🏆 Technology and Electronics categories generated the most revenue and profit.

📉 Office Supplies underperformed consistently and had the lowest margin.

🌍 The West and South regions showed the fastest growth, ideal for expansion.

🧑‍💼 Corporate clients made fewer purchases but had a significantly higher average order value than retail customers.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**✅ Outcome:**

This dashboard enables stakeholders to:

Identify top and bottom-performing products

Allocate inventory and marketing budgets efficiently

Monitor business health via dynamic KPIs

Make informed decisions based on visual data stories
