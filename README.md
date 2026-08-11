# Roland Dela Rosa — Data Analyst & Data Scientist Portfolio

**Portfolio repository:** https://rolanddelarosaph.github.io/analytics/

---

## Overview

Personal analytics portfolio for Roland Dela Rosa, a BS Statistics graduate from Rizal Technological University, DOST Undergraduate Scholar, and Magna Cum Laude. The portfolio focuses on statistical analysis, Bayesian modeling, time-series forecasting, predictive modeling, business analytics, and data visualization, supported by hands-on experience building reliable ETL/ELT pipelines and analytical data models.

Built with vanilla HTML, CSS, and JavaScript — no frameworks or build tools.

---

## Repository Structure

```text
analytics/
├── index.html          # Main portfolio page
├── README.md           # This file
├── .gitignore
└── images/
    ├── architecture food pipeline.png
    ├── architecture datawarehouse.png
    ├── architecture lfs.png
    ├── ph_food_price_dashboard.png
    └── bayesian_model_result.png
```

---

## What I Built

### Philippine Food Price Analytics Pipeline

Analytics and forecasting project built to examine whether actual Philippine market food prices are rising faster than the official CPI and whether peso depreciation provides an early signal of food price increases. It combines WFP market prices, PSA Consumer Price Index data, and live BSP exchange rates, then applies lag-correlation analysis and Prophet time-series forecasting. The analysis found that peso depreciation leads food price increases by 1–2 months (r=0.29, p=0.018), while NCR food prices run 60+ index points above the official CPI.

The analytical layer is supported by an end-to-end cloud ELT pipeline: 300K+ rows are ingested into Snowflake, transformed through dbt using a Bronze/Silver/Gold Medallion Architecture, validated with 20 automated data-quality tests, orchestrated by Apache Airflow on Astronomer Cloud, and surfaced through a live Tableau dashboard.

**Analytics / Modeling:** Time Series Forecasting · Prophet · Predictive Modeling · Lag Analysis · Statistical Analysis · Tableau

**Data / Engineering:** Python · Snowflake · dbt · Apache Airflow · Astronomer Cloud · BSP Live API · Medallion Architecture

**Repository:** https://github.com/rolanddelarosaph/ph-food-price-pipeline

---

### European Fashion Retail Data Warehouse & Analytics

Business analytics and SQL data-warehouse project built from seven European fashion retail datasets. The analytical layer covers revenue trends, channel performance, campaign attribution, product ranking by country, and stockout risk for high-velocity SKUs. Key findings include 92.7% of revenue coming from full-price orders and 55% of product-country inventory positions sitting at critical stock levels.

The analysis is powered by a MySQL star schema and a reproducible pipeline with stored procedures, transaction control, deduplication through `ROW_NUMBER()`, indexed fact tables, and SQL data-quality checks. Business queries use CTEs, window functions, `RANK()`, and `LAG()` to turn the warehouse into decision-ready analysis.

**Stack:** SQL Analytics · MySQL 8.0 · Python · Stored Procedures · Star Schema · Window Functions · CTEs · RANK() · LAG()

**Repository:** https://github.com/rolanddelarosaph/datawarehouse-european-ecommerce

---

### Bayesian Multilevel Modeling of Intergenerational Educational Mobility — PSA LFS Pipeline

Undergraduate thesis centered on Bayesian multilevel modeling of intergenerational educational mobility using PSA Labor Force Survey microdata. A Bayesian Multilevel Linear Model estimates how parental education predicts children's schooling outcomes across all 17 Philippine regions, with region-level random intercepts and slopes fitted through Bambi and PyMC. The analysis found a nationally consistent father-son educational persistence slope of 0.265, with regional estimates close enough that their credible intervals overlap.

The modeling is supported by an ETL pipeline processing 11.28 million rows across 48 quarterly files from 2010 to 2024. A schema registry handles three PSA column schemas and two education coding systems created by the K-12 transition before a 12-step cleaning process constructs the analytical parent-child dataset.

**Modeling / Analytics:** Bayesian Multilevel Modeling · PyMC · Bambi · ArviZ · Intergenerational Mobility · Statistical Analysis

**Data Preparation:** Python · pandas · PSA LFS Microdata · ETL Pipeline · 11.28M rows

**Repository:** https://github.com/rolanddelarosaph/psa-lfs-educational-mobility-pipeline

---

## Core Skills

| Area | Skills |
|---|---|
| Languages & Core | Python · SQL · R · Statistics |
| Analytics & Modeling | Bayesian Modeling · Forecasting · Statistical Analysis & Modeling · Predictive Modeling |
| Data Analysis & Visualization | pandas · NumPy · Tableau · Power BI |
| Data & Engineering | Snowflake · dbt · ETL/ELT · MySQL · Medallion Architecture |

---

## Contact

Currently open to **Data Analyst** and **Data Scientist** opportunities, especially roles involving statistical analysis, forecasting, predictive modeling, business analytics, and data-driven decision making. I also bring hands-on pipeline and data-modeling experience when the work requires going from raw data to analysis-ready datasets.

**Email:** roland.delarosa.ph@gmail.com

**LinkedIn:** https://www.linkedin.com/in/roland-dela-rosa-5595713b9/

**GitHub:** https://github.com/rolanddelarosaph
