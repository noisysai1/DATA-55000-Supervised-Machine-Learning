# Week 06 — Crop Production Data Analysis (Final Project Part 1)

## 📚 Topics Covered
- Exploratory Data Analysis (EDA) on agricultural datasets
- Understanding soil nutrients (N, P, K), pH, rainfall, and temperature
- Correlation analysis between features
- Histogram visualization of numeric columns
- Dataset preprocessing for supervised learning models

---

### ✅ Learning Objectives
- Load and inspect a **large dataset** (≈99,849 rows × 13 columns) of crop production in India.
- Perform **data exploration**: summary statistics, correlations, and feature distributions.
- Interpret relationships between soil composition, environmental factors, and crop yields.
- Prepare dataset for further machine learning tasks (regression and classification).

---

### 📝 Key Concepts & Explanations

1. **Dataset Overview**:  
   Source: Kaggle
   - **Rows:** 99,849  
   - **Columns:** 13 (including State, Crop Type, Crop, soil nutrients, climate variables, and yield).  
   - Example columns:  
     - `State_Name` (e.g., Andhra Pradesh, West Bengal)  
     - `Crop_Type` (kharif, rabi, summer)  
     - `N`, `P`, `K` (soil nutrients)  
     - `pH`, `rainfall`, `temperature`  
     - `Area_in_hectares`, `Production_in_tons`, `Yield_ton_per_hec`

---

2. **Data Inspection**:
   - `.head(10)` displayed first records including cotton, horsegram, maize, and rice.  
   - `.info()` confirmed all numeric and categorical features were loaded correctly.  
   - `.shape` = (99,849, 13).  
   - `.describe()` produced summary statistics (mean, std, min, max for numeric columns).  

---

3. **Correlation Analysis**:
   - **Positive correlations:**  
     - N, P, K nutrients show moderate correlations.  
     - Production is positively related to rainfall and area.  
   - **Negative correlations:**  
     - Soil pH has weak negative correlations with nutrients.  
     - Area and yield show trade-offs in certain cases.  

   Example (correlation coefficients):  

N vs P: 0.34
N vs K: 0.49
Yield vs P: 0.07
Yield vs K: 0.08

---

4. **Histograms & Visualizations**:
- Histograms generated for all numeric variables.  
- Key findings:  
  - Rainfall distribution was **skewed**, indicating variability across states.  
  - pH values centered around **5.5–6.0**, typical for agricultural soils.  
  - Yield varied significantly, reflecting crop type and state-level conditions.

---

### 📊 Week 6 Results
- Successfully **loaded and inspected a large-scale agricultural dataset**.  
- Identified **patterns in soil nutrients and climate variables**.  
- Gained insights into **correlations affecting crop yields**.  
- Prepared the foundation for **predictive modeling (Part 2 in Week 7)**.

---

### 📂 Deliverables
- 📄 [Week 6 Project Notebook PDF](./Week_6_Project_Notebook.pdf)  
- 📄 [Crop Production Dataset (CSV)](./Crop_production.csv)  
- 📄 [Python Script](./project.py)  
---

### 🔖 Reflections
- Handling a **large dataset** was challenging but insightful for agricultural ML applications.  
- Correlation analysis highlighted **multivariate relationships** between nutrients, rainfall, and yield.  
- Visualizations improved understanding of **data distribution** and possible preprocessing needs.  
- This project connected ML concepts to **real-world farming applications**, emphasizing the importance of data-driven agriculture.

---

### ✅ Checklist
- [x] Upload Week 6 project files  
- [x] Explore dataset with Pandas and Matplotlib  
- [x] Generate descriptive statistics  

---
