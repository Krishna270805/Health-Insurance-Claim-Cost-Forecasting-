
# 🩺 Health Insurance Claim Cost Forecasting using Time Series in R

## 📌 Objective
This project aims to forecast monthly health insurance claim payouts using historical data. By identifying trends and seasonal patterns, the model supports more accurate actuarial reserve planning and cost management.

---

## 🛠 Tools & Technologies
- **R:** `ts()`, `HoltWinters`, `forecast`, `ggplot2`
- **Excel:** Data cleaning and preprocessing
- **Visualization:** PNG plots exported from R

---

## 📂 Dataset
- `health_claims.csv` — contains monthly claim payout data from **Jan 2021 to Dec 2023**
- Columns:
  - `month`: Month in `YYYY-MM` format
  - `claim_cost`: Total claim payout for that month

---

## 📈 Approach
1. **Data Preparation:**
   - Loaded CSV and converted `month` to Date format
   - Created a time series object using R's `ts()` function

2. **Exploratory Analysis:**
   - Visualized trends using base R and `ggplot2`
   - Decomposed the series to extract trend, seasonality, and residuals

3. **Modeling:**
   - Applied **Holt-Winters exponential smoothing** for forecasting
   - Optionally used `auto.arima()` from the `forecast` package for comparison

4. **Forecasting:**
   - Projected the next 6 months of claim costs
   - Saved the forecast plot as `claim_cost_forecast.png`

5. **Evaluation:**
   - Assessed prediction accuracy using `accuracy()` from the `forecast` package

---

## 📊 Results
- Detected a **clear seasonal pattern** and an **upward trend** in claim costs
- Forecasts help anticipate future financial liabilities for better reserve planning
- Visualization helps stakeholders understand cost patterns over time

---

## 📁 Output Files
- `health_claims.csv` — dataset
- `health_claim_forecast.R` — R script
- `claim_cost_forecast.png` — forecast plot
- `Health_Insurance_Claim_Forecasting_Summary.pdf` — project summary

---

## ✅ Key Learnings
- How to work with time series data in R
- Applied forecasting models to real-world actuarial data
- Visualized and interpreted results for strategic decision-making

---

## 📧 Contact
For queries, reach out at [your.email@example.com]
