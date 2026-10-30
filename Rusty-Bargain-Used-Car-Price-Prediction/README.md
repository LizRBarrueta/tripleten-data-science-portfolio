# Rusty Bargain — Used Car Price Prediction

## Project Overview

Rusty Bargain, a used car sales service, aims to develop an application that estimates the market value of vehicles based on their characteristics.

The objective of this project was to build and evaluate machine learning models, considering three key factors: prediction quality, training time, and prediction speed.

## Objectives

- Prepare and preprocess historical used car data.
- Analyze vehicle characteristics and their relationship with market prices.
- Train and compare different regression models.
- Evaluate model performance using RMSE.
- Measure training and prediction times.
- Recommend the model that offers the best balance between accuracy and computational efficiency.

## Methodology

- **Data Preparation:** Cleaned and preprocessed the dataset to prepare it for model training.
- **Exploratory Data Analysis:** Examined vehicle features and their relationship with market prices.
- **Model Development:** Trained and compared five regression algorithms: Linear Regression, Random Forest, XGBoost, LightGBM, and CatBoost.
- **Model Evaluation:** Compared models using RMSE, training time, and prediction time to assess both accuracy and computational efficiency.

## Results

The five models showed different levels of accuracy and computational performance.

| Model | RMSE | Training Time (s) | Prediction Time (s) |
|---|---:|---:|---:|
| Linear Regression | Highest | 8.10 | 0.17 |
| Random Forest | 1697.30 | 238.12 | — |
| XGBoost | 1653.27 | 458.51 | 0.49 |
| LightGBM | 1682.26 | 5.98 | 0.42 |
| CatBoost | 1777.84 | 6.05 | 0.01 |

*Note: The prediction time for Random Forest was not included in the reported results.*

## Conclusion and Recommendation

XGBoost achieved the lowest RMSE (1653.27), making it the most accurate model. However, its training time was considerably higher than that of the other alternatives.

CatBoost was selected as the recommended model because it offers a strong balance between prediction quality and computational efficiency:

- **Prediction Speed:** 0.01 seconds, the fastest among the evaluated models.
- **Training Time:** 6.05 seconds, allowing efficient model updates.
- **Prediction Accuracy:** RMSE of 1777.84, providing competitive performance for the intended application.

Given Rusty Bargain's need to provide fast vehicle price estimates, CatBoost represents the most suitable choice for this use case.

## Tools & Technologies

Python · Pandas · NumPy · Scikit-learn · XGBoost · LightGBM · CatBoost · Regression Modeling · RMSE

## Key Skills

Data Preprocessing · Exploratory Data Analysis (EDA) · Regression Modeling · Gradient Boosting · Model Comparison · Performance Evaluation · Hyperparameter Optimization

## Project Files

- Jupyter Notebook containing data preparation, exploratory analysis, model training, and evaluation.

## How to View

Open the notebook in GitHub to explore the analysis, code, and model comparisons. The notebook is written in Spanish.
