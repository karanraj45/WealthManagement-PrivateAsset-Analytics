# Wealth Management & Private Asset Analytics Platform

## 📌 Executive Summary
An enterprise-grade Business Intelligence platform built for wealth management executives to monitor **Assets Under Management (AUM)**, track fee-based **Revenue generation**, measure **Client Attrition/Churn**, and evaluate **Portfolio Risk Exposure**. 

Designed and engineered from scratch, transforming raw transactional data into high-performance executive decision-making tools.

![Wealth Management Dashboard Preview]
<img width="1197" height="672" alt="dashboard-preview" src="https://github.com/user-attachments/assets/977d4c1b-9acd-4a40-be40-61e2ee088bfd" />

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

## 💡 Executive Insights & Strategic Recommendations

### 1. Revenue Concentration Risk
* **Insight:** Fee-based revenue is heavily skewed toward **Retirement ($258.4M)** and **Corporate Services ($96.1M)**, accounting for over 90% of total revenue yield. Equity and Compliance lines remain severely under-monetized (<$35M combined).
* **Strategic Action:** Restructure advisory fee tiers and deploy targeted cross-selling campaigns to high-AUM clients in the Equity division to diversify revenue streams.

### 2. Capital Flow vs. Market Volatility
* **Insight:** Total AUM peaked above **$4.6T+ in 2022**, strongly supported by organic Net Asset Flows ($8.34B+). However, inflows flattened significantly in 2023 due to macroeconomic headwinds and shifting yield environments.
* **Strategic Action:** Strengthen liquidity buffers and shift wealth advisors toward defensive yield products (e.g., fixed income/money market) during market deceleration phases to prevent capital flight.

### 3. Quarterly Attrition & Churn Patterns
* **Insight:** While overall client churn remains controlled at **13.93%**, quarterly trend analysis revealed sharp localized attrition spikes during Q3 cycles (reaching up to ~3.2% per quarter).
* **Strategic Action:** Implement automated client health tracking in CRM to trigger mandatory relationship manager outreach 30 days prior to Q3 cycle dates.

### 4. Portfolio Compliance & Risk Exposure
* **Insight:** Risk tier segmentation indicates that **~87.5% of active clients (381 accounts)** are categorized in the **High Risk** bracket based on volatility and asset concentration.
* **Strategic Action:** Risk management teams must initiate a portfolio rebalancing audit for high-net-worth accounts to mitigate downside exposure and satisfy regulatory compliance guidelines.
