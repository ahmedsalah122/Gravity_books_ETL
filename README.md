# Gravity Books Data Warehouse

## Overview

**Gravity Books Data Warehouse** is an end-to-end Business Intelligence project designed to build a complete Data Warehouse solution for analyzing book sales, customers, shipping methods, and historical transactions.

This project was implemented using the Microsoft BI Stack:

- SQL Server
- SSIS (ETL)
- SSAS (Analysis)


---

## Project Objectives

- Build a scalable Data Warehouse for Gravity Books database
- Design Snowflake Schema
- Create ETL pipelines using SSIS
- Apply Slowly Changing Dimensions (SCD)
- Build OLAP Cube using SSAS

---

# Data Warehouse Schema

This project uses a **Snowflake Schema** to normalize dimensions and improve scalability.

## Fact Tables:

- Fact_Sales
- Fact_History

## Dimension Tables:

- Dim_Book
- Dim_Customer
- Dim_Author
- Dim_Address
- Dim_ShippingMethod
- Dim_Status
- Dim_Date
- Dim_Time

---

# Technologies Used

| Tool | Purpose |
|------|---------|
| SQL Server | Database Engine |
| SSMS | SQL Development |
| SSIS | ETL Pipelines |
| SSAS | Cube Analysis |
| Power BI | Dashboarding |
| Tableau | Data Visualization |

---

# ETL Process (SSIS)

The ETL flow includes:

## Extract:

Data extracted from source OLTP database.

## Transform:

- Data Cleansing
- Data Type Conversion
- Lookup Transformations
- SCD Type 1 / Type 2
- Derived Columns

## Load:

Load data into Dimensions then Fact Tables.

---

# SSIS Packages

- Dim_Book.dtsx
- Dim_Customer.dtsx
- Dim_ShippingMethod.dtsx
- Fact_Sales.dtsx
- Fact_History.dtsx

---

# SSAS Analysis

Multidimensional Cube created for analyzing:

- Sales by Year
- Sales by Quarter
- Orders by Shipping Method
- Revenue by Publisher
- Price by Customer

---



# SQL Scripts

Located inside:

```text
Queries/
Backups/
