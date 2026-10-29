# Beta Bank — Customer Churn Prediction

## Project Overview
Developed a machine learning classification model to predict whether a bank customer is likely to leave. The objective was to achieve an F1-score of at least 0.59 to support customer retention efforts.

## Objectives
- Prepare and preprocess customer data for machine learning.
- Address class imbalance and compare different balancing techniques.
- Train and evaluate classification models.
- Select a model meeting the required F1-score threshold.

## Methodology
- **Data Preprocessing:** Removed irrelevant columns, imputed missing `Tenure` values using the median, encoded categorical variables with `OneHotEncoder`, and standardized numerical features with `StandardScaler`.
- **Class Imbalance:** Analyzed the target distribution (79.63% vs. 20.37%) and compared `class_weight`, upsampling, and downsampling.
- **Model Selection:** Compared three classification algorithms using three balancing approaches, evaluating nine model configurations in total.
- **Evaluation Metrics:** Used F1-score and ROC-AUC to assess classification performance.

## Final Results
- **Final model:** Random Forest Classifier
- **F1-score:** 0.5927
- **ROC-AUC:** 0.8459
- **Required F1-score:** 0.59 — achieved

During model comparison, Random Forest with upsampling achieved an F1-score of 0.6053. The final model achieved an F1-score of 0.5927, meeting the project's minimum requirement.

## Tools & Technologies
Python · Pandas · NumPy · Scikit-learn · OneHotEncoder · StandardScaler · Random Forest

## Key Skills
Data Preprocessing · Classification · Class Imbalance Handling · Upsampling · Downsampling · Feature Encoding · Feature Scaling · Model Evaluation · Hyperparameter Tuning

## Business Outcome
Built a classification model that met the project's minimum F1-score requirement and achieved a ROC-AUC of 0.8459. The model can help the bank identify customers at risk of churn and prioritize retention efforts.

## Project Files
- `BetaBank_churn.ipynb` — Notebook containing the data preprocessing, model comparison, and final evaluation.

## How to View
Open `BetaBank_churn.ipynb` in GitHub to explore the analysis, code, and saved outputs. The notebook is written in Spanish.
