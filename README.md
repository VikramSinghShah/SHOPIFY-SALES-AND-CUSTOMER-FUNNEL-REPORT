**📊 Project Title:**

**SHOPIFY | SALES AND CUSTOMER FUNNEL REPORT**

An end-to-end Power BI project analyzing company sales, customer, and product data from 2023 to 2025. The goal of this project was to uncover trends in revenue, product performance, customer behavior, and geographic sales—providing data-driven insights for business decision-making and strategic planning.

This project demonstrates the complete data analysis process using Power BI only, from importing raw Excel/CSV files, transforming and modeling data using Power Query, and creating insightful visualizations using DAX and interactive dashboard features.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🎯 Objective:**

To build an interactive Power BI dashboard that helps stakeholders:

Monitor Transaction performance, Customer Purchase Behavoiur and Repeated and Single order Customers.

Identify Repeat Customer and Net Sales and Life time value of A customer.

Analyze customer segmentation and purchasing behavior

Track geographic Net Sales, Total Quantity, Total Customers and Repeat Customers  to identify expansion opportunities.


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

1. Net Sales = SUM(Subtotal Price)

2. Total Quantity = SUM(Quantity)

3. Net Avg Order Value = AVERAGE(Subtotal Price)


**For Customer Purchase Behavour:**

1. Total Customers = DISTINCTCOUNT(Customer Id)

2. Single Order Customers = CALCULATE(COUNTROWS(VALUES(Customer Id)), FILTER(VALUES(Customer I), CALCULATE(DISTINCTCOUNT(Order Number)) = 1 ))

3. Repeat Customers = CALCULATE(COUNTROWS(VALUES(Customer Id)), FILTER(VALUES(Customer Id), CALCULATE(DISTINCTCOUNT(Order Number)) > 1 ))



**For Retension & Value KPI's:**

1. Lifetime Value = [Net Sales] / [Total Customers]

2. Repeate Rate = [Repeat Customers] / [Total Customers]

3. Purchase Frequency = DISTINCTCOUNT(Order Number) / [Total Customers]


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🎛️ Filters and Slicers in the Dashboard:**

Select Measure : For Net Sales, Total Quantity, Total Customers and Repeat Customers.

Payment Gateways.

Region

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**📈 Dashboard Features:**

**Line charts:** Net Sales, Total Quantity, Total Customers and Repeat Customers Trend Over Time.

**Bar charts:** City, Product type and Hours Overview by Net Sales, Total Quantity, Total Customers and Repeat Customers.

**Map visualization:** Regional overview by Address and Location breakdown by Net Sales, Total Quantity, Total Customers and Repeat Customers

**Donut/pie charts:** Net Sales, Total Quantity, Total Customers and Repeat Customers by Gateway Payment Method


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**✅ Outcome:**

This dashboard enables stakeholders to:

Identify Net sales ,Total Quantity, and Net Average Order Value and getting the Repeated Customer.

Monitor business health and  customer Purchase Behavour via dynamic KPIs

Make informed decisions based on visual data stories.
