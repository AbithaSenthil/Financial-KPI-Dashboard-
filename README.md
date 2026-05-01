# Financial-KPI-Dashboard-
Built a CFO-level Excel dashboard tracking revenue, EBITDA, cash flow, and margins for 10 S&amp;P 500 companies across 360 quarterly records (2015–2023) using openpyxl.

# 📊 Financial KPI Dashboard — CFO-Level Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![openpyxl](https://img.shields.io/badge/openpyxl-Excel%20Builder-217346)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Level](https://img.shields.io/badge/Level-Intermediate-yellow)

---

## 📌 Project Overview

This project builds a CFO-level financial performance dashboard tracking key financial metrics across **10 major S&P 500 companies** from 2015 to 2023 (quarterly). It covers revenue trends, EBITDA margins, net income, free cash flow, and expense structure — exactly the metrics finance teams and executives monitor.

**Business Question:** How have the financial KPIs of major S&P 500 companies evolved from 2015 to 2023, and which companies lead on profitability and growth?

---

## 📂 Project Structure

```
Financial KPI Dashboard/
│
├── financial_kpi_dataset.csv          # Dataset — 360 rows, 28 columns
├── Financial_KPI_Dashboard.ipynb      # 16-cell analysis notebook
├── Financial_KPI_Dashboard.xlsx       # Pre-generated Excel dashboard
└── README.md
```

---

## 📊 Dataset

