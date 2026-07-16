# Kenya Inflation Impact on SMEs & Households
## Google Data Analytics Certificate — Capstone Project

**Author:** Carsons Ochieng Ooko  
**Date:** July 2026  
**Tools:** Excel | Google BigQuery (SQL) | R (Kaggle) | Tableau Public

---

## Business Question
Which expense categories have driven inflation the most in Kenya over the 
past 29 months (January 2024 – May 2026), and what does this mean for how 
SMEs should adjust their budgets, pricing, and wage decisions?

---

## Client & Stakeholders
- **Client:** HR & Finance advisory consultancy launching an inflation-impact 
  advisory service for SME clients
- **Stakeholders:** SME owners, finance managers, employees affected by 
  cost-of-living changes

---

## Data Source
**Kenya National Bureau of Statistics (KNBS)** — Monthly Consumer Price 
Index (CPI) Reports, January 2024 – May 2026 (29 months).

- Primary government statistical agency (ISO 9001:2015 certified)
- Base period: February 2019 = 100
- Coverage: Urban areas across 50 data collection zones nationwide
- Downloaded from: https://www.knbs.or.ke/download-category/consumer-price-indices-cpi/

---

## Project Structure

```
kenya-inflation-sme-capstone/
├── 01_raw_data/          # Source KNBS PDF reports
├── 02_cleaned_data/      # Cleaned CSV files
├── 03_sql/               # BigQuery SQL queries
├── 04_analysis/          # Exported analysis tables
└── 06_report/            # Final report and documentation
```
---

## Tools & Process
| Phase | Tool | Output |
|---|---|---|
| Ask | — | Business task statement |
| Prepare | KNBS PDFs → Excel | Raw data transcription |
| Process | Excel + BigQuery | 2 clean CSVs, 7 SQL queries |
| Analyze | R on Kaggle | 4 charts + budget model |
| Share | Tableau Public | Interactive dashboard |
| Act | GitHub | Portfolio + recommendations |

---

## Key Findings

**Finding 1 — Non-core inflation averaged 3× core inflation**
Non-core inflation (food and fuel) averaged 9.11% over the period vs core 
inflation at 2.78%. Kenya's headline inflation averaged 4.43%, ranging from 
2.7% (Oct 2024) to 6.9% (Jan 2024). Most inflation pain was driven by 
volatile food and energy prices, not broad structural economic pressure.

**Finding 2 — Food & Beverages is the single biggest inflation driver**
With an average YoY inflation of 6.7% and the largest basket weight (32.9%), 
Food and Non-Alcoholic Beverages contributed more to overall inflation than 
any other category. Transport (4.81%, 9.6% weight) was second most impactful.

**Finding 3 — A fixed KSh 100,000 SME budget never returned to baseline**
Applying actual KNBS division-level inflation to a modelled SME budget, the 
equivalent cost of a KSh 100,000 January 2024 budget never fell back to 
KSh 100,000 at any point across 29 months. Even at the most favourable point 
(October 2024) the same basket cost KSh 101,805. By May 2026 costs were 
rising sharply again.

---

## Recommendations
1. SMEs should review pricing structures at least every 6 months — annual 
   reviews are insufficient given the volatility shown in this data
2. Food-heavy businesses (restaurants, caterers, retailers) should explore 
   supplier contracts that lock in prices for 3–6 months to hedge against 
   food inflation spikes
3. Transport cost savings (route optimization, bulk fuel purchasing) can 
   meaningfully offset the 4.81% average transport inflation
4. Core inflation stability (2.78% avg) suggests wage adjustments of 3–4% 
   annually remain reasonable for service-sector SMEs

---

## Portfolio Links
- **R Analysis Notebook (Kaggle):** https://www.kaggle.com/code/carsonsooko/version-1-full-analysis-complete1
- **Interactive Dashboard (Tableau Public):** https://public.tableau.com/app/profile/carsons.ooko/viz/KenyaInflationSMEDashboard/Dashboard#1
- **Dataset (Kaggle):** https://www.kaggle.com/datasets/carsonsooko/kenya-cpi-inflation-data-2024-2026

---

## Suggested Next Steps
- Add county-level CPI data for regional comparison when KNBS publishes it
- Merge with KNBS wage/earnings data to compute real inflation-adjusted 
  wage growth
- Layer in CBK exchange rate data to quantify how much inflation is 
  imported (fuel, forex-priced goods)
- Extend the dataset monthly as new KNBS reports are published

---

*This project was completed as part of the Google Data Analytics Professional 
Certificate capstone requirement. All data sourced directly from KNBS official 
monthly reports.*
