# Temperature Forecasting using Time Series Machine Learning

## Problem Statement

Accurate temperature forecasting is important for energy planning, agriculture, and environmental monitoring.  
This project builds a machine learning model to predict the next day's temperature using historical data.

---

## Dataset

Daily minimum temperature dataset.

Features:
- Historical temperature values
- Lag features (1,2,3,7,30 days)
- Seasonal encoding (sine/cosine transformation)

Target:
- Next day's temperature

---

## Approach

1. Converted date column to time index
2. Created lag features to capture temporal dependencies
3. Added seasonal encoding using sine and cosine transformation
4. Used time-based train-test split
5. Trained regression models

---

## Models Compared

- Linear Regression
- Random Forest Regressor

---

## Results

Linear Regression RMSE: **2.16**

Random Forest RMSE: **2.17**

Linear regression performed slightly better due to the smooth seasonal nature of temperature data.

---

## Key Insights

- Seasonal encoding significantly improved forecasting accuracy.
- Complex models did not outperform simpler regression models for this dataset.

---

## Technologies Used

- Python
- Pandas
- Scikit-learn
- NumPy
- Matplotlib
