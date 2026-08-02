# Mirza Ishtiyaq Baig | Data Analyst

**CX & Operations Analytics · Cloud Data Architecture · SQL · Python · Power BI**

[LinkedIn](https://www.linkedin.com/in/mirzaishtiyaqbaig/) · [Email](mailto:mirzaishtiyaqbaig1@gmail.com) · Hyderabad, India · Open to Work

---

## About

Data Analyst with 2+ years embedded inside CX and technical support operations — not observing the data from a distance, but managing the workflows that generated it.

At Concentrix, I owned the analytical layer of a 2,000+ weekly case environment: building live data pipelines from Microsoft Fabric via Power Query, designing Power Pivot models consumed directly by the BI development team, and running case telemetry analysis that contributed to an 18% reduction in Tier-2 escalations. That operational grounding shapes how I frame analytical problems — I understand what SLA ageing, routing failures, and handle-time patterns mean before I open a query editor.

My project portfolio extends this into cloud data architecture — Medallion pipelines on Databricks, Snowflake-based data marts, Azure Synapse analytical models, and Python/SQL data engineering — each built on simulated or public operational datasets, and each held to one standard: **every claim in the writeup has to survive being checked against the underlying code and data.** Several of these projects turned up real issues on that kind of review — a revenue-inflating join bug, an unproven "root cause" that didn't survive a significance test, SQL demos that weren't actually reproducible against their own seed data — and each was fixed rather than smoothed over. That review trail is documented in every project's README, not hidden.

---

## Technical Stack

| Layer | Tools |
|---|---|
| **Cloud Platforms** | Snowflake · Databricks (Delta Lake) · Azure Synapse Analytics · Microsoft Fabric |
| **Architecture** | Medallion Architecture (Bronze/Silver/Gold) · Star Schema · ETL/ELT Pipelines |
| **SQL** | Advanced SQL (CTEs, Window Functions, JSON parsing) · T-SQL · Spark SQL · MySQL 8.0 · DuckDB |
| **Python** | Pandas · NumPy · Matplotlib · Seaborn · REST API Ingestion · Faker (synthetic data) |
| **BI & Reporting** | Power BI · DAX · Power Query · Exception Reporting · Executive Dashboards |
| **CX Domain** | Microsoft Dynamics 365 · SLA Governance · Case Telemetry · Ticket Lifecycle Analytics |

---

## Projects

### 1. [Enterprise Databricks Medallion Pipeline](https://github.com/mirza-ishtiyaq/databricks-medallion-architecture)
**Stack:** Databricks · Spark SQL · Delta Lake · Power BI

**Problem:** Fragmented e-commerce and logistics data with no unified analytical layer — causing slow BI reporting and business logic leaking into dashboards instead of being resolved at the data layer.

**What I built:** A full Bronze-Silver-Gold Medallion architecture over the public Olist Brazilian e-commerce dataset (~99K orders). Bronze ingests raw source data as Delta tables; Silver handles temporal normalization and null-key filtering; Gold builds an optimized star schema with pre-computed delivery-SLA flags and a dedicated lost-revenue fact table, pushing 90% of business logic upstream of Power BI. Cross-checked the dashboard's headline figures ($1.20M gross revenue, $97.24K/8.12% leakage, 12.3-day national transit) directly against the underlying screenshots — and caught a real labeling error: the 26-day logistics bottleneck state is Rondônia ("RO"), not Roraima ("RR") as the dashboard itself had mislabeled it.

**Patterns demonstrated:** Medallion architecture design · Delta Lake ACID transactions · Star schema modeling · Screenshot-grounded verification

---

### 2. [Pharmaceutical Cold-Chain Logistics: Spoilage Analytics](https://github.com/mirza-ishtiyaq/snowflake-pharma-logistics-pipeline)
**Stack:** Snowflake · Python · Open-Meteo REST API · Power BI

**Problem:** Cold-chain operations lack visibility into how weather conditions and 3PL carrier transit delays drive pharmaceutical spoilage risk — making it invisible until after the loss is booked.

**What I built:** A multi-layer Snowflake data mart (RAW → CLEAN → BUSINESS) joining 5,000 shipment records against live weather API data, with a per-carrier, per-product financial-loss model. Replicated the Snowflake SQL logic locally against the raw CSVs to independently re-verify every headline number: corrected a $1,000 typo in the total-loss figure, and ran an actual chi-square test on the "high-temperature + long-transit" root-cause claim the original analysis presented as proven — it turned out to be a mild, statistically insignificant signal (p≈0.41), not a confirmed driver. Also surfaced two real data-quality issues: the weather feed only covers half the shipment date range, and 124 shipment IDs carry genuinely conflicting duplicate records.

**Patterns demonstrated:** Multi-source data integration · Snowflake staging architecture · Statistical hypothesis testing · Correcting an unsupported causal claim instead of leaving it in

---

### 3. [EcomDB Analytics Suite — Azure Synapse](https://github.com/mirza-ishtiyaq/azure-synapse-enterprise-analytics)
**Stack:** Azure Synapse Analytics · Microsoft Fabric · T-SQL

**Problem:** E-commerce operations need analytical models beyond revenue totals — identifying at-risk customers, anomalous transactions, and retention patterns from raw transactional data at scale.

**What I built:** Five production-style T-SQL query patterns (a `DENSE_RANK` tie-surfacing example, `NOT EXISTS` cold-lead detection, a consecutive-purchase-day "anchor" trick, loyalty segmentation, and two approaches to impulse-purchase detection) against a normalized 5-table schema, with explicit Synapse/Fabric platform-quirk documentation. Actually executed all five queries against the seed data to confirm the documented behaviors hold — and found the two flagship examples (the ranking tie and the purchase streak) weren't reproducible against the original seed data at all, so extended it with two minimal, clearly-marked rows so both are now genuinely verifiable, not just narrated.

**Patterns demonstrated:** Defensive T-SQL methodology · Azure Synapse architecture · Customer lifecycle analytics · Execution-verified query documentation

---

### 4. [Production Data Cleansing & EDA Engine](https://github.com/mirza-ishtiyaq/python-data-quality-engine)
**Stack:** Python · Pandas · NumPy · Matplotlib

**Problem:** CRM and fulfillment datasets inherited by analysts routinely carry deduplication failures, inconsistent categoricals, and missing values that silently corrupt downstream reporting — and leave no trace of what was fixed.

**What I built:** A modular Python data-quality engine (`deduplicate_entities`, `standardize_countries`, `impute_missing`) with a full anomaly audit trail. Executing the notebook end-to-end for this review surfaced and fixed a genuine cartesian-join bug that had been inflating summed revenue by ~22%, and replaced a set of headline metrics that turned out to be unverified — Average Order Value and Average Transaction Value were both listed as an identical, implausible $104.38 — with real, execution-verified figures.

**Patterns demonstrated:** Production-grade data cleansing architecture · Modular Python design · Referential-integrity bug detection · Data quality auditing with a full audit trail

---

### 5. E-Commerce Data Warehouse & Analytics Pipeline <sup>†</sup>
**Stack:** DuckDB · Python (Faker, Pandas) · SQL

**Problem:** Support and fulfillment teams need to know which high-value customers are experiencing SLA breaches before it shows up as churn.

**What I built:** A seeded, fully deterministic synthetic-data ELT pipeline (1M orders, 1M support tickets, 50K customers) through a Bronze→Silver→Gold DuckDB warehouse, with a window-function-based cohort retention analysis layered on top of the KPI reporting. Re-ran the entire pipeline end-to-end for this review and confirmed every headline figure reproduces exactly — the one project in this portfolio built for full, byte-for-byte reproducibility rather than a single point-in-time analysis.

**Patterns demonstrated:** Deterministic/seeded synthetic data generation · Medallion ELT in DuckDB · Window-function cohort retention · SLA/VIP risk modeling

<sup>† Repository not yet published to GitHub — local project, available on request.</sup>

---

### 6. [Retail Sales Analytics & Store Performance Reporting](https://github.com/mirza-ishtiyaq/Retail-Sales-Analysis)
**Stack:** Python · Pandas · Seaborn · SQL (DuckDB)

**Problem:** Multi-branch retail operations need visibility into which product categories and store locations are driving margin versus volume — and where seasonal demand creates inventory risk.

**What I built:** An EDA pipeline across a 9,800-row, 4-year Superstore-style dataset producing category and regional revenue breakdowns and seasonality trends, now backed by a DuckDB SQL layer that independently cross-validates every pandas aggregation via an `assert`-checked SQL query — so the "Python · Seaborn · SQL" stack is real working code, not just a label.

**Patterns demonstrated:** Exploratory data analysis · Cross-validated dual-engine (pandas + SQL) reporting · Regional performance benchmarking · Transparent handling of a missing source-data gap

---

### 7. [SQL Sales Analytics Engine](https://github.com/mirza-ishtiyaq/Sales_Analysis.SQL)
**Stack:** MySQL 8.0 · CTEs · Window Functions

**Problem:** Translate raw, duplicate-ridden transactional sales data into trustworthy, queryable BI views — without letting a join-type mistake silently understate revenue.

**What I built:** A five-file MySQL pipeline that documents the actual evolution of the work: an original exploratory script, the same logic refactored into single-responsibility phases, and a final consolidated pipeline. It traces one bug end-to-end — the legacy script correctly diagnosed a revenue-undercounting `INNER JOIN` but never actually fixed it; the final pipeline does. This review caught and fixed a second, independent bug: a non-deterministic `ROW_NUMBER()` tie-break in the dedup logic, caused by ordering a partition by its own partition key.

**Patterns demonstrated:** CTEs and window functions (`LAG`, `ROW_NUMBER`) · Join-type business-impact awareness · Documented pipeline evolution and bug-fix history · Independent query correctness review

---

### 8. [U.S. Greenhouse Gas Emissions Analytics](https://github.com/mirza-ishtiyaq/Databricks-Repo)
**Stack:** Databricks · Spark SQL

**Problem:** Environmental policy and sustainability teams need state, county, and per-capita emissions views from inconsistently formatted source data to target high-impact regions.

**What I built:** A Databricks SQL pipeline that cleans comma-formatted numeric strings and guards per-capita calculations against division-by-zero, with a CTE-based state-share-of-national-total pattern and a version-controlled Lakeview executive dashboard. Added a data-quality check (`TRY_CAST`) to explicitly flag values that silently fail to parse instead of disappearing as unexplained `NULL`s.

**Patterns demonstrated:** Spark SQL data cleaning · CTE-based share-of-total analysis · Lakeview dashboard-as-code · Guardrails against silent cast failures

---

### 9. [Power BI Enterprise Sales Analytics Solution](https://github.com/mirza-ishtiyaq/PowerBI_Sales_analysis_dashboard)
**Stack:** Azure Fabric · Spark SQL · Excel · Power BI · DAX

**Problem:** Leadership needs a five-minute read on whether growth is accelerating, which category is underperforming, and whether a "YoY win" is real growth or a bounce-back from a weak prior year.

**What I built:** A two-page Power BI report (KPI cards, YoY/LY comparisons, category and segment breakdowns) independently validated against Excel pivot tables. Rewrote the documentation by directly inspecting the dashboard screenshots rather than relying on the prior text, surfacing findings the original writeup didn't have — the headline 46.9% YoY growth sits on top of a 2016 dip, and 2018's full-year revenue record masks an in-year MTD softening from a 2017 peak.

**Patterns demonstrated:** Power BI star-schema modeling · DAX time-intelligence measures · Cross-tool validation (Excel vs. Power BI) · Screenshot-grounded, evidence-based reporting

---

## Domain Focus

**CX & Operations Analytics**
SLA governance · case telemetry · ticket lifecycle reporting · handle-time analysis · CRM data quality · WISMO

**Supply Chain & Logistics Analytics**
Cold-chain risk modelling · transit delay analytics · order fulfilment analytics · 3PL performance reporting

**Cloud Data Architecture**
Medallion pipeline design · Snowflake data mart engineering · Azure Synapse modelling · Delta Lake · star schema · environmental/public-sector analytics

---

## Let's Connect

- **LinkedIn:** [linkedin.com/in/mirzaishtiyaqbaig](https://www.linkedin.com/in/mirzaishtiyaqbaig/)
- **Email:** mirzaishtiyaqbaig1@gmail.com
- **Location:** Hyderabad, India · Open to pan-India or remote roles
