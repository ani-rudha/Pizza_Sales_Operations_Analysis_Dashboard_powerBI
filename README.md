# 🍕 Pizza Sales & Operational Intelligence Dashboard (*Power BI*)

### ✴️ Project Overview
This project presents an end‑to‑end Pizza Sales & Operational Intelligence Dashboard built using Power BI to analyze product performance, revenue distribution, and kitchen operational efficiency. The objective was to design a clean relational data model, implement robust DAX measures, and deliver executive‑ready insights connecting sales demand with preparation time analysis. The dashboard integrates financial KPIs with operational metrics to simulate a real‑world restaurant performance monitoring system.

### 🎯 Business Objectives
- Measure overall Revenue Performance  
- Identify Top Revenue‑Generating Pizzas  
- Analyze Product Category & Size Contribution  
- Detect Peak Demand Hours  
- Evaluate Average Preparation Time  
- Identify Operational Pressure Windows  
- Design a professional multi‑page interactive dashboard  

### 📂 Dataset Description
The dataset consists of the following tables:

| Table             | Description                                      |
|-------------------|--------------------------------------------------|
| `tab_orders`      | Order‑level data (order_id, date, time)          |
| `tab_order_details` | Line‑level order quantity per pizza             |
| `tab_pizzas`       | Pizza attributes (name, category, size, price)   |
| `tab_operations`   | Kitchen preparation start & end time             |

### 🧱 Data Model Design
The model follows a clean relational (star schema) structure ensuring accurate revenue calculation and clean filter propagation across visuals.

### 🧠 Key DAX Measures Implemented
**Core Sales KPIs:**  
- Total Revenue  
- Total Orders  
- Total Quantity Sold  
- Average Order Value (AOV)  

**Product Intelligence Measures:**  
- Revenue by Category  
- Revenue by Size  
- Top N Revenue Ranking  
- Top N Quantity Ranking  

**Operational Metrics:**  
- Prep Duration (calculated column)  
- Average Prep Time  
- Orders by Hour  
- Revenue by Hour  
- Peak Hour Detection  

**Dynamic UX Measures:**  
- Selected Category = `SELECTEDVALUE(tab_pizzas[pizza_category], "All Categories")`  
- Category‑based conditional formatting  
- Filter‑sensitive KPI calculations  

### 📊 Dashboard Pages
**1. Executive Overview**  
- Total Revenue, Orders, Quantity, AOV  
- Revenue by Category & Size  
- Hourly Order Trend  
*Purpose: High‑level business performance snapshot for management.*

**2. Product Performance**  
- Top 5 Pizzas by Revenue & Quantity  
- Revenue by Category & Size  
- Interactive Category Filtering  
- Dynamic Page Title  
*Purpose: Identify revenue drivers and demand leaders.*

**3. Operational Insights**  
- Orders & Revenue by Hour  
- Average Preparation Time by Hour  
- Peak Demand Identification  
- Kitchen Pressure Analysis  
*Purpose: Connect demand patterns with operational efficiency.*

### ✨ Advanced UX Features
- Multi‑page structured navigation  
- Dynamic page titles using DAX  
- Conditional formatting for category‑based styling  
- Clean executive layout design  
- Export‑safe embedded visuals  
- Balanced visual spacing & consistent formatting  
- Slicer‑based interactive filtering  

### 🔍 Key Business Insights
- Identified peak sales hours and revenue concentration windows.  
- Demand spikes aligned with increased preparation time.  
- High‑volume pizzas not necessarily generating the highest revenue.  
- Size contribution patterns affecting revenue mix.  
- Operational pressure during peak demand periods.

### 💡 Business Recommendations
- Increase staffing during peak hours.  
- Monitor prep time during high‑demand windows.  
- Promote high‑margin pizzas during slower hours.  
- Consider pricing adjustments for top‑performing sizes.  
- Use hourly analysis to optimize production planning.

### ✅ KPI Integrity Validation
- Cross‑validated revenue = price × quantity  
- Verified relationship direction for correct filter propagation  
- Confirmed hour‑based aggregation consistency  
- Tested category filtering impact across pages  
- Validated prep time logic using row‑level calculations  
- Ensured no circular dependencies in model  

### 🛠️ Tools Used
- Power BI Desktop  
- DAX (Advanced Filter Context Handling)  
- Data Modeling (Star Schema Principles)  
- Power Query (ETL & Data Type Correction)  
- Relational Data Modeling  
- CSV data sources  

### 📌 Portfolio Value
This project demonstrates:
- End‑to‑end BI development  
- Strong relational data modeling  
- Practical DAX implementation  
- Operational analytics integration  
- Business KPI design thinking  
- Dashboard UX optimization  
- Debugging and data‑type correction skills  

It reflects the ability to move beyond basic revenue reporting and deliver integrated financial and operational intelligence.

—

*For any questions or collaboration opportunities, feel free to reach out!*
