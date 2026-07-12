# 📊 Superstore Sales & Profit Analysis: An End-to-End Data Science Project

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Data-Science](https://img.shields.io/badge/Data--Science-EDA%20%7C%20ML-green.svg)
![Excel](https://img.shields.io/badge/Excel-Dashboard-success.svg)
![PowerBI](https://img.shields.io/badge/Power--BI-Analytics-orange.svg)

##  Project Overview
This is a comprehensive, end-to-end Data Science and Business Intelligence project conducted on a retail database (**Superstore Giant**). The goal is to provide actionable business insights to understand sales trends, maximize profits, identify loss-making areas, and predict transaction profits using Machine Learning.

To make this project impactful, the analysis is divided into three core deliverables:
1. **Data Analytics & Machine Learning** (Python Notebook)
2. **Interactive Executive Reporting** (Excel Dashboard)
3. **Advanced Business Intelligence** (Power BI Dashboard)

---

##  Business Problem Definition
With growing demands and cut-throat competition in the retail market, the Superstore Giant needs to optimize its operations. This project answers critical business questions:
* Which products, regions, categories, and customer segments should they target or avoid?
* Why are certain regions or products causing heavy losses despite high sales?
* Can we build a predictive regression model to estimate profits before shipping?

---

##  Tech Stack & Tools
* **Data Processing & ML:** Python (`Pandas`, `NumPy`, `Scikit-Learn`)
* **Data Visualization:** `Matplotlib`, `Seaborn`
* **Business Intelligence:** Microsoft Excel (Pivot Tables, Slicers), Power BI (DAX, Power Query, Advanced Visuals)

---

## Project Pipeline

### 1. Data Cleaning & Understanding
* Analyzed a dataset of 9,994 transaction rows and 21 features.
* Handled encoding issues and missing values.
* Converted date strings into proper datetime formats to prepare for time-series and ML features.

### 2. Exploratory Data Analysis (EDA) - Key Insights
* **Top Performers:** Identified the Top 5 most profitable and top-selling products (e.g., *Canon imageCLASS 2200 Advanced Copier* takes the lead).
* **The "Central" Region Issue:** Discovered a critical business leak where certain high-volume products (like the *Fellowes PB500 Electric Punch*) incur massive losses in the Central region due to aggressive discounting strategies (up to 80%).

### 3. Machine Learning (Predictive Modeling)
* **Problem Type:** Regression (Predicting `Profit`).
* **Feature Engineering:** Extracted `Order Year` and `Order Month` from order dates.
* **Preprocessing:** Applied One-Hot Encoding on categorical text columns (`Segment`, `Region`, `Category`, `Sub-Category`).
* **Model:** Trained a **Random Forest Regressor** (80/20 train-test split).
* **Evaluation:** Evaluated performance using Root Mean Squared Error (RMSE) and R² Score to map feature importance.

---

##  Business Intelligence Dashboards

###  Microsoft Excel Dashboard
* **KPI Cards:** Highlights Total Sales, Total Profit, and Average Discounts at a glance.
* **Dynamic Slicers:** Allows managers to filter metrics instantly by Region, Segment, and Category.
* **Risk Alert Feature:** A dedicated visualization calling out top loss-making products to aid immediate strategic decisions.

### Power BI Interactive Dashboard
* **Geographical Insights:** Interactive map visualization to analyze sales distribution across US states and cities.
* **Time Intelligence:** Line charts tracking monthly and yearly sales trends with drill-down capabilities.
* **Predictive Analytics View:** Integrates data insights derived from the Random Forest model, visualizing feature importances for business stakeholders.

---

## Repository Structure
```text
├── Data/
│   └── Sample - Superstore.csv      # The raw dataset
├── Notebooks/
│   └── data_science_project.ipynb   # Python EDA, Preprocessing, and ML code
├── Dashboards/
│   ├── Excel_Dashboard.xlsx         # Dynamic Excel report
│   └── PowerBI_Dashboard.pbix       # Power BI interactive file
└── README.md                        # Project documentation
