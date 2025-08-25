# 🏥 England Health Index (2020–2021): Service Access, Living Conditions & Life Expectancy

This project explores the **Health Index for England (2020/2021)**—focusing on **Service Access**, **Living Conditions**, and **Life Expectancy** indicators. Using official data from the UK Government's open data repositories, built a full analytics pipeline to uncover regional inequalities and inform health planning decisions.

---

## Project Objectives

- Analyze spatial and temporal patterns in England’s **health service access**, infrastructure, and population health outcomes
- Identify areas with poor access to services and lower life expectancy
- Build a seamless data pipeline from **R to SQL**, with visuals powered by **Looker Studio**
- Empower public health professionals and policymakers with a clear, data-driven view of health equity across England

---

## 🗂 Data Sources

- 📥 **[Health Index for England](https://www.gov.uk/government/statistics/health-index-for-england-2020-to-2021)** (ONS)
- 📥 UK Open Government repositories (`data.gov.uk`)
- Indicators include:
  - Service Access (e.g. GP access, emergency care, transport links)
  - Living Conditions (e.g. housing, crime, pollution)
  - Life Expectancy (regional estimates, trends)

---

## 🔁 Workflow Overview

### 1. **Data Collection & Cleaning**
- Used `readr`, `dplyr`, and `janitor` in **R** for importing and standardizing datasets
- Filtered data by indicator groups and normalized regional names and scores

### 2. **Database Integration**
- Connected R to **BigQuery** using `DBI` and `bigrquery`
- Created structured tables to support multi-dimensional querying by indicator, region, and year

### 3. **Data Exploration & Analysis**
- Performed descriptive and comparative analyses across England’s regions
- Highlighted correlations between service access and life expectancy

### 4. **Dashboard & Visual Analytics**
- Built dynamic visuals in **Looker Studio**
- Enabled filterable views by region, index group, and time
- Included choropleth maps, ranking bars, and year-over-year index trendlines

---

## Tools & Technologies

| Tool/Library     | Purpose                                  |
|------------------|-------------------------------------------|
| **R (tidyverse)**| Data import, wrangling, transformation   |
| **R (bigrquery)**| Create pipeline from R to BQ
| **Big Query**    | Structured data storage, query optimization |
| **Looker Studio**| Interactive dashboard visualizations      |
| **ONS & GOV.UK** | Public health and regional indicator data |

---

> ⚠️ *This project uses open, publicly available data and complies with ONS and UK Government data use policies.*
```


# Visualizing on Looker
Dashboard 1: [Service Access and Life Expectancy](http://lookerstudio.google.com/reporting/3393463b-ee1e-41ef-b67a-4163c4866a40/page/4zkVF)
Dashboard 2: [Service Access and Living Conditions](https://lookerstudio.google.com/reporting/e870f3d8-6dbe-4b9b-8402-3d33867e3433/page/2SlVF)

# Further Reading
Read more details on analysis, insights and implications on [Medium](https://medium.com/@temiloluwa.jokotola/englands-2020-2021-health-index-service-access-living-conditions-and-life-expectancy-0d7ec577fbdf)
