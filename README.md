# 🏞️ Bathing Water Quality Analysis (CPCB Standards)

### Power BI Dashboard | Environmental Analytics | Open Dataset Release

This repository contains the analysis, scoring logic, and visual dashboard built on **CPCB (Central Pollution Control Board) Bathing Water Quality Standards** using **minimum & maximum water quality parameters** recorded across multiple water bodies.

The project includes:

* ✔ Cleaned dataset
* ✔ Environmental scoring model (CPCB-based)
* ✔ Power BI dashboard
* ✔ Methodology & insights
* ✔ Reproducible logic for other states/countries

---

## 📑 **Dataset Description**
Dataset Source: The water quality data has been obtained from the official records of the Central Pollution Control Board (CPCB), Government of India — latest publicly released dataset for bathing water bodies. Data was retrieved under CPCB norms and is being shared here for research and environmental analytics purposes. Features of dataset

* Monitoring Location
* Latitude / Longitude
* Water Body Type (Lake / River / Pond)
* **pH (Min – Max)**
* **Dissolved Oxygen (DO) Min – Max**
* **Biochemical Oxygen Demand (BOD) Min – Max**
* **Fecal Coliform (FC) Min – Max**
* CPCB Threshold Pass/Fail (pH, DO, BOD, FC)

This dataset can be used for:

* Bathing water quality assessment
* Environmental monitoring
* CPCB framework-based scoring
* Research & visualization
* Statistical Variation study
* Min Max variation analysis
* Correlation Analysis
  
---

## 🎯 **Objective**

To evaluate bathing water suitability using **CPCB Bathing Water Standards** and visualize the results in a clean, simple Power BI dashboard.

---

## 📘 **CPCB Criteria Used (Regulatory Standards)**

| Parameter                 | Standard          | Pass Condition |
| ------------------------- | ----------------- | -------------- |
| **Dissolved Oxygen (DO)** | ≥ 5 mg/L          | Good           |
| **BOD**                   | ≤ 3 mg/L          | Good           |
| **Fecal Coliform**        | ≤ 2500 MPN/100 ml | Good           |
| **pH**                    | 6.5 – 8.5         | Good           |

Water body is **Suitable for Bathing** only if **all 4 criteria pass** (score = 4).

---

## 🧮 **Scoring Method (0–4 System)**

Each parameter contributes **1 point** if it meets the CPCB standard.

```
DO_score = IF(DO_pass, 1, 0)
BOD_score = IF(BOD_pass, 1, 0)
FC_score  = IF(FC_pass, 1, 0)
pH_score  = IF(pH_pass, 1, 0)
```

Final score:

```
total_score = DO_score + BOD_score + FC_score + pH_score
```

### **CPCB Category Classification**

```
4 → Excellent
3 → Good
2 → Marginal
1 → Poor
0 → Very Poor
```

---

## 📊 **Power BI Dashboard Overview**

The dashboard visualizes:

### **1️⃣ KPI Summary**

* Total water bodies monitored
* Suitable for bathing (%)
* Average total score
* Number of failing stations

### **2️⃣ Map Visualization**

* Location-wise water quality score
* Color-coded CPCB category

### **3️⃣ Parameter Pass %**

* DO
* BOD
* FC
* pH

### **4️⃣ Score Distribution**

* Count of stations with score 0–4

### **5️⃣ Station-Wise Water Quality Table**

* pH Min–Max
* DO Min–Max
* BOD Min–Max
* FC Min–Max
* Category
* Final Suitability

---

## 🛠 **Tools & Technologies**

* **Power BI** for dashboard
* **DAX** for scoring and classification
* **Excel / CSV** for data cleaning
* **Geospatial Mapping** using Lat-Long
* **CPCB Bathing Water Quality Framework**

---

## 📁 **Repository Structure**

```
📦 bathing-water-quality/
│
├── 📄 Dataset.xlsx               # Released dataset (pH, DO, BOD, FC)
├── 📄 PowerBI_Dashboard.pbix     # Dashboard file
├── 📄 README.md                  # Project documentation
├── 📄 scoring_logic.txt          # Scoring & CPCB thresholds

```

## 🔍 **Key Insights from Analysis**

* Many water bodies passed DO and pH criteria
* BOD & Fecal coliform were the frequent failing parameters
* Map highlights regional pollution hotspots
* Only a certain % waterbodies meet full bathing suitability criteria

---

## 🚀 How to Use This Repository

1. Clone this repo
2. Open the dataset in Excel or Power BI
3. Load the **PowerBI_Dashboard.pbix** file
4. Refresh visuals with updated data
5. Modify scoring rules or add new waterbodies as needed

---

## 🌱 **Future Enhancements**

* Integrating WQI (Water Quality Index)
* Insights report generation
* Predictive modelling for pollution hotspots
* Automated data ingestion with APIs
* Statistically based Correlation study
* Variation study
  
---

## 🙌 **Connect With Me**

If you want help with:

* Environmental analytics
* Power BI dashboards
* Water quality scoring models
* Data cleaning automation

Bas batao — main turant add kar dunga!
