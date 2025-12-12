# Bike Buyers Purchase Rate Dashboard (Excel & Tableau)

## Overview

This project analyzes **bike purchasing behavior** using the Bike Buyers dataset.  
Each row represents one customer, and the target variable `Purchased Bike` indicates whether the customer bought a bike (`Yes/No`).

The goal is to answer:

- What is the **overall purchase rate**?
- How does purchase rate change by **gender**, **age band**, **income band**, **commute distance**, and **region**?

I used **Excel** for pivot analysis and band creation, and **Tableau** for visualization and dashboarding.

---

## Dataset

- **Source:** Bike Buyers dataset (Kaggle)
- **Grain:** One row per customer
- **Key fields:**
  - `Gender`
  - `Age` (used to create `age_band`)
  - `Income` (used to create `income_band`)
  - `Commute Distance`
  - `Region`
  - `Purchased Bike` (Yes/No)

*(Add the Kaggle dataset link you used in this repo description if you want.)*

---

## Excel Preparation

### 1) Created derived bands
- **age_band:** `<30`, `30-40`, `41-50`, `>50`
- **income_band:** `Low`, `Medium`, `High`

### 2) Pivot tables
Built pivot tables to compare customers who purchased vs. did not purchase a bike:
- Purchase by **Gender**
- Purchase by **age_band**
- Purchase by **Commute Distance**
- Purchase by **income_band**
- Purchase by **Region**

### 3) Key Results (from the dashboard)

Overall purchase rate: ~48.1%

Gender: Female (~48.7%) and Male (~47.5%) are very close.

Commute Distance: Higher purchase rates for shorter commutes (e.g., 2–5 miles ~58.6%, 0–1 miles ~54.6%) and much lower for long commutes (10+ miles ~29.7%).

Age Band: Highest purchase rate in 30–40 (~57.4%), followed by 41–50 (~46.8%); lowest in older groups (e.g., >50 ~39.9%).

Income Band: Higher purchase rate in High (~52.1%) and Medium (~50.8%) vs Low (~40.7%).

Region: Highest in Pacific (~58.9%), then Europe (~49.3%), lowest in North America (~43.3%).

These insights can help target marketing campaigns toward the segments most likely to purchase.
