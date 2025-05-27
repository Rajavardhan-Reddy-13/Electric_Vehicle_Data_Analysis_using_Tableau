# 🚗 Electric Vehicle Market Analytics Dashboard

This interactive Tableau dashboard project analyzes the growth, distribution, and adoption trends of Electric Vehicles (EVs) across the United States using a real-world dataset. The project focuses on delivering business insights through data visualization, calculated KPIs, and state-wise market exploration.

---

## 📊 Project Objective

To explore and visualize the **landscape of electric vehicles** (BEVs and PHEVs) to support data-driven decision-making for manufacturers, policymakers, and analysts. The dashboard helps answer key questions such as:
- How has EV adoption evolved over the years?
- Which EV types dominate the market?
- What is the average electric range of EVs?
- Which manufacturers and models are most popular?
- How do government policies (CAFV eligibility) affect EV adoption?

---

## 📁 Dataset Used

- **Source**: [Kaggle - EV Population Dataset](https://www.kaggle.com/datasets/rajkumarpandey02/electric-vehicle-population-data)
- **Records**: 119,000+ EV records
- **Fields Included**:
  - `DOL Vehicle ID`
  - `Make`, `Model`, `Model Year`
  - `Electric Vehicle Type (BEV / PHEV)`
  - `Electric Range`
  - `CAFV Eligibility`
  - `State`, `City`

---

## ✅ KPIs (Key Performance Indicators)

1. **Total Vehicles**: Number of distinct EVs in the dataset (using `COUNTD`).
2. **Average Electric Range**: Average miles an EV can travel on a full charge.
3. **Total BEVs and % of Total**: Battery Electric Vehicles count and their market share.
4. **Total PHEVs and % of Total**: Plug-in Hybrid EVs count and their market share.

---

## 📈 Visualizations Created (Sheets)

### 1. Total Vehicles by Model Year
- **Chart Type**: Line / Area Chart (Dual Axis)
- **Insight**: Tracks yearly growth in EV adoption from 2011 to 2024.

### 2. Total Vehicles by State
- **Chart Type**: Map Chart
- **Insight**: Geographic EV distribution highlighting state-wise adoption (e.g., California leads with 119K+ EVs).

### 3. Top 10 Vehicles by Make
- **Chart Type**: Bar Chart (with dynamic Top N parameter)
- **Insight**: Tesla is the dominant manufacturer followed by Nissan and Chevrolet.

### 4. Vehicles by CAFV Eligibility
- **Chart Type**: Donut Chart
- **Insight**: Assesses impact of government policies and clean energy incentives.

### 5. Vehicles by Model
- **Chart Type**: Table / Tree Map
- **Insight**: Identifies most popular EV models (e.g., Tesla Model Y, Model 3).

---

## 🔧 Technical Implementation in Tableau

- **Calculated Fields**:
  - `Total Vehicles = COUNTD([DOL Vehicle ID])`
  - `Avg. Electric Range = AVG([Electric Range])`
  - Conditional counts using `IF` statements for BEVs and PHEVs
  - `% of Total = Total BEVs or PHEVs / Total Vehicles`

- **Filters and Parameters**:
  - Model Year filter ≥ 2011
  - Top N parameter for Make analysis
  - Context filters for EV Type, CAFV Eligibility

- **Dashboard Design**:
  - Custom layout using vertical and horizontal containers
  - KPI cards at the top
  - Interactive filtering (CAFV, State, EV Type)
  - Consistent color themes (green shades for EVs)

---

## 📌 Key Insights Derived

- BEVs dominate the dataset with **83.05%** of vehicles, highlighting strong shift toward fully electric mobility.
- The average electric range is **77.71 miles**, indicating mid-range performance across available models.
- Tesla accounts for over **57%** of all EVs in the dataset, solidifying its market leadership.
- States like **California** have seen the highest EV adoption.
- **45% of vehicles are CAFV-eligible**, indicating policy incentives’ influence on EV purchases.

---

## 📦 Tools & Technologies

| Tool         | Purpose                        |
|--------------|--------------------------------|
| Tableau      | Visualization, KPI dashboard  |
| MS Excel     | Data cleaning and preprocessing |
| Kaggle       | Data source                    |

---

## 📚 Learnings

- Mastered advanced Tableau features like **COUNTD**, **IF-THEN logic**, **dual-axis charts**, and **dynamic parameters**.
- Improved skills in dashboard UX design, filter interactivity, and KPI storytelling.
- Gained deeper insights into real-world EV adoption, government incentives, and consumer preferences.

---
## References
- https://www.youtube.com/watch?v=Y22CBLeHffg
