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
<img width="1247" height="696" alt="Star_Schema" src="https://github.com/user-attachments/assets/12e77094-e04d-4b71-b06d-26c0db671c16" />
<br><br>

---

## 📋 Project Tables & Transformations

### Customer Table
<img width="1907" height="966" alt="customer" src="https://github.com/user-attachments/assets/129ec5fa-160c-4dfe-bab8-7738552cfbf5" />
<br><br>

### Vehicle Table
<img width="1917" height="947" alt="Vehicle" src="https://github.com/user-attachments/assets/db9ff1e3-0433-43ce-a159-e7f791784940" />
<br><br>

### Dealer Table
<img width="1917" height="946" alt="Dealer" src="https://github.com/user-attachments/assets/cab5da83-4068-4022-8f9c-694fa45244b3" />
<br><br>


### Car Sales Fact Table
<img width="1917" height="952" alt="car sales" src="https://github.com/user-attachments/assets/59af04dc-fb44-46fc-98d4-d40e934673f3" />
<br><br>

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

### DAX Formulas
<img width="960" height="1093" alt="Gemini_Generated_Image_1f76kj1f76kj1f76" src="https://github.com/user-attachments/assets/18ab886f-16b5-4bdf-95a7-7e791e3bf715" />

<br><br>

---

# 📄 Dashboard Pages

## 1️⃣ Executive Sales Overview
Provides a high-level summary of car sales performance.  
<img width="791" height="648" alt="Executive Sales Overview" src="https://github.com/user-attachments/assets/029f024c-26dd-4902-a560-4f66b0eae3be" />


## 2️⃣ Customer Analytics Dashboard
Focuses on customer demographics, segmentation, and purchasing behavior.  
<img width="1127" height="660" alt="Customer Analysis" src="https://github.com/user-attachments/assets/f7f45559-325a-425d-a25f-a34dfef1cbe1" />


## 3️⃣ Vehicle Performance Dashboard
Evaluates brand-level and model-level performance.  
<img width="977" height="637" alt="Vehicle Performance Analysis" src="https://github.com/user-attachments/assets/fcd9741a-b9b6-497d-8bc8-8b68bde13288" />

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
