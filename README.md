# 🛒 Maven Market — Retail Performance Dashboard (Power BI)

### 🚀 Executive Summary
**Goal:** Build a three-page Power BI report that lets a retail operations team monitor performance against monthly targets across 24 stores in the USA, Canada and Mexico.
**Role:** BI Developer.
**Tools:** Power BI Desktop (star-schema data model, DAX measures, KPI cards with goals, drill-through, cross-filtering).

---

## 📖 The Story
Maven Market runs stores across three countries and sells hundreds of branded products. Leadership had the transaction data but no way to answer the two questions that actually matter month to month: **are we hitting target, and where specifically are we missing?**

I built a report that answers both in one screen — headline KPIs against goal at the top, then the store, brand and product breakdowns that explain the number underneath.

---

## 📊 The Dashboard

### 1. Topline Performance
![Topline performance page](Maven%20market%20Topline%20Performance.png)

Current-month transactions, profit and returns, each shown against its goal with a sparkline for trend. Brand-level table on the left ranks all 30 product brands by transactions, profit, profit margin and return rate, with conditional formatting so weak margins and high return rates surface without reading numbers. Country slicers and a revenue-vs-target gauge complete the view.

**What it shows:** 41,012 transactions and $155,752 profit at a 59.31% blended margin. Current month beat both the transaction goal (+5.69%) and the profit goal (+5.61%), but returns came in 2.9% over target — growth is being partly given back.

### 2. Store Performance
![Store performance page](Maven%20Market%20Store%20performance.png)

Store-level view: a scatter of transactions against return rate with reference lines at the mean, so under-performers and high-return stores fall into readable quadrants. Treemap sizes each country by store count; the monthly revenue trend runs alongside.

**What it shows:** Store 12 is the top generator. Revenue is flat around $95–100K for most of the year then climbs sharply from October, a seasonality pattern targets should account for. Stores 20 and 23 sit in the worst quadrant — low volume *and* the highest return rates in the estate.

### 3. Product Effect
![Product effect page](Maven%20market%20product%20Effect.png)

Product attribute analysis — top sellers by fat content, recyclability and membership tier, with matrices crossing those attributes against child status and transaction volume.

**What it shows:** Low-fat products account for 35.27% of transactions and $420,753 of revenue. Bronze members drive 56.3% of all transactions, which reframes the loyalty programme: the entry tier is the volume tier, not Golden.

---

## 🛠️ Technical Skills Demonstrated
* **Data modelling:** Star schema across transactions, products, stores, customers and calendar with correctly-defined relationships.
* **DAX:** Current-month measures, goal comparisons, profit margin and return-rate calculations, time intelligence for weekly and monthly trending.
* **KPI design:** Cards with explicit goals and variance rather than bare totals — the number always arrives with its context.
* **Interactivity:** Country slicers, cross-filtering between visuals, and page navigation so one report serves executive and operational readers.
* **Visual selection:** Scatter with mean reference lines for outlier detection, treemap for part-to-whole, gauge for single-target tracking.

---

## 🗂️ Repository Contents

| File | What it is |
|---|---|
| `MavenMarket_Report.pbix` | The Power BI report — open in Power BI Desktop |
| `Maven market Topline Performance.png` | Page 1 screenshot |
| `Maven Market Store performance.png` | Page 2 screenshot |
| `Maven market product Effect.png` | Page 3 screenshot |

---

## 📊 Future Improvements
* **Returns root cause:** Stores 20 and 23 have the highest return rates in the estate — a drill-through page linking returns to specific products and brands would turn the observation into an action.
* **Rolling forecast:** Add a forecast line to the monthly revenue trend so targets can be set from the seasonality rather than flat.
* **Row-level security:** Restrict store managers to their own store to make the report distributable.

---

### 👋 About Me
Data Analyst based in **Manchester, UK**, working in **SQL, Excel, Tableau and Power BI**.
[LinkedIn](https://www.linkedin.com/in/ibomeno-basiekanem/) · [Portfolio](https://thelordbass.github.io/)
