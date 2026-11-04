<div align="center">

# 🍨 Melt Gelato | Retail Sales & Demand Analytics

### Data-Driven Inventory Planning and Operational Efficiency

**Python · Machine Learning · Statistical Analysis · Power BI**

An end-to-end retail analytics project transforming historical point-of-sale data into actionable insights for demand forecasting, product prioritisation, and operational planning.

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat-square&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Visualisation-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=flat-square&logo=jupyter&logoColor=white)

</div>

---

## 📌 Project Overview

Retail businesses often face challenges in predicting customer demand, maintaining product availability, and managing operational resources efficiently.

This project analyses historical point-of-sale transactions from **Melt Gelato**, a gelato and café business in Navan, Ireland.

The analysis combines exploratory data analysis, statistical methods, machine learning, and product-level analytics to identify demand patterns and develop practical recommendations for inventory and operational planning.

**Academic Context:** Business Data Management Capstone — IIT Madras

### 🎯 Project Objectives

- Identify seasonal, weekly, and hourly sales patterns.
- Examine relationships between weather conditions and revenue.
- Develop and evaluate daily revenue forecasting models.
- Identify high-revenue products using ABC classification.
- Explore frequently purchased product combinations.
- Measure demand variability across product categories.
- Translate analytical findings into operational recommendations.

---

## 🔄 Analytics Workflow

```text
              Historical POS Data
                       │
                       ▼
              Data Understanding
                       │
                       ▼
            Cleaning & Validation
                       │
                       ▼
          Exploratory Data Analysis
                       │
              ┌────────┴────────┐
              ▼                 ▼
       Weather Analysis    Product Analysis
              │                 │
              ▼                 ▼
       Sales Forecasting   ABC Classification
              │                 │
              │            Market Basket
              │              Analysis
              └────────┬────────┘
                       ▼
             Business Recommendations
                       │
                       ▼
             Operational Decision Support
```

---

## 📊 Key Findings

### 1. Sales Demand Patterns

The exploratory analysis identified clear differences in demand across weekdays, weekends, and seasons.

| Finding | Observation |
|:---|:---|
| Highest-revenue month | May 2025 |
| Lowest-revenue month | January 2025 |
| Weekend demand | Average daily revenue approximately 54% higher than weekdays |
| Peak sales hour | 8 PM |
| Leading revenue category | Gelato |

**Business implication:** Historical demand patterns can support staffing decisions, product preparation, and inventory planning.

### 2. Weather and Sales Relationships

Historical weather observations were combined with daily sales records to examine relationships between revenue and weather conditions.

The analysis considered:

- Temperature
- Rainfall
- Sunshine duration

Sunshine showed a moderate positive correlation with daily revenue (**Pearson r = 0.494**).

These findings suggest that weather may provide useful context for understanding demand, although correlation does not establish causation.

### 3. Daily Revenue Forecasting

Three forecasting approaches were evaluated using a chronological training and testing split.

| Model | Test WAPE |
|:---|---:|
| **Calendar Ridge Regression** | **12.74%** |
| Calendar + Observed Weather Ridge | 15.03% |
| Seasonal Naïve (7-day lag) | 18.83% |

**Best-performing model:** Calendar Ridge Regression

The results indicate that calendar-related features provided a useful basis for predicting daily revenue during the evaluation period.

Including observed weather variables did not improve accuracy on the held-out test set.

### 4. ABC Product Classification

Products were ranked by revenue contribution and classified into A, B, and C groups.

| Category | Number of Products | Revenue Contribution |
|:---:|---:|---:|
| **A** | **44** | **80.45%** |
| B | 61 | 14.58% |
| C | 282 | 4.97% |
| **Total** | **387** | **100%** |

**Business implication:** Category A products may warrant closer inventory monitoring because they account for most payment revenue.

The classification is based on revenue rather than profitability.

### 5. Product Demand and Market Basket Analysis

The analysis also examined:

- Frequently purchased product combinations.
- Associations between products within completed transactions.
- Daily revenue variability across product categories.
- Differences between relatively stable and variable demand.

