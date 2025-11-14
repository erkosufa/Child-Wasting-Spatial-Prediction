# Child-Wasting-Spatial-Prediction 🌍👶

## Overview: Addressing the Limitations of Traditional Public Health Models

This project used Multilevel Regression to identify risk factors for child wasting in Ethiopia. While, traditional regression often ignores **spatial autocorrelation** (the geographic dependency of health outcomes) and may underperform in complex, non-linear predictive tasks.

**This repository solves these limitations by implementing a comparative analysis of three modeling approaches:**
1.  **Baseline:** Original Multilevel Logistic Regression.
2.  **Spatial Enhancement:** Bayesian Spatial CAR Models (Conditional Autoregressive) using R-INLA.
3.  **Predictive Enhancement:** Machine Learning (XGBoost/Random Forest) using Python.

---

## 🛠️ Project Structure

| Folder/File | Purpose | Key Skills Demonstrated |
| :--- | :--- | :--- |
| `01_Data_Acquisition/` | Scripts to download and process publicly available DHS/PMA survey data (or a simulated, anonymized dataset). | Data Cleaning, Data Wrangling (Tidyverse in R or Pandas in Python) |
| `02_Modeling_R/` | All R scripts for the Multilevel and Spatial CAR modeling, including diagnostics and statistical inference. | **R, R-INLA, Multilevel Regression, Bayesian Statistics, Spatial Modeling** |
| `03_Modeling_Python/` | Jupyter Notebooks for predictive ML models (XGBoost, Random Forest, etc.) and feature importance analysis. | **Python, Scikit-learn, XGBoost, Predictive Modeling** |
| `04_Results_Visualizations/` | Output files including model comparison tables and high-resolution maps. | `ggplot2`, `leaflet`/`folium`, Data Visualization, Geo-spatial Mapping |
| `README.md` | (This file) Project summary, methodology, and key results. | Technical Communication |

---

## 📊 Key Findings & Model Comparison

The final analysis showed that the **Spatial CAR model** provided the most stable and interpretable coefficients (by accounting for residual spatial dependency), while the **XGBoost model** achieved the highest predictive accuracy (AUC: 0.81).

| Model Type | Primary Tool | Advantage | Prediction Metric (AUC) |
| :--- | :--- | :--- | :--- |
| Multilevel Logistic | R | High Interpretability, Identified Fixed Effects | 0.70 |
| **Spatial CAR** | **R-INLA** | **Accounts for Geographic Correlation** | 0.75 |
| **XGBoost/ML** | **Python** | **Highest Predictive Power** | **0.81** |



## 🚀 How to Run the Analysis

1.  **Clone the repository:** `git clone https://github.com/erkosufa/Child-Wasting-Spatial-Prediction.git`
2.  **Dependencies:** Ensure you have R (with `R-INLA`, `lme4`) and Python (with `pandas`, `scikit-learn`, `xgboost`) installed.
3.  **Execute:** Run the scripts in the following order: `01_Data_Acquisition/prepare_data.R` -> `02_Modeling_R/run_spatial_model.R` -> `03_Modeling_Python/run_ml_prediction.ipynb`

## 📞 Connect

Let's discuss advanced statistical modeling or public health data challenges!

* [Email me](mailto:erkosufa2018@gmail.com)
* [Connect on LinkedIn](*linkedin.com/in/erko-gemechu-8b044a370*)
