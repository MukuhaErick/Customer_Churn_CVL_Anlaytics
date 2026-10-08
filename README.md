# Customer Churn & Lifetime Value (CLV) Analysis

An end-to-end data analytics and machine learning pipeline predicting customer churn and evaluating Customer Lifetime Value (CLV) to inform targeted marketing retention strategies.

## Executive Summary
This project evaluates retail customer transaction histories to identify key behavioral drivers of churn (inactivity > 90 days)[cite: 2]. By combining hypothesis testing, binary classification modeling, and financial simulation, the framework demonstrates how predictive analytics can directly increase retention ROI[cite: 2, 7].

Key business findings include:
* **Primary Churn Drivers:** Order frequency ($p < 0.0001$) and total monetary spend ($p < 0.0001$) are statistically significant indicators of customer retention[cite: 2, 3].
* **Model Performance:** Logistic Regression outperformed Random Forest with an **ROC-AUC of 0.7452**[cite: 2] and a **churn recall rate of 82%**[cite: 6].
* **Financial Impact:** A simulated win-back campaign targeting high-value at-risk customers yielded a **1,315.71% ROI** and **$61,772.51 in net recovered revenue**[cite: 7].

---

## Tech Stack & Methodology
* **Language & Tools:** Python 3.13, VS Code, Jupyter Notebooks[cite: 2, 4]
* **Data Processing & EDA:** Pandas, NumPy, SciPy (Welch's t-tests)[cite: 2]
* **Machine Learning:** Scikit-Learn (Logistic Regression, Random Forest, StandardScaler)[cite: 2, 6]
* **Data Visualization:** Matplotlib, Seaborn[cite: 2, 4]

---

## Key Results & Figures

### 1. Statistical Feature Distributions
Welch's two-sample t-tests confirmed that active customers maintain significantly higher order frequencies (5.83 vs 4.30) and overall spend ($493.09 vs $365.09) compared to churned customers[cite: 2, 3].

![EDA Feature Distributions](reports/figures/eda_feature_distributions.png)

### 2. Feature Importance (Logistic Regression Coefficients)
Standardized feature coefficients highlight that purchase frequency has the strongest negative impact on churn odds[cite: 7].

![Feature Importance](reports/figures/feature_importance.png)

### 3. Financial Campaign Simulation
| Metric | Value |
| :--- | :--- |
| **Targeted At-Risk Customers** | 313[cite: 7] |
| **Campaign Budget ($15/cust)** | $4,695.00[cite: 7] |
| **Projected Conversion Rate** | 20.00%[cite: 7] |
| **Gross Revenue Recovered** | $66,467.51[cite: 7] |
| **Net Revenue Gain** | **$61,772.51**[cite: 7] |
| **Projected ROI** | **1,315.71%**[cite: 7] |

---

## How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/customer-churn-clv-analysis.git](https://github.com/your-username/customer-churn-clv-analysis.git)
   cd customer-churn-clv-analysis