# 📦 Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository!
This project demonstrates a comprehensive data warehousing and analytics solution, from build using built using **SQL Server**, designed to demonstrate industry best practices in **data engineering** and **data analytics**. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

---

## 📌 Project Requirements

### 🏗️ Building the Data Warehouse (Data Engineering)

#### 🎯 Objective

Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### 📚 Specifications

* **Data Sources**: ERP & CRM datasets provided as CSV files
* **Data Quality**: Clean and resolve inconsistencies
* **Integration**: Merge sources into a single analytical model
* **Scope**: Use the latest dataset only (no historization needed)
* **Documentation**: Clear data model documentation for business and analytics teams

---

### 📊 BI: Analytics & Reporting (Data Analytics)

#### 🎯 Objective
Deliver meaningful insights using SQL-based analytics covering:

* **Customer Behavior**
* **Product Performance**
* **Sales Trends**

Insights enable data-driven decision-making at all business levels.

---
# 🏗️ Project Architecture
```
Source Systems (ERP + CRM CSV Files)
              │
              ▼
      Data Ingestion Layer
              │
              ▼
      Data Quality & Cleaning
              │
              ▼
      SQL Server Data Warehouse
      ├── Bronze Layer (Raw)
      ├── Silver Layer (Cleaned)
      └── Gold Layer (Analytics)
              │
              ▼
      BI & Analytics (SQL Queries)
```

---

# 🗂️ Repository Structure

```
📁 Project-Root
│
├── 📁 01_Data
│   ├── ERP.csv
│   ├── CRM.csv
│
├── 📁 02_Notebooks
│   ├── Data_Cleaning.sql
│   ├── Integration.sql
│   ├── Analytics.sql
│
├── 📁 03_Documentation
│   ├── data_model.md
│   ├── ERD.png
│   ├── project_plan.md
│
├── 📁 04_Scripts
│   ├── create_tables.sql
│   ├── transformations.sql
│
└── README.md
```

---

# 🧱 Data Warehouse Layers

### 🟫 **Bronze Layer (Raw Data)**

* Holds unmodified ERP & CRM data
* Used for traceability and validation

### 🪙 **Silver Layer (Cleaned & Standardized)**

* Data quality fixes applied
* Standardized formats (dates, IDs, naming)
* Deduplicated records

### 🥇 **Gold Layer (Analytics Ready)**

* Final star-schema / dimensional model
* Optimized for BI and reporting
* Includes calculated fields & business metrics

---

# 📐 Data Model Overview

**Dimensions**

* `dim_customer`
* `dim_product`
* `dim_date`
* `dim_sales_rep`

**Fact Table**

* `fact_sales`

**Key Features**

* Surrogate keys
* Cleaned customer/product IDs
* Conformed dimensions across ERP & CRM

---

# 📊 Analytics Deliverables

### Key Insights Produced:

✔️ Top-selling products
✔️ Customer purchase frequency
✔️ Monthly/Yearly sales trends
✔️ Sales performance by region
✔️ Customer segmentation opportunities

Each deliverable is backed by optimized SQL queries included in the repository.

---

# 🚀 How to Run the Project

### **Prerequisites**

* SQL Server (Express, Developer, or Azure SQL)
* SQL Server Management Studio (SSMS)

### **Steps**

1. Clone the repository
2. Create a new SQL Server database
3. Run the scripts in `04_Scripts/`
4. Import ERP & CRM CSV files into the Bronze tables
5. Execute transformation scripts
6. Run analytical SQL queries

---

# 📄 Documentation

Full documentation is provided in the `/03_Documentation` folder, including:

* Data model explanation
* Entity-relationship diagram
* Naming conventions
* Project plan & workflow

---

# 🏁 Conclusion
This project showcases:
* End-to-end data engineering
* Best practices in data modeling
* Hands-on analytics using SQL
* Portfolio-ready documentation
* 
---

## 🛡️ License
This project is licensed under the **[MIT License](LICENSE)**. You are free to use, modify, and share this project with proper attribution.

## 🌟 About Me
Hi there! I'm **Chameera Niroshan Perera**., an enthusiastic Data Engineer with a passion for turning data into powerful insights. I enjoy sharing what I learn, breaking down technical topics into simple and engaging content, and showcasing practical data engineering projects that highlight real-world expertise.


