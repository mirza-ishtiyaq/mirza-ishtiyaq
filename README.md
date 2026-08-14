<div align="center">

# Mirza Ishtiyaq Baig
### Data & Operations Analyst · BI Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mirzaishtiyaqbaig-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mirzaishtiyaqbaig/)
[![Email](https://img.shields.io/badge/Email-mirzaishtiyaqbaig1%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mirzaishtiyaqbaig1@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-mirza--ishtiyaq-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mirza-ishtiyaq)

![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Azure](https://img.shields.io/badge/Azure_Synapse-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=flat-square&logo=databricks&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat-square&logo=powerbi&logoColor=black)

</div>

---

## About

A 26-day shipment sat inside a 12.3-day average and nobody caught it.
That's the job — finding the thing the dashboard is quietly hiding.

Two years in CX and technical-support operations, now building the data
layer beneath the reporting. Eighteen months segmenting enterprise PC
failures to SKU level at Concentrix, then six months on Snowflake marts,
Databricks Medallion pipelines and Python data-quality frameworks —
strongest where operations meet the warehouse: SLA breaches, carrier
performance, fulfilment leakage.

---

## Find What You Need

| If you're hiring for... | Start here |
|---|---|
| **Data Analyst** | [Career Snapshot](#career-snapshot) → [Technical Stack: SQL & Data](#technical-stack) → [Automation & Process Improvement](#automation--process-improvement) |
| **Business Analyst** | [Selected Operational Work](#selected-operational-work) → [Domain Focus](#domain-focus) → [Actively Building](#actively-building) |
| **Operations Analyst** | [Career Snapshot](#career-snapshot) → [Automation & Process Improvement](#automation--process-improvement) |
| **BI Developer** | [Technical Stack: BI & Reporting](#technical-stack) → [Actively Building](#actively-building) |
| **Just want the numbers** | [Impact Snapshot](#impact-snapshot) |

---

## Career Snapshot

| Role | Organization | Period | What I Actually Did |
|---|---|---|---|
| Data Analytics Intern — Cloud Architecture & Operations | Full Stack Academy | Feb 2026 – Jul 2026 | Built three Snowflake, Databricks and DuckDB pipelines end-to-end and bridged a macOS-hosted MySQL instance to Power BI via a Python/ODBC connector — replacing manual exports with live refresh — then trained incoming candidates in SQL and Power BI. |
| Advisor II, Technical Support | Concentrix Technologies India | Jul 2024 – Dec 2025 | Automated the daily case-reporting workflow in Excel VBA and built Power BI dashboards on case volume and defect trends across consumer and commercial PC product lines — extracting from SQL Server and Microsoft Dynamics through Power Query and Power Pivot — to govern SLA attainment against a 98% target. |
| eSupport Officer — Incident Management | IntouchCX (24-7 Intouch) | Aug 2023 – Mar 2024 | Extracted and triaged live ticket inventory hourly from ServiceNow across multiple chat queues, routing cases to the right resolver team and flagging backlog build-up before it reached an SLA breach. |

---

## Selected Operational Work

**Concentrix — Technical Support Operations (18 months)**
Segmented recurring hardware failures across three consumer and commercial PC product lines to model level. Sustained 88–94% weekly resolution across 2,000+ cases while governing SLA attainment against a 98% target.

**IntouchCX — Incident Management (8 months)**
Ran continuous data validation on open-ticket inventory across multiple chat queues. Traced handle-time outliers to root cause and maintained fewer than one SLA deadline miss per month.

---

## Automation & Process Improvement

**Excel VBA Case-Reporting Automation (Concentrix)**
Automated the daily case-reporting workflow in Excel VBA, replacing a manual preparation sequence that previously consumed the first hour of every shift.

**macOS → Power BI Live-Reporting Bridge (Full Stack Academy)**
Built a Python/ODBC connector bridging a macOS-hosted MySQL instance to Power BI, replacing manual CSV exports with live dashboard refresh.

---

## Actively Building

Real gaps against 2026 role requirements, closed deliberately rather than
glossed over. An entry is added here only once there's a genuine, defensible
deliverable behind it — not before.

<!-- Entries added here as each deliverable is completed. Do not add
     placeholder, aspirational, or "in progress" entries without a real
     artefact behind them. -->

---

## Technical Stack

| Layer | Tools |
|---|---|
| **Cloud Platforms** | Snowflake · Databricks (Delta Lake) · Azure Synapse Analytics · Microsoft Fabric |
| **Architecture** | Medallion Architecture (Bronze/Silver/Gold) · Star Schema · ETL/ELT Pipelines |
| **SQL** | Advanced SQL (CTEs, Window Functions) · T-SQL · Spark SQL · MySQL 8.0 · DuckDB |
| **Python** | Pandas · NumPy · Matplotlib · REST API Ingestion · Faker (synthetic data) |
| **BI & Reporting** | Power BI · DAX · Power Query · Power Pivot · Exception Reporting |
| **CX Domain** | Microsoft Dynamics 365 · SLA Governance · Case Telemetry · Ticket Lifecycle Analytics |

---

## Featured Projects

The three case studies below are the ones I'd point a recruiter to first — they map directly to the domain I'm targeting (e-commerce operations, supply chain, and CX analytics) and each carries a quantified, verified business outcome. Four more projects — SQL, BI, and data-quality work — are summarized further down in [Additional Projects](#additional-projects).

### 1. Cold-Chain Spoilage & Carrier SLA Recovery Engine
**[📦 pharma-cold-chain-analytics](https://github.com/mirza-ishtiyaq/pharma-cold-chain-analytics)** &nbsp; `Snowflake` `Python` `Open-Meteo REST API` `Power BI`

**Data Source:** 5,000 pharmaceutical shipment records across 5 Indian logistics hubs (Hyderabad, Mumbai, Delhi, Chennai, Bangalore), joined against real historical weather telemetry pulled live from the Open-Meteo Historical Weather REST API.

**Problem:** Cold-chain teams had no visibility into whether spoilage was driven by ambient heat, carrier transit delays, or a combination of both — and no financial mechanism to hold underperforming 3PL carriers accountable.

```mermaid
flowchart LR
    A["Open-Meteo REST API<br/>+ ERP Shipment Logs"] --> B["Snowflake RAW Layer<br/>(Staging Tables)"]
    B --> C["Snowflake CLEAN Layer<br/>(Whitespace, Dates, Nulls)"]
    C --> D["Snowflake BUSINESS Layer<br/>(Spoilage & Loss Model)"]
    D --> E["Power BI Command Center<br/>(SLA Claims & Spoilage)"]
```

![Pharma Cold-Chain Spoilage Dashboard](images/snowflake_pharma_dashboard.jpg)

**Solution & Findings:**
- **$708,550** in YTD spoilage loss across 297 of 5,000 shipments — a **5.94%** spoilage rate against a **<2%** industry benchmark.
- Ran an actual chi-square test on the ">30°C origin temp + >40hr transit" hypothesis rather than presenting it as proven: the result is **not statistically significant at this sample size (p≈0.41)**, reported honestly as a monitoring hypothesis, not a confirmed root cause.
- Surfaced two real data-quality blockers before the finding gets used to justify a packaging-SOP change: the weather feed only covers **49% of shipments**, and **124 Shipment_IDs** carry genuinely conflicting duplicate records.
- **Delhivery + FedEx account for 42% ($298,750)** of total loss — a documented, carrier-attributable SLA claim.

**Tools Used:** Snowflake SQL (RAW → CLEAN → BUSINESS schemas), Python (REST ingestion, Pandas), Power BI (exception-reporting UX).

**Stakeholder Summary:** There is a recoverable **$298.75K SLA claim** against two named carriers, actionable today. The temperature-transit packaging fix is **not yet justified by the data** — closing the weather-coverage gap is the next step, before that capital investment, not after.

---

### 2. E-Commerce Fulfilment Medallion Pipeline & Revenue Leakage Audit
**[📦 ecommerce-medallion-pipeline](https://github.com/mirza-ishtiyaq/ecommerce-medallion-pipeline)** &nbsp; `Databricks` `Spark SQL` `Delta Lake` `Power BI`

**Data Source:** The public [Brazilian E-Commerce (Olist) dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) — ~99,000 real orders across customers, orders, items, products, sellers, and geolocation tables.

**Problem:** Reporting directly off raw transactional tables created dashboard latency and pushed business logic — SLA flags, revenue-loss classification — into Power BI instead of resolving it upstream.

```mermaid
flowchart LR
    A["Raw Transactional &<br/>Logistics Extracts (Olist)"] --> B["Databricks BRONZE Layer<br/>(Raw Delta Lake Tables)"]
    B --> C["Databricks SILVER Layer<br/>(Timestamp Parsing & Schema)"]
    C --> D["Databricks GOLD Layer<br/>(Star Schema & SLA Fact)"]
    D --> E["Power BI Dashboard<br/>(Revenue Leakage & Transit)"]
```

![E-Commerce Medallion Data Model](images/databricks_data_model.png)
![E-Commerce Financial Dashboard](images/databricks_finance_dashboard.png)
![E-Commerce Logistics Dashboard](images/databricks_logistics_dashboard.png)

**Solution & Findings:**
- **90%** of transformations and star-schema modeling pushed upstream of Power BI via a Bronze → Silver → Gold Delta Lake build.
- **$97.24K revenue leakage** identified — **8.12%** of a **$1.20M** gross pipeline — trapped in canceled/unavailable order states.
- **26-day regional transit outlier** versus a **12.3-day** national baseline.
- Independently re-checked the dashboard's own screenshots and caught a real labeling bug: the 26-day bottleneck state is **Rondônia ("RO")**, mislabeled as Roraima ("RR") in the original dashboard — corrected in this write-up.

**Tools Used:** Databricks, Spark SQL, Delta Lake (ACID transactions), Power BI (star-schema import model).

**Stakeholder Summary:** Finance can act on a documented **$97.24K leakage figure** today. Logistics should investigate **Rondônia specifically** — not Roraima, per the corrected record — before renegotiating carrier contracts on that lane.

---

### 3. CX Support Ticket Lifecycle & SLA Breach Diagnostic Engine
**[📦 cx-ticket-lifecycle-engine](https://github.com/mirza-ishtiyaq/cx-ticket-lifecycle-engine)** &nbsp; `DuckDB` `Python (Faker, Pandas)` `SQL`

**Data Source:** The FakeStore public REST API (real 20-SKU product catalog) plus a fully seeded synthetic transactional layer (`Faker.seed(42)`) generating **1,000,000 orders**, **1,000,000 support tickets**, and **50,000 customers** — deterministic and independently reproducible end-to-end.

**Problem:** Support and fulfilment teams need to identify which high-value customers are experiencing SLA breaches **before** it shows up as churn, not after.

```mermaid
flowchart LR
    A["FakeStore REST API<br/>+ Synthetic Engine (Faker)"] --> B["DuckDB BRONZE Layer<br/>(Raw Orders & Tickets)"]
    B --> C["DuckDB SILVER Layer<br/>(SLA Ageing & Window Functions)"]
    C --> D["DuckDB GOLD Layer<br/>(VIP Risk Fact Table)"]
    D --> E["Executive Analytics Suite<br/>(Cohort Retention & SLA Diagnostics)"]
```

![CX SLA Breach Diagnostic Dashboard](images/e_commerce_etl_dashboard.png)

**Solution & Findings:**
- **$244.8M** total order revenue modeled · **$244.82** AOV · **$4,896.31** average customer lifetime value.
- **50.04%** overall SLA compliance — 499,566 of 1M tickets breached.
- **49.35%** of all tickets (493,502) classified `URGENT – High-Value VIP` (customers with $2,500+ LTV hitting an SLA breach).
- Built a window-function cohort retention layer on top — and stated plainly that the ~54–57% flat retention this specific dataset shows is an honest property of **uniformly random synthetic order dates**, not a real decay curve, rather than dressing up a meaningless result as insight.
- Re-ran the entire pipeline end-to-end for this review — every headline figure reproduced exactly. The one project in this portfolio built for full, byte-for-byte reproducibility.

**Tools Used:** DuckDB, Python (Faker, Pandas), SQL (window functions), Matplotlib/Seaborn.

**Stakeholder Summary:** CX leadership gets one concrete, ready-to-wire rule: auto-escalate the ~493K tickets tagged `URGENT–VIP` to a sub-4-hour SLA queue — the single highest-leverage retention lever this dataset surfaces.

---

## Domain Focus

**CX & Operations Analytics**
SLA governance · case telemetry · ticket lifecycle reporting · handle-time analysis · CRM data quality · Dynamics 365

**Business Analysis & Process Improvement:** requirements translation · stakeholder communication · root cause analysis · process documentation

**Supply Chain & Logistics Analytics**
Cold-chain risk modelling · transit delay analytics · order fulfilment analytics · 3PL performance reporting

**Cloud Data Architecture**
Medallion pipeline design · Snowflake data mart engineering · Azure Synapse modelling · Delta Lake · star schema design

---

## Impact Snapshot

| Metric | Where It Came From |
|---|---|
| **$708.5K** spoilage loss quantified — **$298K recoverable** in SLA claims against 2 named carriers | Pharmaceutical Cold-Chain Analytics (Snowflake) |
| **$97.24K** revenue leakage surfaced in a $1.20M e-commerce pipeline | E-Commerce Medallion Pipeline (Databricks) |
| **2,000,000+** orders & support tickets processed in a Bronze→Silver→Gold warehouse | CX SLA Diagnostic Engine (DuckDB) |
| **49.35%** of tickets flagged urgent VIP-risk before they became churn | CX SLA Diagnostic Engine (DuckDB) |
| **7** end-to-end analytics builds across Snowflake, Databricks, Synapse, MySQL, DuckDB & Python — 3 featured as core case studies below | This portfolio |
| **3** real data/reporting bugs found and fixed under independent review | Not just built — checked |

---

## Additional Projects

Broader SQL, BI, and data-engineering fundamentals — each still a complete, verified build, kept here in short form so the three case studies above stay the focus.

| Project | Stack | Highlight |
|---|---|---|
| **Enterprise Sales Analytics Dashboard** | Azure Fabric · Spark SQL · Power BI · DAX · Excel | $2.26M in multi-year sales reconciled Power BI ↔ Excel to the cent; the project behind my Python/ODBC live-reporting bridge from the Full Stack Academy internship. |
| **Retail Data Quality & Executive Analytics Engine** | Python · Pandas · NumPy · Matplotlib | Modular dedup → standardize → impute → join pipeline that deliberately avoided a fan-out join bug and caught 3 orphan transactions instead of silently absorbing them. |
| **Sales Data Analysis & Business Logic** | MySQL 8.0+ · CTEs · Window Functions | Traced a revenue-undercounting `INNER JOIN` bug across its full lifecycle — diagnosed, "fixed" only in a comment, then actually fixed in the final pipeline. |
| **EcomDB — Enterprise SQL Analytics Suite** | T-SQL · Azure Synapse · Microsoft Fabric | Five production business-question queries (revenue ranking, cold-lead detection, loyalty segmentation) with documented Synapse/Fabric-specific gotchas. |

---

## Data & Reproducibility

Project datasets are **synthetic or public** — real client and transaction data from my CX roles is confidential and cannot be published. Weather data in the cold-chain project is real, pulled live from the Open-Meteo Historical Weather API. Synthetic datasets are generated with deliberate quality defects (mixed timestamp formats, duplicate keys, null fields, negative lead-times) so the cleaning layers solve problems that actually occur in production extracts.

---

## Education & Certifications

**B.Sc. Data Science** — Osmania University, Hyderabad, India · 2025

**Certifications:**
- Microsoft Fabric: Data Flows & Data Storage (2025)
- SQL for Data Analysis — LinkedIn (2025)
- Analyzing & Visualizing Data Using Excel — NASBA (2025)
- Excel Data Management — PMI (2025)
- Data Analytics Internship — Full Stack Academy (2026)

---

## Currently

Targeting **Data Analyst**, **Business Analyst**, **Operations Analyst**, and **BI Developer** roles — particularly in e-commerce operations, supply chain, and CX analytics.

---

## Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mirzaishtiyaqbaig-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mirzaishtiyaqbaig/)
[![Email](https://img.shields.io/badge/Email-mirzaishtiyaqbaig1%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mirzaishtiyaqbaig1@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-mirza--ishtiyaq-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mirza-ishtiyaq)
