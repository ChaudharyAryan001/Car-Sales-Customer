# 📊 Car Sales & Customer Intelligence Dashboard

## 🎯 Project Overview
The Car Sales & Customer Intelligence Dashboard is an end-to-end Power BI project designed to transform raw car sales and customer data into actionable business insights.

This project demonstrates the complete Business Intelligence workflow, including:
- Data Cleaning & Transformation using Power Query
- Star Schema Data Modeling
- Relationship Management
- DAX Measures & Calculated Columns
- Time Intelligence Analysis
- Customer Segmentation
- Vehicle Performance Analysis
- Dealer Contribution Analysis
- Interactive Dashboard Design

---

## 🛠 Tools & Technologies Used
- Power BI Desktop  
- Power Query  
- DAX (Data Analysis Expressions)  
- Star Schema Modeling  
- Data Visualization  
- Time Intelligence Functions  

---

## 📂 Data Model Architecture
A Star Schema model was implemented to improve performance and simplify analytical reporting.

### Fact Tables
- **Fact_CarSales**

### Dimension Tables
- **Dim_Customer**
- **Dim_Vehicle**
- **Dim_Dealer**
- **Dim_Date**

---

## ⭐ Star Schema Design
The data model follows a centralized fact table structure connected to multiple dimension tables.

### Model Benefits
- Faster query performance  
- Better scalability  
- Simplified relationships  
- Efficient DAX calculations  

### Screenshot
![Star Schema](images/star_schema.png)

---

## 📋 Project Tables & Transformations

### Customer Table
![Customer Table](images/dim_customer.png)

### Vehicle Table
![Vehicle Table](images/dim_vehicle.png)

### Dealer Table
![Dealer Table](images/dim_dealer.png)

### Date Table
![Date Table](images/dim_date.png)

### Car Sales Fact Table
![Car Sales Fact](images/fact_carsales.png)

---

```

## 📈 DAX Calculations Implemented

### Measures
- Total Sales = SUM(Fact_CarSales[Sales_Amount])  
- Cars Sold = COUNT(Fact_CarSales[Car_id])  
- Average Selling Price = AVERAGE(Fact_CarSales[Sales_Amount])  
- Total Customers = DISTINCTCOUNT(Fact_CarSales[Customer_key])  
- Total Dealers = DISTINCTCOUNT(Fact_CarSales[Dealer_Key])  
- Revenue Per Customer = DIVIDE([Total Sales],[Total Customers])  
- Revenue Per Dealer = DIVIDE([Total Sales],[Total Dealers])  
- Average Sales Per Day = DIVIDE([Total Sales],DISTINCTCOUNT(Dim_Date[Date]))  
- Highest Sale = MAX(Fact_CarSales[Sales_Amount])  
- Lowest Sale = MIN(Fact_CarSales[Sales_Amount])  
- Average Cars Sold Per Dealer = DIVIDE([Cars Sold],[Total Dealers])  
- Average Customer Income = AVERAGE(Dim_Customer[Annual Income])  

### Filter Context Functions
- Regional % Sales  
- Market Share %  
- Sales Vs Avg Sale  
- Running Total Sales  

### Time Intelligence Functions
- Sales YTD = TOTALYTD([Total Sales],Dim_Date[Date])  
- Sales QTD = TOTALQTD([Total Sales],Dim_Date[Date])  
- Sales MTD = TOTALMTD([Total Sales], Dim_Date[Date])  

### Calculated Columns
- Month Number  
- Year  
- Month Name  
- Quarter  
- Vehicle Category  
- Income Group  

```

### Screenshot
![DAX Formulas](images/dax_formulas.png)

---

# 📄 Dashboard Pages

## 1️⃣ Executive Sales Overview
Provides a high-level summary of car sales performance.  
![Executive Overview](images/executive_sales.png)

## 2️⃣ Customer Analytics Dashboard
Focuses on customer demographics, segmentation, and purchasing behavior.  
![Customer Analysis](images/customer_analysis.png)

## 3️⃣ Vehicle Performance Dashboard
Evaluates brand-level and model-level performance.  
![Vehicle Performance](images/vehicle_performance.png)

## 4️⃣ Dealer Contribution Dashboard
Analyzes dealer-wise sales contribution and regional performance.  
![Dealer Dashboard](images/dealer_dashboard.png)

---

## 🔍 Key Insights Generated
- Generated total sales of **671M+** across all transactions.  
- Cars Sold: **24K** with an average selling price of **28K**.  
- Top performing brands: **Chevrolet, Ford, Dodge, Mercedes-Benz**.  
- SUVs and Hatchbacks contributed the highest revenue share.  
- Q4 was the strongest sales period with **248M revenue**.  
- Identified top revenue-generating customers and dealers.  
- Tracked return reasons and quality-related issues.  
- Applied Time Intelligence functions for performance tracking.  

---

## 🚀 Skills Demonstrated
- **Power Query** → Data Cleaning, Transformation, Preparation  
- **Data Modeling** → Star Schema, Relationship Management  
- **DAX** → Measures, Calculated Columns, Time Intelligence  
- **Visualization** → KPI Cards, Donut Charts, Treemaps, Waterfall Charts, Decomposition Trees  
- **Business Intelligence** → Customer Analytics, Vehicle Analytics, Dealer Monitoring, Sales Analysis  

---

## 📌 Project Outcome
This dashboard transforms raw car sales data into meaningful business intelligence, enabling data-driven decision making through interactive reporting, advanced DAX calculations, and professional dashboard design.
