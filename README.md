# 📊 P&L Analytics Dashboard — Contoso Corporation

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Finance](https://img.shields.io/badge/Finance%20%26%20Analytics-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

---

## 📌 Overview

A fully interactive, multi-page **Power BI P&L Analytics Dashboard** built for Contoso Corporation's Finance & Analytics team. This dashboard delivers a comprehensive view of financial performance across three dedicated report pages — providing decision-makers with real-time insights into revenue, costs, profitability, and budget attainment.

---

## 🖥️ Dashboard Pages

### 1️⃣ Executive Summary
High-level financial KPIs and trend analysis for quick business performance assessment.

- Total Revenue, COGS, Gross Profit, Total OpEx, and Net Profit KPI cards
- Monthly Revenue Trend (area chart)
- Revenue vs COGS vs Net Profit — Monthly comparison
- Top Revenue Accounts breakdown (donut chart)
- Segment Profitability by Net Profit (bar chart)
- Year-on-Year Comparison — Revenue, Gross Profit & Net Profit

### 2️⃣ Segment Analysis
Deep dive into segment-level performance and expense tracking.

- Revenue by Segment — Monthly (stacked bar chart)
- Expense Breakdown — Monthly (COGS, OpEx, Interest Tax)
- Revenue vs Budget — Monthly tracking
- EBIT Margin Contribution by Segment (donut chart)
- Working Capital — Monthly (Current Assets vs Current Liabilities)

### 3️⃣ P&L Statement
Full structured Profit & Loss statement with detailed variance analysis.

- Year to Date, Actual, and Budget columns
- Budget Attainment % per line item
- Last Month figures with LM Variance %
- Last Year figures with LY Variance %
- Drill-down capability across P&L categories

---

## 📈 Key Metrics (2025)

| Metric | Value |
|--------|-------|
| Total Revenue | 7M |
| Total COGS | 3M |
| Gross Profit | 3M |
| Total OpEx | 749K |
| Net Profit | 2M |
| Top Segment | Products (48.48% EBIT) |
| Budget Attainment | ~91% |

---

## ⚙️ Features

- ✅ Dynamic slicers — filter by **Year**, **Month**, and **Segment**
- ✅ Synced slicers across all three report pages
- ✅ Year-over-Year performance comparison (2024 vs 2025)
- ✅ Budget attainment tracking with percentage formatting
- ✅ Drill-down enabled P&L table with expandable categories
- ✅ Monthly trend analysis across all key financial metrics
- ✅ Working capital monitoring
- ✅ Segment profitability and EBIT margin contribution

---

## 🗂️ Data Model

The dashboard is built on the following key data tables:

- **Fact Table** — Sales transactions with revenue, COGS, and expense data
- **Date Table** — Full calendar table enabling time intelligence functions
- **Segment Table** — Products, Services, Subscriptions
- **Budget Table** — Monthly budget figures per account and segment
- **Account Table** — Chart of accounts with P&L hierarchy (Level_02)

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Power BI Desktop | Dashboard development |
| DAX | Measures and calculated columns |
| Power Query | Data transformation and cleaning |
| Excel / CSV | Source data |

---

## 📐 DAX Measures Used

```dax
-- Total Revenue
Total Revenue = SUM(FactSales[Revenue])

-- Gross Profit
Gross Profit = [Total Revenue] - [Total COGS]

-- Net Profit
Net Profit = [EBIT] - [Interest & Tax]

-- Budget Attainment %
Budget Attainment % = DIVIDE([Monthly Actual], [Monthly Budget])

-- YOY Revenue Variance
YOY Revenue % = DIVIDE([Total Revenue] - [LY Revenue], [LY Revenue])

-- LM Variance %
LM Var % = DIVIDE([Monthly Actual] - [Last Month Actual], [Last Month Actual])
```

---

## 📁 Repository Structure

```
📦 PL-Analytics-Dashboard
 ┣ 📂 Data
 ┃ ┣ 📄 FactSales.csv
 ┃ ┣ 📄 BudgetData.csv
 ┃ ┗ 📄 AccountMaster.csv
 ┣ 📂 Screenshots
 ┃ ┣ 🖼️ Executive_Summary.png
 ┃ ┣ 🖼️ Segment_Analysis.png
 ┃ ┗ 🖼️ PL_Statement.png
 ┣ 📄 PL_Analytics_Dashboard.pbix
 ┣ 📄 README.md
 ┗ 📄 LICENSE
```

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) — latest version recommended

### Steps to Run
1. Clone this repository
```bash
git clone https://github.com/yourusername/PL-Analytics-Dashboard.git
```
2. Open **PL_Analytics_Dashboard.pbix** in Power BI Desktop
3. If prompted, update the data source path to your local **Data** folder
4. Click **Refresh** to load the latest data
5. Use the **Year**, **Month**, and **Segment** slicers to explore the dashboard

---

## 📷 Screenshots

### Executive Summary
![Executive Summary](Screenshots/Executive_Summary.png)

### Segment Analysis
![Segment Analysis](Screenshots/Segment_Analysis.png)

### P&L Statement
![P&L Statement](Screenshots/PL_Statement.png)

---

## 🎥 Dashboard Walkthrough

> A full video walkthrough of this dashboard is available on LinkedIn.
> 📺 [Watch the Demo](https://www.linkedin.com/in/yourprofile)

---

## 🙋 About the Author

Built by **Charuka** — Finance & Analytics Professional

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yourusername)

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

*If you found this project helpful, please consider giving it a ⭐ on GitHub!*
