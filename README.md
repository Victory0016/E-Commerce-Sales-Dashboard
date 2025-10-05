# 📊 E-Commerce Sales Dashboard

## 📌 Table of Contents
- [Introduction](#introduction)  
- [Dashboard Overview](#dashboard-overview)  
- [Business Problem](#business-problem)  
- [Objectives](#objectives)  
- [Tools & Technologies Used](#tools--technologies-used)  
- [Wireframing & Design Planning](#wireframing--design-planning)  
- [Data Preparation & Cleaning (Power Query Editor)](#data-preparation--cleaning-power-query-editor)  
- [Data Modeling (Power Pivot & Relationships)](#data-modeling-power-pivot--relationships)  
- [KPI Calculations (DAX Measures)](#kpi-calculations-dax-measures)  
- [Pivot Table Analysis](#pivot-table-analysis)  
- [Detailed Insights](#detailed-insights)  
- [Profitability Recommendations](#profitability-recommendations)  
- [Conclusion](#conclusion)  


---

## Introduction

The E-Commerce industry generates vast amounts of data across transactions, customers, suppliers, and stores. To remain competitive, businesses need to track key performance indicators (KPIs), understand customer behavior, and identify growth opportunities.

This project demonstrates how I built a **comprehensive E-Commerce Sales Dashboard in Excel** using **Power Query, Power Pivot, Pivot Tables, and DAX Measures**. The dashboard helps stakeholders monitor performance, improve profitability, and make data-driven decisions.

---

##  Dashboard Overview

The dashboard delivers a view of sales performance by consolidating multiple datasets into an interactive report. It highlights:
  <img width="1353" height="684" alt="Screenshot 2025-10-05 182528" src="https://github.com/user-attachments/assets/9f3e4b1e-9ca7-453f-8ef0-e0bb98953c87" />
  <img width="1342" height="685" alt="Screenshot 2025-10-05 182830" src="https://github.com/user-attachments/assets/a3747abf-53ec-41b8-b386-b937a32df924" />


---

##  Business Problem

The company had fragmented sales data across multiple dimensions (fact tables, product details, stores, customers, time, and transactions). Without a consolidated system, management lacked visibility into:
- Which products or categories drive the most profit.
- Which suppliers and stores perform best.
- Customer purchasing behavior and retention.
- Year-over-year growth trends for revenue and quantity.

---

##  Objectives

- Integrate multiple datasets into a clean, unified model.  
- Automate data transformation using **Power Query**.  
- Build relationships between fact and dimension tables.  
- Create **KPI measures** to evaluate performance.  
- Provide a clear **dashboard for decision-making**.  
- Recommend strategies for **profitability and growth**.  

---

## Tools & Technologies Used

- **Microsoft Excel**  
   - Power Query Editor (data preparation)  
   - Power Pivot (data modeling & measures)  
   - Pivot Tables & Pivot Charts  
   - DAX Measures  
- **PowerPoint** – for dashboard wireframing  

---

##  Wireframing & Design Planning

Before building the dashboard, I designed a **wireframe in PowerPoint** to map out:
- Placement of KPIs at the top (Revenue, Quantity, Customers).  
- Visuals for trends (line charts), comparisons (bar charts), and breakdowns (donut charts).  
- Sections for **Products, Customers, Geography, and Suppliers**.
 <img width="1199" height="645" alt="Screenshot 2025-09-26 145932" src="https://github.com/user-attachments/assets/c954b80d-c0d1-4849-add6-38114772666e" />
 <img width="1198" height="666" alt="Screenshot 2025-09-26 150053" src="https://github.com/user-attachments/assets/4b78cdea-dd94-4750-9da8-1e7978d1371a" />

This step ensured a logical layout and client-focused storytelling.

---

##  Data Preparation & Cleaning (Power Query Editor)

Steps taken to clean and prepare the data:
1. Imported datasets: **Fact Table, Item Dimension, Store Dimension, Time Dimension, Transaction Dimension, Customer Dimension**.  
2. Replaced all lowercase words with **Proper Case** for readability.  
3. Promoted the **first row to headers**.  
4. Extracted **Month Name** from the Date column.  
5. Added a **Blank Query** to store calculated measures.  
6. Due to the large dataset, selected **Close & Load To → Data Model** (instead of worksheets).  

---

##  Data Modeling (Power Pivot & Relationships)

- Opened **Power Pivot → Manage** to build relationships.  
- Linked the **Fact Table** to dimension tables (Star Schema).  
- Ensured proper joins (e.g., DateID, CustomerID, ProductID).  
- This allowed cross-analysis (e.g., sales by store, customer, or region).
- <img width="1916" height="979" alt="Screenshot 2025-09-26 142817" src="https://github.com/user-attachments/assets/ea3af921-13f7-4b72-b757-061edecef245" />
  
---

##  KPI Calculations (DAX Measures)

I created the following **DAX measures** in the Blank Query:

**Core KPIs:**
- Total Sales 
- Total Quantity
- Average Unit Price  
- Total Customers
- Previous Year Sales  
- Previous Year Quantity  
- Previous Year Avg. Unit Price  
- Previous Year Customers  
- YoY Sales Growth (%)  
- YoY Quantity Growth (%)  
- YoY Avg. Unit Price Growth (%)  
- YoY Customer Growth (%)  

All YoY measures were **formatted as percentages** using **Custom Formatting** for clarity.

---

##  Pivot Table Analysis

Two additional Pivot Tables were created for deeper analysis:
1. **Product & Category Analysis** – Identifying top-performing products and categories by revenue.  
2. **Customer & Supplier Analysis** – Ranking top customers and suppliers by contribution.  
 <img width="1908" height="855" alt="Screenshot 2025-09-25 195114" src="https://github.com/user-attachments/assets/36e91fa6-3e30-43f1-82a4-8eeebf7d6d34" />
 <img width="1913" height="859" alt="Screenshot 2025-09-25 195150" src="https://github.com/user-attachments/assets/2bd95b8e-805c-4309-b880-c65dcf560ad7" />
 <img width="1919" height="861" alt="Screenshot 2025-09-25 195254" src="https://github.com/user-attachments/assets/541a9024-2c67-4009-b0e0-f42d8e08df2a" />

---

##  Detailed Insights

Key findings from the dashboard:
- Total revenue reached **$105M across 6M units**.  
- **Energy beverages and healthy food categories** drive the highest sales.  
- **Ningbo Seduno** and **Indo Count Industries** are leading suppliers.  
- **Bangladesh and India** contribute the most to revenue.  
- **Card transactions dominate (90%)**, while mobile payments are underutilized (2%).  
- Seasonal peaks occur **March–July**, indicating potential for targeted promotions.  

---

## Profitability Recommendations

1. **Promote Mobile Payments** – Introduce discounts to increase adoption, reducing transaction costs.  
2. **Expand High-Demand Categories** – Focus on beverages and health-related products.  
3. **Supplier Optimization** – Strengthen contracts with top suppliers to secure better margins.  
4. **Regional Growth** – Target underperforming regions with localized offers and campaigns.  
5. **Customer Retention Programs** – Offer loyalty rewards to high-value customers.  
6. **Store Optimization** – Invest in top-performing stores and evaluate weaker ones for restructuring.  

---

##  Conclusion

This project demonstrates how **Excel (Power Query + Power Pivot + Pivot Tables)** can transform raw, disconnected datasets into a **powerful dashboard for profitability and growth strategies**.



