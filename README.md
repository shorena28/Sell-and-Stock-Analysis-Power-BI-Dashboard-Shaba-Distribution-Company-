# 📦 Procurement & Stock Performance Dashboard (Power BI)

## 📌 Overview

This dashboard analyzes procurement plan execution and stock performance, combining:

- Procurement vs Execution
- Stock vs Sales dynamics
- Inventory sustainability
- Brand-level performance
- Time-based stock behavior

👉 Designed for procurement, supply chain, and sales analytics.

---

# 🎯 Key Objectives

- Track procurement plan execution (2024 vs 2025)
- Monitor stock levels vs sales
- Evaluate inventory efficiency
- Identify overstock / understock risks
- Support better purchasing decisions

---

# 📊 Key KPIs

| KPI | Value | Description |
|---|---|---|
| Sell at Cost Price | 57M | Total sales value at cost |
| Stock at Cost Price | 256M | Total inventory value at cost |
| Total Stock Quantity | 258M | Total stock units |
| Sold Quantity | 18M | Total sold units |
| Avg Sold Quantity | 4K | Average sold quantity |

👉 Quick snapshot of inventory scale vs movement.

---

# 📈 Dashboard Structure

## 1. 📅 Procurement Plan Execution (2025 vs 2024)

### Includes

- Annual Procurement Plan
- Plan Execution
- Difference
- % Execution
- Sales with Big Amount

### 👉 Insight

- Measure how much of the plan is fulfilled
- Compare year-over-year procurement performance
- Detect under-execution gaps

### ⚠️ Observation

> % Execution = 0% may indicate:
>
> - Missing plan data
> - Incorrect measure logic

👉 Important to fix before presenting.

---

## 2. 📦 Stock & Sales Overview

### KPIs Show

- Inventory size vs movement
- Sales speed

### 👉 Insight

- High stock + low sales = ⚠️ Overstock risk
- Balanced ratio = ✅ Healthy inventory flow

---

## 3. 🏷️ Brand-Level Stock Performance

### Includes

- Sell at Cost Price
- Sold Quantity
- Avg Sold Quantity
- Stock at Cost
- Total Stock
- Remaining Stock (Months)

### 👉 Insight

Identify:

- Fast-moving brands
- Slow-moving / dead stock
- Overstock risks

---

## 4. 📊 Multi-Brand Comparison Table (by Year)

Shows performance across brands such as:

- Adidas
- Apple
- BMW
- Chanel
- Coca-Cola

### 👉 Insight

- Compare brands across years
- Detect growth or decline

---

## 5. 📅 Monthly Inventory Behavior

### Includes

- Sales (Cost Price)
- Sold Quantity
- Avg Sold Quantity
- Stock levels
- Remaining Stock (Months)

### 👉 Insight

Detect:

- Seasonality
- Inventory buildup
- Consumption trends

---

# 🎛️ Filters (Slicers)

- Brand
- Year
- Month
- Quarter

👉 Fully dynamic analysis across all visuals.

---

# ⚙️ Key Calculations

## 📦 Remaining Stock (Months)

```DAX
Remaining Stock Months =
DIVIDE(
    [Total Stock Quantity],
    [Avg Monthly Sold Quantity],
    0
)