For example, Gelato exhibited greater relative daily revenue variability (**CV = 0.69**) than Coffee (**CV = 0.25**).

These findings provide a starting point for product preparation and potential promotional decisions.

---

## 📁 Repository Structure

```text
Melt-Gelato-Retail-Sales-Demand-Analytics/
│
├── notebooks/
│   ├── 01_Data_Understanding.ipynb
│   ├── 02_Data_Cleaning.ipynb
│   ├── 03_Exploratory_Data_Analysis.ipynb
│   ├── 04_Weather_Statistical_Analysis.ipynb
│   ├── 05_Sales_Forecasting_Interpreted.ipynb
│   ├── 06_Product_Inventory_Analysis_Interpreted.ipynb
│   └── 07_Business_Recommendations.ipynb
│
├── .gitignore
├── requirements.txt
└── README.md
```

### Notebook Guide

| Notebook | Focus |
|:---|:---|
| **01 — Data Understanding** | Dataset structure, initial inspection, and data quality checks |
| **02 — Data Cleaning** | Payment, refund, and void handling; validation |
| **03 — Exploratory Data Analysis** | Revenue trends, peak hours, weekdays, and categories |
| **04 — Weather & Statistical Analysis** | Weather relationships and statistical evaluation |
| **05 — Sales Forecasting** | Baseline forecasting, Ridge Regression, and model comparison |
| **06 — Product & Inventory Analysis** | Product rankings, ABC classification, market basket analysis, and demand variability |
| **07 — Business Recommendations** | Evidence-based recommendations and operational decision support |

---

## 🛠️ Technology Stack

| Area | Tools / Methods |
|:---|:---|
| Programming | Python |
| Data Manipulation | Pandas, NumPy |
| Visualisation | Matplotlib, Seaborn, Power BI |
| Machine Learning | Scikit-learn, Ridge Regression |
| Statistical Analysis | Pearson and Spearman correlations |
| Forecast Evaluation | MAE, RMSE, WAPE |
| Product Analytics | ABC Classification, Pareto Analysis |
| Basket Analytics | Transaction-level product associations |
| Development Environment | Jupyter Notebook |

---

## 💡 Business Recommendations

Based on the analysis, the project identified several opportunities for operational improvement.

**Inventory Prioritisation**

Monitor high-revenue products more closely to reduce the risk of unexpected unavailability.

**Demand-Based Preparation**

Use historical weekday, seasonal, and category-level patterns to support daily product preparation.

**Forecast-Assisted Planning**

Use calendar-based revenue forecasts as an additional input when planning staffing and operational resources.

**Product Combination Opportunities**

Explore frequently purchased product combinations to identify potential promotional opportunities.

**Continuous Evaluation**

Validate recommendations against inventory availability, product costs, wastage, and operational constraints before implementation.

---

## 🔒 Data Confidentiality

> **The original business dataset is not publicly available.**

This project uses confidential point-of-sale information provided for academic analysis.

To protect business confidentiality:

- Raw transaction datasets are excluded from this repository.
- Processed transaction-level datasets are not published.
- Business-sensitive source files are not included.
- The notebooks document the analytical workflow and methodology.

**Note:** The notebooks require access to the original private datasets for full execution.

---

## ⚠️ Limitations

- The analysis covers a limited historical observation period.
- Forecasting performance was evaluated using a chronological holdout period.
- Weather relationships are observational and do not establish causality.
- Inventory levels, product costs, wastage, and staffing information were not available for direct financial impact assessment.
- Recommendations require operational testing before implementation.

---

## 👩‍💻 About the Author

**Aakriti Abhay Singh**

MSc Data & Computational Science — University College Dublin  
B.Tech Data Science & Engineering — Manipal University Jaipur  
BSc Data Science & Programming — IIT Madras

**Areas of Interest:** Data Analytics · Machine Learning · Business Intelligence · Applied Data Science

---

<div align="center">

### 🍨 Turning Retail Data into Better Business Decisions

*Business Data Management Capstone Project | IIT Madras*

</div>
