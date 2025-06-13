# 📈 Sales Forecasting Using Time Series Analysis

## 🧠 About the Project

This project was created to forecast monthly product sales using time series analysis techniques. I generated a 3-year mock dataset with trend and seasonality to simulate a realistic business scenario.

The main objective was to build a reliable model that could predict sales for the next 12 months, while also evaluating its accuracy and visualizing forecast trends.

---

## 🛠️ Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- `statsmodels` for decomposition
- `pmdarima` for SARIMA modeling
- `sklearn` for evaluation metrics

---

## 🔍 Approach

1. **Generated Mock Sales Data**  
   Simulated 36 months of monthly sales using Poisson distribution + linear trend.

2. **Time Series Decomposition**  
   Broke the series into trend, seasonality, and residual components to better understand the structure.

3. **Modeling with SARIMA**  
   Used `auto_arima()` to find the optimal seasonal ARIMA configuration. Trained the model on the first 24 months and tested it on the final 12 months.

4. **Forecasting**  
   Generated 24-month forecasts (12 for validation and 12 for the future) and visualized them with confidence intervals.

5. **Evaluation**  
   Evaluated performance using:
   - **MAE**: 17.22  
   - **RMSE**: 21.04  
   Found that predictions were mostly accurate, but the model underperformed slightly during high-sales months.

---

## ✅ Key Takeaways

- SARIMA captured the overall sales trend and regular seasonality well.
- The model struggled slightly with year-end and mid-year sales peaks.

---

## 📁 Files

- `sales_forecasting.ipynb` – Jupyter Notebook with full code  
- `Task3_Sales_Forecasting_Using_Time_Series_Analysis.pdf` – Final report  
- `Task3_README.md` – This file

---

*Author: [Nasir Ali] | Date: June 13, 2025*