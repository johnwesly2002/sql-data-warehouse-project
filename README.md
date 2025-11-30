# 📦 SQL Data Warehouse Project  
Building a modern data warehouse with SQL Server using **Bronze, Silver, Gold** architecture, ETL pipelines, data modeling, and analytics.

---

## 📘 Table of Contents
- [Introduction](#introduction)
- [Architecture (Bronze–Silver–Gold)](#architecture-bronze–silver–gold)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [MIT License](#mit-license)

---

## 📖 Introduction  
This project demonstrates how to design a modern **SQL-based Data Warehouse** using the industry-standard **Bronze → Silver → Gold** layered architecture.

It covers:

- ETL using SQL/T-SQL  
- Bronze: Raw ingestion  
- Silver: Clean, validated, business-ready data  
- Gold: Star schema models for analytics  
- Fact & dimension modeling  
- Analytics-ready tables  

---

## 🏗 Architecture (Bronze–Silver–Gold)

### 🟫 **Bronze Layer – Raw Data**
- Stores raw ingested data exactly as received  
- Used for lineage, auditing, and reprocessing  
- Minimal or no transformations  
- Data sources: CSV, Excel, APIs, OLTP dumps  

### ⚪ **Silver Layer – Cleansed & Standardized Data**
- Deduplicated and validated data  
- Schema alignment  
- Handling nulls, type conversions  
- Join preparation & basic business logic  
- Data quality checks implemented here  

### 🟡 **Gold Layer – Analytics & Star Schema**
- Fact & Dimension tables  
- Designed for reporting and dashboards  
- SCD (Slowly Changing Dimensions) supported  
- Aggregated marts for business users  
- Optimized indexing & query performance  

---

## ⭐ Features
- ✔ Bronze/Silver/Gold layered warehouse  
- ✔ SQL-based ETL pipelines  
- ✔ Data quality & validation rules  
- ✔ Star schema models for BI tools  
- ✔ Fact & Dimension tables  
- ✔ Incremental load strategy  
- ✔ Audit logging framework  
- ✔ Analytics-ready datasets  

---

## 🛠 Tech Stack

| Component | Usage |
|----------|--------|
| **SQL Server** | Core data warehouse engine |
| **T-SQL** | ETL, transformations, business logic |
| **SSMS / Azure Data Studio** | Database development |
| **SSIS / ADF (optional)** | ETL orchestration |
| **Power BI** (optional) | Analytics & dashboards |

---

## 🔄 ETL Workflow

### **1. Extract → Bronze**
- Data loaded directly into **Bronze tables**  
- Preserves raw format  
- Metadata and audit logs registered  

### **2. Transform → Silver**
- Clean & standardized data  
- Remove duplicates  
- Validate relationships  
- Enforce schema consistency  
- Apply first-level business rules  

### **3. Load → Gold**
- Build **Dimension tables (DimCustomer, DimProduct...)**  
- Build **Fact tables (FactSales, FactOrders...)**  
- Create aggregated marts for BI layers  
- Implement SCD Type-1/Type-2 dimensions  

---

MIT License

Copyright (c) 2025
