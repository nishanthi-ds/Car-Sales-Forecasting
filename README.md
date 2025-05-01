# Car Sales Forecasting using SARIMAX

This time series forecasting project uses the **SARIMAX model** to predict **monthly car sales**. SARIMAX is an extension of the ARIMA model that supports **seasonal effects** and **exogenous variables**, making it suitable for modeling real-world time-dependent data with trends and seasonal patterns.

---

## Project Overview

This project aims to understand the pattern in car sales over time and forecast future values. It includes:

- Loading and cleaning the dataset.
- Exploratory Data Analysis (EDA) with visualizations.
- Time series decomposition to analyze trend, seasonality, and noise.
- Building and tuning a SARIMAX model.
- Forecasting and comparing predictions with actual values.

---

## Dataset

- **File**: `monthly-car-sales.csv`
- **Content**: Monthly car sales data (usually 1 record per month).
- **Format**: CSV with columns like `Month`, `Sales`, etc.
- **Period**: Spanning multiple years to capture seasonality.

---

## Project Structure

```
├── forcasting.ipynb       # Jupyter notebook with full analysis and model
├── monthly-car-sales.csv  # Dataset used
└── README.md              # Project documentation
```

---

## Steps

1. **Importing Libraries**
2. **Loading the Dataset**
3. **Exploratory Data Analysis**
   - Line plots for sales trends
   - Seasonal decomposition
4. **Stationarity Check**
   - Augmented Dickey-Fuller test
   - Differencing
5. **Training the SARIMAX Model**
   - Determining p, d, q, P, D, Q, s values
   - Training the model
7. **Forecasting**
   - Predicting future sales
   - Visualizing predictions vs actual values
8. **Model Evaluation**
   - RMSE, R2 Square metrics

---

## Why SARIMAX?

- Handles both trend and seasonality.
- Can incorporate external regressors 
- Suitable for monthly sales data with seasonal peaks and dips.

---

## Tools & Libraries

- **Python**
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Visualization
- **Statsmodels**: SARIMAX modeling and diagnostics
- **NumPy**: Numerical computing

---

