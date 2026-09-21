# Growth Insights Data Platform

A robust, end-to-end data platform engineered to ingest, transform, validate, and load user growth and product analytics data for reliable data warehousing and analytics.

---

## 🛠 Tech Stack

- **Core Language:** Python
- **Data Processing & Manipulation:** Pandas, SQL
- **Database & Data Warehouse:** PostgreSQL
- **Workflow Orchestration:** Apache Airflow
- **Cloud Object Storage:** AWS S3
- **Containerization & Deployment:** Docker & Docker Compose

---

## 🎯 Problem Statement

Fast-growing organizations generate high-volume product and marketing data across multiple disjointed sources. Without an automated, reliable data engineering pipeline, raw data suffers from inconsistent schemas, missing values, duplicates, and unvalidated quality. This creates delays in business reporting, unreliable analytics, and a lack of scalable infrastructure for tracking key metrics like customer retention, user acquisition, and conversion funnels.

---

## 💡 Solution

The **Growth Insights Data Platform** provides an automated, production-ready ETL/ELT pipeline architecture:
1. **Extraction & Ingestion:** Ingests raw batch and streaming datasets into cloud landing zones (AWS S3) and local staging areas.
2. **Validation & Quality Control:** Automatically checks incoming data against schema requirements and validation rules, routing invalid records to a rejected partition for auditability.
3. **Transformation:** Cleans, standardizes, and enriches data using Pandas and optimized SQL transformations.
4. **Data Warehousing & Load:** Loads processed data into PostgreSQL structured data models (DDL / Star Schema) optimized for analytical reporting.
5. **Orchestration & Infrastructure:** Manages workflow dependencies, retries, and monitoring via Apache Airflow, fully containerized using Docker.

---

## 📂 Project Structure

```
growth-insights/
├── dags/                  # Apache Airflow DAG definitions & workflows
├── data/                  # Data directory (contents git-ignored)
│   ├── raw/               # Raw incoming data landing zone
│   ├── clean/             # Processed and validated data
│   └── rejected/          # Quarantine zone for records failing validation
├── docs/                  # Documentation & progress tracking
│   └── progress.md        # Daily project log & milestones
├── sql/                   # SQL scripts
│   ├── ddl/               # Schema definitions, tables, and indexes
│   └── analytics/         # Business intelligence & analytical queries
├── src/                   # Core Python application logic
│   ├── generate/          # Synthetic data generators & mock providers
│   ├── extract/           # Data extraction routines & API connectors
│   ├── transform/         # Transformation logic & business rules
│   ├── validate/          # Data quality checks & schema assertions
│   └── load/              # Database loaders & S3 destination handlers
├── tests/                 # Unit & integration test suites
├── .gitignore             # Environment & artifact exclusions
└── README.md              # Project documentation
```

---

## 🗺 8-Week Roadmap

- [ ] **Week 1:** Project Setup, Architecture Design & Synthetic Data Generation
- [ ] **Week 2:** Data Extraction & Raw Storage Setup (AWS S3)
- [ ] **Week 3:** Data Quality & Schema Validation Rules (Data Quarantine Pipeline)
- [ ] **Week 4:** Data Transformation & Business Logic Implementation (Pandas & SQL)
- [ ] **Week 5:** PostgreSQL Data Warehouse Modeling (DDL) & Automated Loaders
- [ ] **Week 6:** Workflow Orchestration using Apache Airflow DAGs
- [ ] **Week 7:** Docker Containerization, Services Setup & End-to-End Integration
- [ ] **Week 8:** Analytics Queries, Business Reports & Final Platform Documentation