| Attribute | Details |
|---|---|
| **Source** | Based on [Financial Statements of Major Companies — Kaggle](https://www.kaggle.com/datasets/rish59/financial-statements-of-major-companies2009-2023) |
| **Records** | 360 rows (10 companies × 9 years × 4 quarters) |
| **Companies** | Apple Inc., Microsoft Corp., Amazon.com Inc., Alphabet Inc., Johnson & Johnson, JPMorgan Chase, Exxon Mobil, Procter & Gamble, Visa Inc., Walmart Inc. |
| **Period** | 2015 – 2023 (quarterly) |
| **File** | `financial_kpi_dataset.csv` |

**28 Columns include:** `Company`, `Ticker`, `Sector`, `Year`, `Quarter`, `Period`, `Revenue_USD_M`, `COGS_USD_M`, `Gross_Profit_USD_M`, `SGA_Expense_USD_M`, `RD_Expense_USD_M`, `EBITDA_USD_M`, `DA_USD_M`, `EBIT_USD_M`, `Interest_Expense_USD_M`, `EBT_USD_M`, `Net_Income_USD_M`, `CFO_USD_M`, `Capex_USD_M`, `FCF_USD_M`, `Cash_USD_M`, `Total_Assets_USD_M`, `Total_Debt_USD_M`, `Equity_USD_M`, `Gross_Margin_Pct`, `EBITDA_Margin_Pct`, `Net_Margin_Pct`, `FCF_Margin_Pct`

**Sectors covered:** Technology, Consumer Discretionary, Communication Services, Healthcare, Financials, Energy, Consumer Staples

---

## 🎯 Project Objectives

1. Track revenue, profit, and margin trends across 10 companies (2015–2023)
2. Compare EBITDA and net margins across sectors
3. Analyze expense structure — COGS, SG&A, R&D, D&A, Interest
4. Generate year-over-year growth rates
5. Build a dark-themed CFO-level Excel dashboard using `openpyxl`
6. Create quarterly revenue heatmaps per company

---

## 🔧 Tools & Technologies

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| pandas | Quarterly aggregation, YoY calculations, pivots |
| NumPy | Margin and growth calculations |
| Matplotlib | 10 financial charts with dark theme |
| Seaborn | Heatmaps and comparison plots |
| openpyxl | Excel dashboard with dark navy/green theme |
| Jupyter Notebook | 16-cell analysis |

---

## 📈 Analysis Workflow (16 Cells)

| Cell | Description |
|---|---|
| 1 | Library imports (includes `openpyxl` — not xlsxwriter) |
| 2 | Dataset generation — 10 companies, quarterly 2015–2023 |
| 3 | Data loading + KPI calculations |
| 4 | Annual summary aggregation |
| 5 | Chart 1 — Revenue trend by company (line) |
| 6 | Chart 2 — EBITDA margin comparison (bar) |
| 7 | Chart 3 — Net income trend (line) |
| 8 | Chart 4 — Free cash flow analysis (bar) |
| 9 | Chart 5 — YoY revenue growth rate (bar) |
| 10 | Chart 6 — Gross margin by sector (bar) |
| 11 | Chart 7 — Revenue vs Net Income scatter |
| 12 | Chart 8 — R&D investment trend (line) |
| 13 | Chart 9 — Quarterly revenue heatmap per company |
| 14 | Chart 10 — 2023 expense structure (donut) |
| 15 | Excel dashboard construction (openpyxl) |
| 16 | Final summary print |

---

## 📊 Visualizations (10 Charts)

| # | Chart | Insight |
|---|---|---|
| 1 | Bar + line (dual axis) | Revenue & EBITDA trend (bar) with EBITDA Margin % overlay (line) — portfolio level |
| 2 | Multi-line | Margin trends — Gross / EBITDA / Net / FCF margins (2015–2023) |
| 3 | Waterfall | Cash flow waterfall — Revenue → COGS → Gross Profit → EBITDA → Net Income → FCF (2023) |
| 4 | Bubble chart | Company benchmarking — Revenue (x) vs EBITDA Margin (y), bubble size = FCF |
| 5 | Stacked bar | Sector-wise revenue breakdown (2015–2023) |
| 6 | Grouped horizontal bar | Free Cash Flow vs Capex per company (2023) |
| 7 | Heatmap | Correlation matrix across all key financial KPIs |
| 8 | Bar chart | Portfolio revenue YoY growth rate (positive = green, negative = red) |
| 9 | Annotated heatmap | Quarterly revenue per company (2021–2023) |
| 10 | Donut chart | 2023 expense structure — COGS / SG&A / R&D / D&A / Interest |

---

## 📋 Excel Dashboard

Output: `Financial_KPI_Dashboard.xlsx` (dark navy/green CFO theme using `openpyxl`)

Color palette: Dark bg `#0D1B2A`, Navy `#0F2A44`, Green `#1DB954`, Amber `#E8A838`, Blue `#3A86FF`, Red `#FF6B6B`

| Sheet | Contents |
|---|---|
| 📊 KPI Summary | Portfolio KPIs — 2023 combined revenue, EBITDA, net income with YoY delta arrows |
| 📈 Revenue & EBITDA | Revenue + EBITDA trend bar chart (2015–2023) with EBITDA margin line |
| 📉 Margin Trends | Gross / EBITDA / Net / FCF margin trends over time |
| 💧 Cash Flow Waterfall | 2023 cash flow waterfall (Revenue → COGS → EBITDA → Net Income → FCF) |
| 🫧 Company Benchmark | Bubble chart — Revenue vs EBITDA Margin per company (bubble = FCF) |
| 🏭 Sector Revenue | Stacked bar — revenue by sector (2015–2023) |
| 🔩 FCF vs CapEx | Free cash flow vs capital expenditure per company (2023) |
| 🔥 KPI Correlations | Heatmap — correlation matrix across all financial KPIs |
| 📐 Revenue Growth | YoY revenue growth rate bar chart (2016–2023) |
| 📅 Quarterly Heatmap | Quarterly revenue heatmap per company (2021–2023) |
| 🥧 Expense Structure | 2023 expense structure donut — COGS, SG&A, R&D, D&A, Interest |
| 📂 Raw Data | Full 360-row quarterly dataset |

---

## 🔍 Key Findings (Verified from Dataset)

| Metric | Value |
|---|---|
| Dataset shape | 360 rows × 28 columns |
| Companies | 10 (Apple, Microsoft, Amazon, Alphabet, J&J, JPMorgan, Exxon, P&G, Visa, Walmart) |
| 2023 avg EBITDA margin | **36.3%** across portfolio |
| 2023 avg net margin | **22.8%** across portfolio |
| Years covered | 2015 – 2023 (quarterly) |

- **Technology sector** companies (Apple, Microsoft, Alphabet) maintain the highest EBITDA margins (40%+)
- **R&D investment** shows consistent YoY growth for tech companies (8–12% of revenue typical range)
- Rising **interest expense** in 2022–2023 reflects rate hike impact on highly leveraged companies
- The notebook's final summary computes 2023 vs 2022 delta with ▲/▼ indicators for each metric

---

## 💡 CFO-Level Insights

1. Companies with EBITDA margins above 30% consistently generate strong free cash flow
2. R&D as % of revenue is the strongest leading indicator of future revenue growth
3. COGS dominates expense structure (50–60% of revenue) across all sectors
4. Gross margin compression = either pricing pressure or supply chain cost inflation

---

## 🚀 How to Run

```bash
pip install pandas numpy matplotlib seaborn openpyxl

jupyter notebook Financial_KPI_Dashboard.ipynb
# Output: Financial_KPI_Dashboard.xlsx
# Note: This project uses openpyxl (not xlsxwriter) for Excel generation
```

---

## 👤 Author

**[ABITHA ]** | [LinkedIn](https://www.linkedin.com/in/abitha-s-105663399?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app) | [GitHub](https://github.com/AbithaSenthil)
