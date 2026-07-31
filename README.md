# Mirza Ishtiyaq Baig | Data Analyst

**CX & Operations Analytics · Cloud Data Architecture · SQL · Python · Power BI**

[LinkedIn](https://www.linkedin.com/in/mirzaishtiyaqbaig/) · [Email](mailto:mirzaishtiyaqbaig1@gmail.com) · Hyderabad, India · Open to Work

---

## About

Data Analyst with 2+ years embedded inside CX and technical support operations — not observing the data from a distance, but managing the workflows that generated it.

At Concentrix, I owned the analytical layer of a 2,000+ weekly case environment: building live data pipelines from Microsoft Fabric via Power Query, designing Power Pivot models consumed directly by the BI development team, and running case telemetry analysis that contributed to an 18% reduction in Tier-2 escalations. That operational grounding shapes how I frame analytical problems — I understand what SLA ageing, routing failures, and handle-time patterns mean before I open a query editor.

My project portfolio extends this into cloud data architecture — Medallion pipelines on Databricks, Snowflake-based data marts, Azure Synapse analytical models, and Python data quality engines — each built on simulated operational datasets to demonstrate end-to-end methodology, architectural thinking, and production-grade code standards.

---

## Technical Stack

| Layer | Tools |
|---|---|
| **Cloud Platforms** | Snowflake · Databricks (Delta Lake) · Azure Synapse Analytics · Microsoft Fabric |
| **Architecture** | Medallion Architecture (Bronze/Silver/Gold) · Star Schema · ETL/ELT Pipelines |
| **SQL** | Advanced SQL (CTEs, Window Functions, JSON parsing) · T-SQL · Spark SQL |
| **Python** | Pandas · NumPy · Matplotlib · REST API Ingestion |
| **BI & Reporting** | Power BI · DAX · Power Query · Exception Reporting · Executive Dashboards |
| **CX Domain** | Microsoft Dynamics 365 · SLA Governance · Case Telemetry · Ticket Lifecycle Analytics |

---

## Projects

### 1. [Enterprise Databricks Medallion Pipeline](https://github.com/mirza-ishtiyaq/databricks-medallion-architecture)
**Stack:** Databricks · Spark SQL · Delta Lake · Power BI

**Problem:** Fragmented CRM and logistics data with no unified analytical layer — causing slow BI reporting and business logic leaking into dashboards instead of being resolved at the data layer.

**What I built:** A full Bronze-Silver-Gold Medallion architecture on Databricks. Bronze ingests raw source data. Silver handles temporal normalisation, null resolution, and deduplication. Gold constructs optimised Fact/Dimension star schemas, pushing 90% of business logic upstream so Power BI reads pre-aggregated, clean models — not raw tables.

**Patterns demonstrated:** Medallion architecture design · Delta Lake ACID transactions · Star schema modelling · Upstream logic consolidation

---

### 2. [Pharmaceutical Cold-Chain Logistics: Spoilage Analytics](https://github.com/mirza-ishtiyaq/snowflake-pharma-logistics-pipeline)
**Stack:** Snowflake · Python · Open-Meteo REST API · Power BI

**Problem:** Cold-chain operations lack visibility into how weather conditions correlate with transit delays across 3PL carriers — making spoilage risk invisible until post-shipment.

**What I built:** An end-to-end analytics scenario designed to surface that risk. Ingested live weather API data via Python into a multi-layer Snowflake environment (RAW → CLEAN → BUSINESS), joined it with a simulated shipment fulfilment dataset of 5,000 records, and engineered a transit delay and financial exposure model segmented by 3PL carrier and transit corridor. Built for executive-level spoilage risk reporting.

**Patterns demonstrated:** Multi-source data integration · Snowflake staging architecture · REST API ingestion · Financial risk modelling from operational data

---

### 3. [EcomDB Analytics Suite — Azure Synapse](https://github.com/mirza-ishtiyaq/azure-synapse-enterprise-analytics)
**Stack:** Azure Synapse Analytics · Microsoft Fabric · T-SQL

**Problem:** E-commerce operations need analytical models beyond revenue totals — identifying at-risk customers, anomalous transactions, and retention patterns from raw transactional data at scale.

**What I built:** A set of production-ready T-SQL analytical models targeting cold lead identification, transaction anomaly detection, and customer retention scoring. Written with strict CTE architecture throughout, handling Synapse-specific DATETIME2 constraints, and designed to demonstrate join consequence awareness on large distributed datasets.

**Patterns demonstrated:** Defensive T-SQL methodology · Azure Synapse architecture · Customer lifecycle analytics · Anomaly detection logic

---

### 4. [Production Data Cleansing & EDA Engine](https://github.com/mirza-ishtiyaq/python-data-quality-engine)
**Stack:** Python · Pandas · NumPy · Matplotlib

**Problem:** CRM and fulfilment datasets inherited by analysts routinely carry deduplication failures, inconsistent categoricals, and missing values that silently corrupt downstream reporting — and leave no trace of what was fixed.

**What I built:** A modular Python data quality engine applied to a simulated CRM and fulfilment dataset. Handles primary key deduplication, categorical string normalisation, non-destructive missing value imputation, and transit lead-time anomaly detection — producing a clean, analytics-ready output with a full audit trail of every transformation applied.

**Patterns demonstrated:** Production-grade data cleansing architecture · Modular Python design · Data quality auditing · EDA pipeline structuring

---

### 5. [Retail Sales Analytics & Store Performance Reporting](https://github.com/mirza-ishtiyaq/Retail-Sales-Analysis)
**Stack:** Python · Pandas · Seaborn · SQL

**Problem:** Multi-branch retail operations need visibility into which product categories and store locations are driving margin versus volume — and where seasonal demand creates inventory risk.

**What I built:** An EDA-driven analytics pipeline across a multi-category, multi-region retail transaction dataset. Generates category-level revenue heatmaps, isolates high-yield product segments by region, and surfaces seasonal demand shifts — structured as a reusable reporting pipeline with automated summary outputs.

**Patterns demonstrated:** Exploratory data analysis · Retail operations analytics · Regional performance benchmarking · Automated reporting structure

---

## Domain Focus

**CX & Operations Analytics**  
SLA governance · case telemetry · ticket lifecycle reporting · handle-time analysis · CRM data quality · WISMO

**Supply Chain & Logistics Analytics**  
Cold-chain risk modelling · transit delay analytics · order fulfilment analytics · 3PL performance reporting

**Cloud Data Architecture**  
Medallion pipeline design · Snowflake data mart engineering · Azure Synapse modelling · Delta Lake · Star schema

---

## Let's Connect

- **LinkedIn:** [linkedin.com/in/mirzaishtiyaqbaig](https://www.linkedin.com/in/mirzaishtiyaqbaig/)
- **Email:** mirzaishtiyaqbaig1@gmail.com
- **Location:** Hyderabad, India · Open to pan-India or remote roles
