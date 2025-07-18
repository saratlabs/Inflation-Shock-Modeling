# 📈 Inflation Shock Modeling

> **Modeling the Impact of Food and Fuel Price Shocks on Overall Inflation**
> Lightweight Econometric Approach using Simulated Macroeconomic Data

---

## 🧠 Objective

This project aims to **simulate and analyze the influence of sectoral shocks**—specifically from food and fuel price indices—on a country’s inflation rate. Using lightweight, interpretable models, the analysis provides insights into:

* How inflation responds differently to food vs. fuel price changes
* Short-term volatility patterns in inflation
* Price elasticity using linear regression techniques

---

## 🧰 Techniques Used

| Module                     | Technique                  | Description                                         |
| -------------------------- | -------------------------- | --------------------------------------------------- |
| 📊 Time Series Forecasting | **ARIMA**                  | Forecasting simulated inflation trends              |
| 📈 Elasticity Mapping      | **OLS Regression**         | Estimating sensitivity of inflation to price shocks |
| 📉 Volatility Analysis     | **Rolling Std. Deviation** | Identifying high-risk inflationary periods          |

---

## 📦 Dataset

This project uses **simulated data** to model real-world macroeconomic behavior. The dataset contains:

* `Date`
* `Food_Price_Index`
* `Fuel_Price_Index`
* `Inflation_Rate`

Data was generated to mimic typical quarterly or monthly patterns observed in macroeconomic time series.

---

## 📊 Key Findings

### 🔁 ARIMA Forecasting

* Modeled future inflation rates based on observed simulated trends.
* Helped identify seasonal peaks in inflation pressure.

### 📐 Price Elasticity Analysis

OLS regression results showed:

```text
Fuel_Price_Index     coef = 1.7753 (p = 0.006) ✅
Food_Price_Index     coef = 0.1080 (p = 0.905) ❌
R-squared            = 0.143
```

* **Fuel prices significantly influence inflation**, indicating **high elasticity**.
* **Food prices had negligible short-run impact**, suggesting **inelastic behavior**.
* Model explains about **14.3%** of inflation variability — consistent with macroeconomic expectations in a simplified setting.

### 📉 Volatility Mapping

* Inflation rates show **greater volatility** in periods driven by fuel shocks.
* Rolling standard deviation revealed **pockets of instability** aligned with spikes in fuel price changes.

---

## 🔧 Tools & Libraries

* `Python 3.x`
* `pandas`, `numpy`
* `matplotlib`, `seaborn`
* `statsmodels`

---

# Project Structure

📁 inflation_shock_modeling/
│
├── 📁 Data/                  # Simulated food, fuel, and inflation datasets
├── 📁 Notebooks/             # Main notebook containing all analysis
│   └── inflation_shock_modeling.ipynb
├── 📁 Outputs/               # ARIMA plots, Elasticity graphs, Volatility visuals
└── README.md                # Project summary and documentation


---

## 🚀 Conclusion

This project provides a simple yet powerful demonstration of how inflation responds asymmetrically to **sectoral price shocks**. The analysis highlights the **dominant role of fuel price volatility** in shaping inflationary pressure and sets the stage for deeper causal or ML-based explorations in macroeconomics.

---

## Contribution & Credits

Project Lead: Sai Sarat Chandra

Data Science & Econometrics Enthusiast

Focus: Causal Inference, Policy Modeling, and AI for Social Impact


