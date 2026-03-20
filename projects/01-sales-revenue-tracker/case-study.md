# 📁 Project 01 — Sales & Revenue Tracker (FY 2024)

**Role:** Remote Data Entry Clerk  
**Tools:** Microsoft Excel  
**Date:** March 2026  
**File:** [Download Sales_Revenue_Tracker_FY2024.xlsx](./Sales_Revenue_Tracker_FY2024.xlsx)

---

## Background

A mid-sized Kenyan business operating across four regions — Nairobi, Mombasa, Kisumu, and Nakuru — needed its full year of sales transactions organised, cleaned, and reported in a structured format. The company had raw sales activity across four representatives and three product categories (Electronics, Furniture, and Accessories), but no centralised, formula-driven tracker to make sense of it all.

A remote data entry clerk was brought in to handle the end-to-end data management task.

---

## The Problem

The business faced a common operational challenge — data existed but was not usable. Specifically:

- Transaction records were scattered with no consistent structure
- There was no automated way to calculate revenue after discounts
- Leadership had no visibility into which region, rep, or product category was driving the most revenue
- There was no verification process to catch errors before the data reached decision-makers

---

## What I Did

### 1. Data Entry & Organisation
All 26 sales transactions were entered into a clean, structured spreadsheet — each record capturing the Order ID, date, sales rep, region, product, category, units sold, and unit price. Nothing was left blank or inconsistent.

### 2. Formula Building
Rather than hardcoding calculated values, live Excel formulas were used throughout. Gross revenue, net revenue after discount, regional breakdowns, and rep-level summaries all calculate in real time — meaning the file updates automatically if any input changes.

### 3. Data Verification
A dedicated verification log was produced documenting 10 quality checks — covering duplicate detection, date range validation, formula accuracy, discount consistency, and a final tie-out between the raw data and the summary dashboard. Every check passed.

### 4. Reporting & Formatting
A summary dashboard was built on top of the raw data, giving management instant visibility into KPIs — total orders, total revenue, performance by region, by category, and by sales rep — all without touching the source data.

---

## Tools & Formulas Used

| Formula | Purpose |
|---|---|
| `=G4*H4` | Gross Revenue (Units × Unit Price) |
| `=I4*(1-J4)` | Net Revenue after discount |
| `=SUMIF(...)` | Revenue totals by Region, Category, Rep |
| `=COUNTIF(...)` | Order counts by Region, Category, Rep |
| `=IF(B8=0,0,D8/B8)` | Average Net Revenue per Order |

---

## The Output

A fully self-contained, three-sheet Excel workbook:

| Sheet | Contents |
|---|---|
| **Sales Data** | 26 entered records with live Gross & Net Revenue formulas |
| **Summary Dashboard** | KPI cards, revenue by region, category, and sales rep |
| **Verification Log** | 10-point quality check — all passed ✔ |

---

## Real-World Value

This is exactly the kind of task businesses outsource to remote data clerks daily. The value is not just in typing data — it is in delivering information that is **accurate, organised, and decision-ready.**

A sales manager opening this file can immediately answer:
- *Who is my top rep?*
- *Which region is underperforming?*
- *What is my net revenue after discounts?*

— without asking anyone a single question.

---

📎 **[Download the Excel file](./Sales_Revenue_Tracker_FY2024.xlsx)**
