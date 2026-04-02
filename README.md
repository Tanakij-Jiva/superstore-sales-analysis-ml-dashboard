# Superstore Sales Analysis & Machine Learning Project

## Overview

This project analyzes retail sales data to uncover key business insights and build a predictive model for profit. It combines **business intelligence (BI)** and **machine learning (ML)** to support data-driven decision-making.

The project is divided into two main components:

* **Interactive Dashboard (Power BI / Tableau)** — for business insights
* **Machine Learning Model (Python)** — for profit prediction

---

## Objectives

* Analyze sales and profitability trends
* Identify key drivers of profit
* Build a predictive model to estimate profit
* Communicate insights through an interactive dashboard

---

## Dashboard (Business Intelligence)

The dashboard provides a clear overview of business performance:

### Key Features:

* Sales, Profit, and Margin KPIs
* Sales trends over time
* Regional performance analysis
* Category-level profitability

### Tools Used:

* Power BI / Tableau

---

## Key Insights

### 1. Discount Impact

* Strong **negative relationship** between discount and profit
* High discounts often lead to losses

**Business implication:**
Discount strategies must be optimized to avoid profit erosion

---

### 2. Sales vs Profit Mismatch

* High sales do not always translate into high profit
* Some high-revenue products have low margins

**Business implication:**
Focus on **profitability**, not just revenue

---

### 3. Regional Performance Variation

* Significant differences in profit across regions

**Business implication:**
Target underperforming regions for improvement

---

### 4. Category Contribution

* A small number of categories drive most of the profit

**Business implication:**
Prioritize high-margin product categories

---

## Machine Learning Model

### Model Details:

* Model: XGBoost
* Task: Regression (Predict Profit)
* Target Variable: `Profit`

### Feature Engineering:

* Extracted time features (Year, Month)
* Encoded categorical variables
* Removed irrelevant identifiers

### Hyperparameter Tuning:

* Method: Bayesian Optimization using Optuna
* Improved model performance and efficiency

---

## Model Performance

* Evaluated using:

  * Mean Absolute Error (MAE)
  * R² Score

* Visual analysis:

  * Actual vs Predicted
  * Residual distribution
  * Feature importance

---

## Key ML Insights

* Discount is one of the strongest predictors of profit
* Certain categories significantly influence outcomes
* Model captures nonlinear relationships effectively

---

## Tech Stack

### Data Analysis & ML:

* Python
* Pandas
* Scikit-learn
* XGBoost
* Optuna

### Visualization:

* Power BI / Tableau
* Plotly (for exploratory analysis)

---

## Project Structure

```
project/
│── data/
│   └── superstore.csv
│
│── notebooks/
│   └── analysis_and_model.ipynb
│
│── dashboard/
│   └── powerbi_dashboard.pbix
│
│── README.md
```

---

## How to Run

1. Clone the repository
2. Open the notebook in Google Colab or Jupyter
3. Install dependencies:

   ```
   pip install pandas scikit-learn xgboost optuna
   ```
4. Run all cells

---

## Future Improvements

* Deploy model as a web application
* Integrate real-time predictions into dashboard
* Experiment with advanced models (LightGBM, CatBoost)
* Improve feature engineering

---

## Business Value

This project demonstrates how data can be used to:

* Optimize pricing and discount strategies
* Improve profitability
* Support strategic decision-making

---

## Author:

Tanakij Jivacharoen

---

## Key Takeaway

This project goes beyond basic analysis by combining **interactive dashboards with predictive modeling**, showcasing end-to-end data science capabilities.
