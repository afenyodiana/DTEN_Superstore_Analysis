# DTEN Superstore Analysis
### Data Science & Analytics Internship Project

**Author:** Diana Sedinam Afenyo  
**Organization:** Daryl Tech & Educational Network  
**Date:** October 2026

---

## 📋 Project Overview

This project analyzes 9,994 Superstore sales orders (2014–2017) to uncover profitability drivers and build a predictive model + interactive dashboard.

**Tools Used:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn) · Power BI · Jupyter Notebook

---

## 📁 Repository Structure

| File | Description |
|------|-------------|
| `DTEN_Task1_EDA.ipynb` | Task 1: Exploratory Data Analysis (4 charts + insights) |
| `DTEN_Task2_Predictive_Model.ipynb` | Task 2: Random Forest Classifier for profitability prediction |
| `DTEN_Task3_Dashboard.pbix` | Task 3: Interactive Power BI dashboard |
| `Screenshot 2026-10-05 194214.png` | Task 3 dashboard image |
| `superstore.csv` | Raw dataset (9,994 rows, 21 columns) |

---

## 📊 Task 1: Exploratory Data Analysis — Key Findings

1. **Regional Performance:** The West region leads in both Sales (~$725K) and Profit. The Central region shows disproportionately low profit relative to sales — suggesting regional discounting or cost issues.
2. **Sub-Category Profitability:** Tables (-$17,725) and Bookcases (-$3,472) operate at a loss. Copiers (+$55,617), Phones, and Accessories drive the majority of profit.
3. **The Discount Problem:** A -0.22 correlation exists between Discount and Profit, with a critical tipping point at 40%. Below 40%, orders remain profitable; above 40%, most operate at a loss.
4. **Growth & Seasonality:** Consistent YoY growth from 2014–2017, with recurring spikes in September and November/December (back-to-school and holiday effects).

---

## 🤖 Task 2: Predictive Model Building

- **Target Variable:** `Is_Profitable` (1 if Profit > 0, else 0)
- **Model:** Random Forest Classifier (100 trees)
- **Accuracy:** ~80%
- **Top 3 Predictors:** Discount, Sales, Quantity

**Key Takeaway:** The model confirms EDA findings — Discount is the strongest predictor of whether an order loses money.

---

## 📈 Task 3: Interactive Dashboard (Power BI)

Features:
- KPI Cards — Total Sales, Profit, Quantity
- Bar Chart — Sum of Sales by Region
- Line Chart — Sum of Profit over Time
- Bar Chart — Profit by Sub-Category
- Slicer — Region (interactive filter)

---

## 🎯 Recommendations

1. Cap all discounts at 30–35% to protect margins.
2. Re-evaluate the Tables and Bookcases product lines.
3. Investigate Central region's pricing and discounting practices.
4. Increase investment in high-margin categories (Copiers, Phones, Accessories).
5. Deploy the Power BI dashboard for weekly performance monitoring.

---

**© 2026 Diana Sedinam Afenyo — Data Science & Analytics Internship Project**
