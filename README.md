# Car Sales Forecasting using SARIMAX

This time series forecasting project uses the **SARIMAX model** to predict **monthly car sales**. SARIMAX is an extension of the ARIMA model that supports **seasonal effects** and **exogenous variables**, making it suitable for modeling real-world time-dependent data with trends and seasonal patterns.

The project includes the following steps:

1- **Data Collection:** A monthly car sales dataset is used, containing historical sales figures over time.

2- **Data Analysis:** The dataset is analyzed.

3- **Stationarity Check:** The Augmented Dickey-Fuller (ADF) test is applied to assess whether the time series is stationary.

4- **Data Visualization:** Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) plots are used to determine the optimal parameters for the SARIMAX model.

5- **Model Building:** A SARIMAX (Seasonal ARIMA with Exogenous variables) model is constructed, considering parameters such as p, d, q (ARIMA terms) and seasonal components.

6- **Model Training:** The model is trained on the historical dataset by tuning the parameters p, d, and q based on ACF/PACF insights.

7- **Model Evaluation:** The model's performance is evaluated using R² score to measure the goodness of fit.

8- **Prediction Plot:** Forecast results are visualized with actual vs. predicted car sales in a forecast plot.

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

