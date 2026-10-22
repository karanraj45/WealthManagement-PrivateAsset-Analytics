# Wealth Management & Private Asset Analytics Platform

## 📌 Executive Summary
An enterprise-grade Business Intelligence platform built for wealth management executives to monitor **Assets Under Management (AUM)**, track fee-based **Revenue generation**, measure **Client Attrition/Churn**, and evaluate **Portfolio Risk Exposure**. 

Designed and engineered from scratch, transforming raw transactional data into high-performance executive decision-making tools.

---

## 🏗️ Architecture & Data Pipeline
1. **Backend Relational Storage (PostgreSQL):** Ingested raw mock brokerage records, structured tables, enforced primary/foreign keys, and normalized data into a clean **Star Schema**.
2. **Data Modeling & Star Schema:**
   - **`Dim_Clients` (Dimension Table):** Stores unique client profiles, risk scores, regions, and business lines.
   - **`Fact_MonthlyAUM` (Fact Table):** Stores time-series transactional metrics, monthly AUM balances, net flows, revenue streams, and binary churn flags.
3. **Data Transformation (Power Query):** Verified data profiling, type safety, and error-free loading.
4. **Data Modeling & DAX (Power BI):** Established a 1-to-Many (`1:*`) relationship model and built custom measures using advanced DAX variables (`VAR`), `DISTINCTCOUNT`, and safe division logic.

---

## 📊 Key Dashboard Features & Visuals
* **Macro Scale & Capital Flows:** Line & Column chart tracking AUM trajectory alongside organic Net Asset Flows over time.
* **Revenue Monetization:** Horizontal bar chart detailing fee yields across business lines (*Retirement, Corporate Services, Equity, Compliance*).
* **Behavioral Attrition Tracking:** Quarterly column chart isolating client churn rate spikes.
* **Risk & Compliance Posture:** Segmented donut chart categorizing active client distribution across *Low, Moderate, and High-Risk* tiers.
* **Dynamic Regional Slicers:** Instant cross-filtering capabilities across geographic regions and custom date ranges.

---

## 🛠️ Tech Stack
* **Database & SQL:** PostgreSQL, Relational Database Design, Star Schema Modeling
* **Data Transformation:** Power Query, ETL Logic
* **DAX & Modeling:** Power BI Desktop, Calculated Columns, Measures, Variables (`VAR`)
* **UI/UX Design:** Executive 16:9 Dark Theme Widescreen UI
