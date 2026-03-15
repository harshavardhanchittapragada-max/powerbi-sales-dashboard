# 📊 Power BI Sales Dashboard

![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi)
![DAX](https://img.shields.io/badge/DAX-Measures-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Project Overview

An interactive Power BI dashboard built to give business stakeholders a clear view of sales performance — by product, region, and time period — without needing to touch raw data.

**Business Question:** Where are we winning, where are we losing, and what does the trend look like?

---

## 📊 Dashboard Features

| Feature | Detail |
|---|---|
| KPI Cards | Total Revenue, Total Profit, Profit Margin %, Orders Count, Avg Order Value, YoY Growth |
| Slicers | Region, Product Category, Date Range |
| Charts | Monthly trend line, Top 10 products bar chart, Regional map |
| Drill-through | Click any region → see individual product breakdown |
| Forecast | 3-month sales forecast on trend line |

---

## 📈 Key Findings

- Q4 consistently outperformed Q1 by **~22%** — clear seasonal demand pattern
- Profit margins ranged from **4% to 38%** across product categories
- Top 3 products drove **58% of total revenue**
- 2 regions were **30%+ below the sales average** — flagged for review

---

## 🔧 Tech Stack

- **Power BI Desktop** — dashboard design
- **Power Query** — data transformation
- **DAX** — custom measures and KPI calculations
- **Excel** — source data

---

## 💡 DAX Measures Used
```dax
Total Revenue = SUM(Sales[Sales])

Profit Margin % = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Sales])) * 100

YoY Growth % = 
DIVIDE(
    [Total Revenue] - CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Calendar[Date])),
    CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Calendar[Date]))
) * 100
```

---

## 🚀 How to Open

1. Download and install **Power BI Desktop** (free) from microsoft.com
2. Open `sales_dashboard.pbix`
3. Use slicers to filter by region, product, or date

---

## 💡 What I Learned

- A dashboard is only useful if non-technical users can operate it — slicers and clear labels matter
- DAX measures are far more flexible than calculated columns for dynamic KPIs
- Data model relationships must be set correctly before any measure works properly

---

## 📬 Connect

**Harsha Vardhan Chittapragada**
[LinkedIn](https://linkedin.com/in/harshavardhanchittapragada) · [GitHub](https://github.com/harshavardhanchittapragada-max)
