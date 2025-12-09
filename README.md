# 📊 Mobile Sales Dashboard

A concise Power BI project that visualizes mobile sales performance across cities, brands, models, and time. The repo contains a one-page dashboard and multi-page reports for Month-To-Date (MTD) and Year‑over‑Year (YoY) analysis.

---

## Project Pages

### 1. Dashboard (Single page)

* KPIs: Total Sales, Total Quantity, Transactions, Average Price
* City-wise sales map
* Monthly quantity trend
* Customer ratings summary
* Payment method distribution
* Brand & model performance
* Day-wise sales trend

### 2. MTD Report

* Daily cumulative month-to-date sales chart
* Filters: Year / Quarter / Month / Day

### 3. Same Period Last Year (YoY)

* Year-over-year comparison (Year / Quarter / Month)
* Detailed table by Year → Quarter → Month → Day

---

## Files

* `mobile_sales_dashboard.pbix` — Power BI Desktop file (main report)
* `data/` — raw or sample datasets (CSV / Excel)
* `docs/` — screenshots and notes

> Replace filenames above with actual file names you upload to the repository.

---

## Key Measures & Modeling (examples)

* `Total Sales` = SUM(sales)
* `Total Quantity` = SUM(quantity)
* `Transactions` = DISTINCTCOUNT(transaction_id)
* `Avg Price` = DIVIDE([Total Sales], [Total Quantity])
* `MTD Sales` = TOTALMTD([Total Sales], 'Date'[Date])
* `Same Period Last Year` = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))

(Adjust measure names to match your PBIX.)

---

## How to run

1. Open the `.pbix` file in **Power BI Desktop**.
2. Refresh data if you provided external data files.
3. Use slicers and filters on the report to explore metrics.

---

## Purpose

This dashboard is built to monitor business performance, track current month progress, and measure growth versus the same period last year. It is suitable for sales managers and product analysts.

---




