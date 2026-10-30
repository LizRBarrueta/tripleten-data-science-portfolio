# Sweet Lift Taxi — Taxi Order Forecasting

## Project Overview

Sweet Lift Taxi, a taxi service company, aims to improve driver availability during peak hours by accurately forecasting taxi order demand.

The objective of this project was to develop a machine learning model capable of predicting the number of taxi orders for the next hour, helping the company better allocate its resources.

## Objectives

- Analyze historical taxi order data and identify demand patterns.
- Explore hourly and daily seasonality.
- Prepare time-based features for model training.
- Train and optimize regression models to forecast taxi demand.
- Evaluate model performance using RMSE.
- Achieve an RMSE below the project target of 48.

## Methodology

- **Data Preparation:** Processed historical taxi order data and prepared it for time series forecasting.
- **Exploratory Data Analysis:** Analyzed demand patterns, hourly seasonality, and fluctuations over time.
- **Feature Engineering:** Created lagged features to capture relationships between past and future demand.
- **Model Development:** Trained and optimized multiple regression models, including LightGBM.
- **Model Evaluation:** Compared predictions against actual values and analyzed residuals to assess model performance.

## Results

<badge color="success">Project RMSE target achieved</badge>

**Best-performing model: Optimized LGBM Regressor**

| Model | Test RMSE |
|---|---:|
| Optimized LGBM Regressor | 40.35 |
| Naive Model | 58.88 |
| Project target | Below 48 |

The optimized LGBM Regressor achieved an RMSE of 40.35, outperforming the Naive baseline and meeting the project's performance requirement.

## Key Findings

- Lagged demand features, particularly `lag_23`, `lag_24`, `lag_18`, `lag_17`, and `lag_19`, were among the most influential predictors.
- The hour of the day was also an important feature due to daily demand seasonality.
- The model captured general demand trends and daily patterns but had some difficulty predicting extreme demand peaks.
- Residuals were centered around zero, suggesting no significant systematic bias, although some large errors remained.

## Conclusion and Recommendations

The optimized LGBM Regressor was selected as the best-performing model, achieving an RMSE of 40.35 on the test set.

Its performance exceeded the project target and significantly improved upon the Naive baseline (58.88).

Recommendations for further improvement include:

- Investigating periods with the largest prediction errors to identify external factors affecting demand, such as weather conditions or special events.
- Incorporating relevant external variables when available.
- Retraining the model periodically with updated data to adapt to changing demand patterns.

## Tools & Technologies

Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · LightGBM · Time Series Analysis · Feature Engineering

## Key Skills

Time Series Forecasting · Data Preprocessing · Exploratory Data Analysis (EDA) · Feature Engineering · Regression Modeling · Model Optimization · Model Evaluation · Residual Analysis

## Project Files

- Jupyter Notebook containing data preparation, exploratory analysis, feature engineering, model training, and evaluation.

## How to View

Open the notebook in GitHub to explore the analysis, code, visualizations, and model evaluation. The notebook is written in Spanish.