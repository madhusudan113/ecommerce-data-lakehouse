# E-Commerce Data Lakehouse Platform

## Project Overview

This project demonstrates the design and implementation of an end-to-end E-Commerce Data Lakehouse using Databricks, PySpark, Delta Lake, Unity Catalog, SQL, and Power BI.

The solution follows the Medallion Architecture (Bronze, Silver, Gold) to ingest, transform, model, and analyze e-commerce data.

---

## Business Problem

An e-commerce company generates data from multiple systems:

* Orders
* Customers
* Products
* Payments

The business requires a scalable analytics platform to monitor revenue, customer behavior, product performance, and payment trends.

---

## Technology Stack

* Databricks Free Edition
* PySpark
* Delta Lake
* Unity Catalog
* SQL
* Power BI
* GitHub

---

## Architecture

CSV Files

→ Bronze Layer (Raw Delta Data)

→ Silver Layer (Cleaned & Validated Data)

→ Gold Layer (Business Data Model)

→ SQL Analytics

→ Power BI Dashboard

---

## Medallion Architecture

### Bronze Layer

Stores raw source data exactly as received.

### Silver Layer

Performs:

* Null handling
* Duplicate removal
* Date standardization

### Gold Layer

Creates business-ready datasets:

* Fact_Sales
* Dim_Customer
* Dim_Product

---

## Data Sources

### Orders

* order_id
* customer_id
* product_id
* quantity
* price
* order_date

### Customers

* customer_id
* name
* city
* state

### Products

* product_id
* product_name
* category

### Payments

* payment_id
* order_id
* payment_method
* amount

---

## Incremental ETL

Implemented Delta Lake MERGE operation to process only new records.

Benefits:

* Reduced processing time
* Reduced compute cost
* Scalable architecture

---

## Data Quality Checks

Implemented:

* Null validation
* Duplicate removal
* Date conversion
* Schema consistency

---

## Data Modeling

Star Schema Design

Fact Table:

* Fact_Sales

Dimension Tables:

* Dim_Customer
* Dim_Product

---

## SQL Analytics

Implemented business queries:

* Top Products
* Revenue by State
* Monthly Revenue Trend
* Top Customers
* Payment Method Analysis

---

## Workflow Automation

Databricks Workflow:

Bronze_Load

↓

Silver_Transform

↓

Gold_Model

↓

Analytics

---

## Dashboard Features

* Total Revenue
* Total Orders
* Total Customers
* Revenue by Category
* Revenue by State
* Monthly Sales Trend
* Top Products
* Payment Method Analysis

---

## Key Skills Demonstrated

* Data Lakehouse
* Medallion Architecture
* ETL Development
* Delta Lake
* Incremental Processing
* Data Quality
* Data Modeling
* SQL Analytics
* Workflow Orchestration
* Power BI Reporting

---

## Future Enhancements

* Auto Loader
* Structured Streaming
* SCD Type 2
* Data Quality Framework
* CI/CD Integration
* Automated Testing
* Monitoring & Alerting

---

## Author

Madhu Sudan

Data Engineer Portfolio Project
