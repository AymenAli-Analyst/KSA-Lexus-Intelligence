# 🏎️ LexusMatrix-BI: KSA Lexus Sales Analytics

[![Database: SQL Server](https://img.shields.io/badge/Database-SQL_Server-red.svg)](https://www.microsoft.com/en-us/sql-server)
[![Data Pipeline: Excel](https://img.shields.io/badge/Pipeline-Excel_ETL-green.svg)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![BI Tool: Power BI](https://img.shields.io/badge/BI_Tool-Power_BI-yellow.svg)](https://powerbi.microsoft.com/en-us/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

> **LexusMatrix-BI:** An interactive KSA Lexus sales analytics solution. Built an end-to-end data pipeline using Excel for data cleaning, SQL Server for data warehousing/heavy relational aggregations, and Power BI with advanced DAX to deliver interactive dashboards tracking 3bn SAR revenue, logistics bottlenecks, and credit risks across 11 cities.

---

## 🎯 Project Objectives & Business Goals
* **Logistics Optimization:** Identify and diagnose the correlation between high sales volume and shipping latency (`Avg_Days_To_Deliver`) to eliminate delivery delays.
* **Geographical Revenue Tracking:** Pinpoint top-performing economic regions (Jeddah, Riyadh) and deploy targeted data-driven strategies for underperforming cities.
* **Financial Risk Mitigation:** Analyze consumer payment methods to manage credit exposure and optimize cash flow stability.

---

## 🛠️ Tech Stack & Technical Architecture
This repository showcases a complete, end-to-end data engineering and business intelligence pipeline divided into three specialized phases:

1. **Excel (Data Cleaning & Preliminary ETL):**
   * Handled raw transactional inputs and vehicle telemetry logs.
   * Executed structural normalization, resolved missing data anomalies, and standardized regional names across Saudi Arabia.
2. **SQL Server (Data Warehousing & Aggregation):**
   * Migrated cleaned datasets into structured relational database tables.
   * Developed advanced SQL scripts using multi-table joins, indexing, and window functions to compute core KPIs (e.g., Net Revenue of 3bn SAR, 23% Sales Growth, and dynamic VAT calculations).
3. **Power BI (Visual Intelligence & Analytics):**
   * Connected directly to optimized SQL Server views.
   * Authored customized **DAX** expressions to calculate dynamic time-intelligence measures and interactive business metrics.

---

## 📊 Business Insights & Diagnostic Solutions

| Identified Issue | Data Metric | Technical / Strategic Solution Implemented |
| :--- | :--- | :--- |
| **High Shipping Latency** | Delivery averages **22-24 days** across major hubs. | Integrated real-time logistics tracking and dynamic inventory re-routing logic. |
| **Regional Sales Disparity** | Jeddah/Riyadh exceed **0.51bn SAR** while Abha logs **0.22bn SAR**. | Shifted flexible vehicle allocation and introduced localized promotional campaigns. |
| **High Credit Risk Exposure** | **23.81%** of purchases rely heavily on In-House Financing. | Proposed a predictive Machine Learning Credit Scoring model to pre-screen customer reliability. |

---

## 📂 Repository Structure
```text
├── data/                    # Cleaned dataset files processed via Excel
├── sql_queries/             # SQL scripts for transformations, schema creation, and aggregation
├── powerbi_dashboard/       # Interactive Power BI workbook file (.pbix)
└── README.md                # Project documentation and executive summar
