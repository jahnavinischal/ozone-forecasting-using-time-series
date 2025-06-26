
# Ozone Forecasting using Time Series Analysis

This project applies time series modeling techniques to forecast the depletion of the ozone layer, focusing on the maximum ozone hole area over Antarctica from 1979 to 2020. The objective is to predict future trends and evaluate model performance using both statistical and machine learning approaches.

---

## 📊 Dataset

- Source: [Kaggle - Ozone Layer Dataset](https://www.kaggle.com/datasets/programmerrdai/ozone-layer)
- Time Period: 1979–2020
- Features Used:
  - Year
  - Maximum ozone hole area (NASA)
  - Mean ozone hole area
  - ODS Consumption

---

## 🔧 Tools & Libraries

- Python 
- pandas, numpy
- matplotlib, seaborn
- statsmodels (ARIMA, SARIMA, Holt-Winters)
- pmdarima (auto_arima)
- scikit-learn (KNN)
- plotly

---

## 🧪 Modeling Workflow

1. Data Preprocessing:
   - Removed irrelevant columns
   - Applied log transformation
   - Interpolated missing values
   - Resampled data using time-based index

2. Stationarity Tests:
   - ADF (Augmented Dickey-Fuller)
   - KPSS

3. Models Implemented:
   - ARIMA (on log-transformed and non-transformed data)
   - SARIMA
   - Auto ARIMA
   - Exponential Smoothing (Holt-Winters)
   - K-Nearest Neighbors (KNN)

4. Model Diagnostics:
   - Residual analysis using ACF, PACF
   - Ljung-Box test

5. Forecasting & Evaluation:
   - Forecasted values from 2021–2030
   - Metrics used: MAE, MSE, RMSE

---

## 📈 Results Summary

- Best model: Auto ARIMA (2,2,1) based on AIC and test metrics
- Log-transformed ARIMA showed stable forecasts
- KNN and Exponential Smoothing models underperformed
- Overall trend forecast indicates gradual decline in ozone hole area

---

## 🚀 Future Enhancements

- Add deep learning models (LSTM/GRU)
- Incorporate external climate variables
- Deploy as a Streamlit dashboard

---

## 📄 Auto ARIMA Forecast Screenshot:
![ozone pred](https://github.com/user-attachments/assets/aeaf0a7b-4e87-4a69-8bfb-66b7987b89b9)


