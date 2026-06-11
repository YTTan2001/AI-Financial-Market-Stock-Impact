# AI Financial Market Stock Impact Prediction
## Overview
This project focuses on predicting stock market impact driven by events using both **classical statistical methods** and **machine learning models**. 
It compares the performance of ARIMA (time-series statistical model) against a Random Forest regression model.
The key objective is to explore whether machine learning models can better capture **non-linear patterns** and **event-driven spikes** compared to traditional forecasting techniques.

## Objectives
1. Build a baseline forecasting model using ARIMA
2. Develop a Random Forest regression model for improved prediction
3. Evaluate and compare model performance using standard regression metrics
4. Analyze the influence of event-driven market behavior
5. Identify limitations of purely historical price-based forecasting
   
## Dataset
The dataset includes:
1. Historical stock market time-series data

** **Key observation:** Stock movements show strong volatility spikes during event occurrences, making them partially non-stationary and difficult to model accurately using only historical prices.

## Methodology
**1. Data Preprocessing**
- Handling missing values
-  Time-series alignment
- Feature engineering from historical price movements
- Event-based feature integration (where available)
  
**2. Models Used**
i. ARIMA (Baseline Model)
- Classical statistical time-series forecasting model
- Assumes linear relationships and stationarity
ii. Random Forest Regressor
- Ensemble machine learning model
- Captures non-linear relationships between features
- More robust to noisy financial data
  
## Evaluation Metrics
The models were evaluated using:
- MAE (Mean Absolute Error): 0.4653
- RMSE (Root Mean Squared Error): 0.6257
- R² Score: 0.5060
  
## Results Summary
- The Random Forest model outperformed the ARIMA baseline by approximately 15%
- However, overall predictive performance remains moderate
- The model explains about 50% of variance (R² ≈ 0.51) in stock impact

This suggests that while machine learning improves predictive power, stock market behavior remains highly **complex and partially unpredictable using historical data alone**.
