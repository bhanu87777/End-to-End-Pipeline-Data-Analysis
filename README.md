<h1>Data Warehouse and Analytics Project</h1>

## 📘 Welcome

**Data Warehouse and Analytics Project** — a comprehensive portfolio project showcasing a modern data warehousing and analytics solution. This repository demonstrates how to ingest, transform, model, and analyze data using a layered Medallion Architecture, producing business-ready datasets and SQL-driven insights. Designed for data engineers, analysts, and architects, the project highlights industry best practices and end-to-end workflows for reliable, reproducible analytics.

---

## 🏗️ Data Architecture

- **Bronze Layer:** Stores raw data ingested from source systems as-is. In this project, raw CSV files from ERP and CRM systems are loaded into a SQL Server database to preserve original data and provenance.
- **Silver Layer:** Contains cleansed, standardized, and normalized data. Transformations at this stage address data quality issues, deduplication, and schema harmonization to prepare data for modeling.
- **Gold Layer:** Houses business-ready datasets modeled into a star schema (fact and dimension tables) optimized for reporting, analytics, and BI consumption.

  <div style="text-align: center;">
    <h3>Architecture</h3>
    <img src="docs/data_architecture.png" alt="Dashboard Overview" style="width: 80%; border-radius: 10px; box-shadow: 0 4px 10px rgba(0,0,0,0.2);">
  </div>

---

## 📖 Project Overview

This project covers the following core activities:

- Designing a modern data warehouse using Medallion Architecture (Bronze → Silver → Gold).
- Building ETL pipelines to extract data from CSV sources, transform and clean it, then load into the warehouse.
- Developing fact and dimension tables tailored for analytical queries and reporting.
- Creating SQL-based analytics and dashboards to surface insights into customers, products, and sales trends.

---

## 📂 Repository Structure

```
data-warehouse-project/
│
├── datasets/                           # Raw CSV datasets (ERP and CRM)
│
├── docs/                               # Documentation, diagrams, and requirements
│   ├── etl.drawio                      # ETL process diagrams
│   ├── data_architecture.drawio        # Overall architecture diagrams
│   ├── data_catalog.md                 # Dataset catalog and field metadata
│   ├── data_flow.drawio                # Data flow diagrams
│   ├── data_models.drawio              # Star schema and model diagrams
│   └── naming-conventions.md           # Naming and modeling standards
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Load raw CSV into staging / SQL Server
│   ├── silver/                         # Cleaning, deduplication, normalization
│   └── gold/                           # Build fact and dimension tables
│
├── tests/                              # Data quality checks and validation scripts
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information
├── .gitignore                          # Git ignore rules
└── requirements.txt                    # External tool dependencies (optional)
```

---

## 📌 How to Get Started

1. Clone the repository and review `docs/data_catalog.md` to understand dataset fields.
2. Install SQL Server Express and SSMS (or use a Dockerized SQL Server instance).
3. Load CSV files from `datasets/` into the Bronze staging tables using provided scripts.
4. Run Silver scripts to cleanse and standardize data.
5. Execute Gold scripts to create fact/dimension tables and validate results.
6. Run analytics SQL in SSMS or connect a BI tool to the Gold schema for dashboards.

---

📝 Conclusion

The AI-Finance Dashboard provides a comprehensive, modular, and scalable solution for managing business inventory and finances. Its integration of modern web technologies with real-time analytics enables actionable insights, efficient operations, and data-driven decision-making.
