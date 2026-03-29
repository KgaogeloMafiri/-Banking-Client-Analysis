# 🏦 Banking Client Analysis — EDA & Power BI Dashboard

![Python](https://img.shields.io/badge/Python-0C1B33?style=flat-square&logo=python&logoColor=0EA5A0)
![Power BI](https://img.shields.io/badge/Power%20BI-0C1B33?style=flat-square&logo=powerbi&logoColor=F2C811)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0C1B33?style=flat-square&logo=postgresql&logoColor=0EA5A0)
![Pandas](https://img.shields.io/badge/Pandas-0C1B33?style=flat-square&logo=pandas&logoColor=0EA5A0)
![Status](https://img.shields.io/badge/Status-In%20Progress-F59E0B?style=flat-square)

---

## 📌 Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on a banking client dataset of 3,000 clients across 25 variables — covering demographics, financial products, income, risk profiles, and loyalty classifications. The insights from the EDA will feed directly into an interactive Power BI dashboard for business intelligence reporting.

---

## 🗂️ Dataset

| Property | Detail |
|---|---|
| Records | 3,000 clients |
| Columns | 25 |
| Source | Banking.csv |
| Date Range | 2001 – 2024 |

**Key Variables:**

- **Demographics** — Age, Nationality, Occupation, Gender
- **Financial Products** — Bank Loans, Bank Deposits, Credit Card Balance, Business Lending, Saving & Checking Accounts, Foreign Currency Account
- **Client Profile** — Loyalty Classification, Fee Structure, Risk Weighting, Properties Owned
- **Other** — Estimated Income, Superannuation Savings, Date Joined

---

## 📁 Project Structure

```
banking-client-analysis/
│
├── data/
│   └── Banking.csv                  # Raw dataset
│
├── eda/
│   └── banking_eda.py               # Full EDA Python script
│
├── charts/
│   ├── 01_missing_values.png
│   ├── 02_distributions.png
│   ├── 07_correlation_heatmap.png
│   └── 09_outliers.png
│
├── sql/
│   └── banking_table.sql            # pgAdmin table creation & import scripts
│
├── dashboard/
│   └── banking_dashboard.pbix       # Power BI dashboard (coming soon)
│
└── README.md
```

---

## 🔍 EDA Sections

| # | Section | Description |
|---|---|---|
| 1 | Data Overview | Shape, dtypes, null counts, duplicates, descriptive stats |
| 2 | Missing Values | Heatmap of null values across all columns |
| 3 | Distributions | Histograms for all 9 financial variables |
| 4 | Correlation | Heatmap of all numeric variable correlations |
| 5 | Outlier Detection | Box plots with IQR method across 6 financial columns |
| 6 | Summary Report | Full printed EDA summary with key statistics |

---

## 📊 Power BI Dashboard *(Coming Soon)*

The dashboard will be built on top of the cleaned dataset loaded into **PostgreSQL** and will include the following pages:

- **Executive Overview** — KPI cards, total clients, avg income, deposits and loans
- **Client Demographics** — Nationality, age groups, occupation breakdown
- **Income & Loyalty Analysis** — Income by loyalty tier and fee structure
- **Financial Products** — Loans, deposits, credit cards and business lending breakdown
- **Risk Profile** — Risk weighting distribution and relationship with financial metrics
- **Client Acquisition** — Time series of new clients joined per year

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python (Pandas, NumPy) | Data loading, cleaning, wrangling |
| Matplotlib & Seaborn | Data visualisation and EDA charts |
| SciPy | Statistical analysis |
| PostgreSQL / pgAdmin | Database storage and SQL queries |
| Power BI | Interactive dashboard (in progress) |
| DAX | Dashboard measures and KPIs |


---

## 🗄️ Database Setup (pgAdmin)

To load the data into PostgreSQL:

1. Open **pgAdmin** and connect to your database
2. Run `sql/banking_table.sql` to create the table
3. Import `Banking.csv` using the pgAdmin Import Tool
4. Use `SET datestyle = 'DMY'` to handle the date format correctly

---

## 📈 Key Findings *(Preview)*

- 🌍 The dataset covers clients from **multiple nationalities** with varying income and product profiles
- 💰 Significant variation in **estimated income** across loyalty tiers and fee structures
- ⚠️ Outliers detected in **Bank Loans** and **Business Lending** — indicative of high-value clients
- 📅 Client acquisition shows interesting **growth trends** over the 2001–2024 period
- 🔗 Strong correlations found between **Bank Deposits**, **Checking Accounts**, and **Saving Accounts**

---

## 🚧 Status & Roadmap

- [x] Data loaded into PostgreSQL
- [x] EDA completed — 9 charts generated
- [x] Data cleaning & feature engineering
- [ ] Power BI dashboard — in progress
- [ ] DAX measures and KPIs
- [ ] Final insights report

---

## 👤 Author

**Kgaogelo Mafiri**
Geophysicist & Aspiring Data Analyst | South Africa 🇿🇦

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0C1B33?style=flat-square&logo=linkedin&logoColor=0EA5A0)](https://www.linkedin.com/in/kgaogelo-mafiri-608613124/)
[![GitHub](https://img.shields.io/badge/GitHub-0C1B33?style=flat-square&logo=github&logoColor=0EA5A0)](https://github.com/KgaogeloMafiri)

---

<p align="center">💡 Turning banking data into actionable insights | South Africa 🇿🇦</p>
