# 📁 Project 02 — Inventory Management System (FY 2024)

**Role:** Remote Data Entry Clerk  
**Tools:** Microsoft Excel  
**Date:** March 2026  
**File:** [Download Inventory_Management_Kazi_Supplies_FY2024.xlsx](./Inventory_Management_Kazi_Supplies_FY2024.xlsx)

---

## Background

Kazi Supplies Ltd, a Nairobi-based office supplies company, needed a centralised inventory management system to track stock levels, monitor inflows and outflows, flag low-stock items, and report the total value of goods held at any time.

The company stocked 30 unique products across 6 categories — Stationery, Electronics, Furniture, Hygiene, Pantry, and Security — sourced from 6 different suppliers. A remote data entry clerk was brought in to build and populate the full inventory system from scratch.

---

## The Problem

Without a structured system, the business faced:

- No visibility into which items were running low until stock physically ran out
- No record of who moved stock, when, and why
- No way to calculate the total value of inventory at any given time
- Expiry-date sensitive items (sanitisers, food, masks) with no tracking in place
- Management unable to make informed reorder decisions

---

## What I Did

### 1. Data Entry & Organisation
All 30 inventory items were entered into a structured master sheet capturing: Item ID, Product Name, Category, Supplier, Unit Price, Units In Stock, Reorder Level, Units On Order, Last Restocked date, Expiry Date, and Notes.

A separate stock movement log was built recording 25 transactions — covering every Stock In, Stock Out, and Adjustment event across the year, with the responsible staff member noted for each.

### 2. Formula Building
All calculated columns were built using live Excel formulas — no hardcoded values:

| Formula | Purpose |
|---|---|
| `=E4*F4` | Stock Value (Unit Price × Units In Stock) |
| `=IF(F4=0,"⚠ Out of Stock", IF(F4<=G4,"🔶 Low Stock","✔ OK"))` | Automatic status flag |
| `=SUMIF(...)` | Units and value totals by category |
| `=COUNTIF(...)` | SKU counts and status counts |

### 3. Data Verification
A 12-point verification log was completed covering: duplicate ID checks, missing field checks, negative stock checks, formula accuracy, status flag logic, category consistency, stock movement reconciliation, dashboard tie-out, and expiry date review. All 12 checks passed.

### 4. Reporting & Formatting
A summary dashboard was built showing: KPI cards (total SKUs, units, stock value, items on order), stock status breakdown (OK / Low Stock / Out of Stock), category-level summary, and a colour-coded **Low Stock & Reorder Alert table** highlighting items needing immediate attention.

---

## The Output

A fully self-contained, four-sheet Excel workbook:

| Sheet | Contents |
|---|---|
| **Inventory Master** | 30 items with live stock value and auto status flags |
| **Stock Movement Log** | 25 transactions — ins, outs, adjustments |
| **Summary Dashboard** | KPIs, category breakdown, reorder alert table |
| **Verification Log** | 12-point quality check — all passed ✔ |

---

## Real-World Value

A procurement or operations manager opening this file can immediately answer:

- *What is our total inventory value right now?*
- *Which items need to be reordered today?*
- *Who last moved stock, and when?*
- *Which products are expiring soon?*

This is the kind of system that prevents stock-outs, reduces waste, and gives management the confidence to make purchase decisions without guesswork.

---

📎 **[Download the Excel file](./Inventory_Management_Kazi_Supplies_FY2024.xlsx)**
