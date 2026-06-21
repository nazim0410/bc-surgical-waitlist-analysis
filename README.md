# BC Surgical Waitlist Analysis
### Trends, Capacity & Regional Equity (2009–2025)

**Author:** Mohammad Nazim Rehman  
**[View Interactive Tableau Dashboard →](https://public.tableau.com/app/profile/mohammad.nazim.rehman/viz/Project1_17820069097990/BCSurgicalWaitlistAnalysisTrendsCapacityRegionalEquity20092025)**

---

## Project Overview

British Columbia's surgical waitlist has grown substantially over the past 15 years, with the COVID-19 pandemic causing lasting disruption to surgical service delivery. This project analyzes **55,024 records** spanning **16 fiscal years (2009/10–2024/25)** across BC's 6 health authorities and 83 procedure types to answer four key questions:

1. How has the provincial surgical waitlist changed since 2009?
2. What was the impact of COVID-19 on wait times, and has the system recovered?
3. Are there regional disparities in surgical access across BC's health authorities?
4. Which procedures place the greatest burden on the system?

The findings support evidence-based resource allocation and surface a significant regional equity gap with direct implications for healthcare planning and policy.

---

## Key Findings

| Finding | Detail |
|---|---|
| **Waitlist Growth** | Grew 34.5% over 15 years — from 72,120 (2009/10) to 97,046 cases (2023/24) |
| **COVID-19 Impact** | 90th percentile wait peaked at 32.6 weeks; system still 21% above pre-COVID baseline |
| **Regional Equity Gap** | Northern Health patients wait **54% longer** (42.4 weeks) than Fraser Health patients (27.6 weeks), despite far fewer cases |
| **Highest Volume Procedure** | Cataract Surgery — 17,523 cases waiting |
| **Longest Wait Procedure** | Tympanoplasty — 72 weeks (90th percentile) |
| **Dual-Burden Procedures** | Knee & Hip Replacement rank in top 10 for both volume AND wait time |

---

## Dashboard Preview

![Provincial Trend](01_provincial_trend.png)
*Provincial waitlist and wait time trends, 2009–2025, with COVID-19 period highlighted*

![Health Authority Comparison](02_health_authority.png)
*Cases waiting by health authority, 2024/25*

![Procedure Analysis](03_procedure_analysis.png)
*Top 10 procedures by case volume and by longest wait time*

![COVID Impact](04_covid_impact.png)
*Pre-COVID, COVID, and post-COVID period comparison*

**[→ Explore the full interactive dashboard on Tableau Public](https://public.tableau.com/app/profile/mohammad.nazim.rehman/viz/Project1_17820069097990/BCSurgicalWaitlistAnalysisTrendsCapacityRegionalEquity20092025)**

---

## Methodology

1. **Data Cleaning** — Standardized column names, converted data types, removed null aggregate rows
2. **Segmentation** — Split data into 4 analytical views: provincial trend, health authority comparison, procedure-level detail, and quarterly trend
3. **Exploratory Analysis** — Conducted trend analysis, regional comparison, and period-over-period (pre/during/post-COVID) analysis in Python
4. **Visualization** — Built 4 static charts in Python (Matplotlib/Seaborn) and an interactive 4-panel dashboard in Tableau Public

---

## Data Source

[BC Ministry of Health — Surgical Patient Registry (Open Data)](https://catalogue.data.gov.bc.ca/dataset/bc-surgical-wait-times)  
Published by the Government of British Columbia. Data covers fiscal years 2009/10 to present, updated quarterly and annually.

---

## Repository Contents
bc-surgical-waitlist-analysis/
├── bc_surgical_analysis.ipynb        — Full analysis notebook with interpretation
├── 01_provincial_trend.png           — Provincial trend chart
├── 02_health_authority.png           — Health authority comparison chart
├── 03_procedure_analysis.png         — Procedure burden analysis chart
├── 04_covid_impact.png               — COVID-19 impact comparison chart
├── tableau_01_provincial_trend.csv   — Cleaned data: provincial trend
├── tableau_02_health_authority.csv   — Cleaned data: health authority detail
├── tableau_03_procedures.csv         — Cleaned data: procedure detail
├── tableau_04_quarterly.csv          — Cleaned data: quarterly trend
├── tableau_05_ha_latest.csv          — Cleaned data: HA snapshot (latest year)
└── README.md
---

## Tools Used

**Python** (Pandas, NumPy, Matplotlib, Seaborn) — data cleaning, exploratory analysis, statistical summarization  
**Tableau Public** — interactive dashboard design and data storytelling

---

## Conclusion & Policy Implications

1. **Capacity gap, not just COVID recovery** — Waitlist growth reflects a structural issue that predates and outlasts the pandemic
2. **Regional equity requires targeted investment** — The 54% wait time gap between Northern and Fraser health authorities reflects unequal resource distribution, not demand differences
3. **Dual-burden procedures need priority** — Knee and Hip Replacement surgeries strain the system on both volume and wait time dimensions

---

*This is an independent analysis using publicly available open government data, conducted for educational and portfolio purposes.*
