# Zyfra — Gold Recovery Prediction

## Project Overview

This project focuses on developing a machine learning model to predict gold recovery efficiency at different stages of the gold extraction and purification process for Zyfra, a mining company.

The goal is to improve production efficiency by accurately predicting gold recovery rates and supporting better operational decision-making.

## Objectives

- Prepare and analyze historical data from the gold extraction process.
- Validate the calculation of gold recovery efficiency.
- Investigate metal concentrations and particle size distributions throughout the purification stages.
- Identify and handle missing values and anomalous observations.
- Train and evaluate machine learning models to predict gold recovery.
- Select the best-performing model based on the Symmetric Mean Absolute Percentage Error (sMAPE).

## Methodology

- **Data Preparation:** Cleaned and preprocessed the datasets, handled missing values, and removed anomalous observations.
- **Exploratory Data Analysis:** Analyzed metal concentrations (gold, silver, and lead) throughout the extraction stages and compared particle size distributions between training and test datasets.
- **Feature Analysis:** Examined relationships between process variables and gold recovery efficiency.
- **Model Development:** Trained and compared regression models, including Random Forest, using cross-validation.
- **Model Evaluation:** Evaluated model performance using weighted sMAPE and compared results against a Dummy baseline model.

## Results

**Best-performing model: Random Forest**

| Evaluation | Weighted sMAPE |
|---|---:|
| Cross-validation | 9.27 |
| Test set | 9.87 |
| Dummy baseline | 10.09 |

The Random Forest model achieved better predictive performance than the Dummy baseline, demonstrating its ability to estimate gold recovery more effectively.

## Conclusion

Random Forest was identified as the most robust model, achieving a weighted sMAPE of 9.27 during cross-validation and 9.87 on the test set, outperforming the Dummy baseline (10.09).

The results support the potential use of machine learning to improve gold recovery predictions and contribute to more efficient mining operations.

## Recommendations

- **Controlled Deployment:** Implement the Random Forest model in a production environment to begin optimizing gold recovery.
- **Continuous Monitoring:** Track sMAPE performance to detect deviations and determine when model adjustments are needed.
- **Economic Impact Analysis:** Quantify the financial implications of the model's prediction error to assess whether its performance meets operational requirements.
- **Continuous Improvement:** Further optimize hyperparameters to explore opportunities for reducing prediction error.

## Tools & Technologies

Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Random Forest · Regression Modeling · Cross-Validation

## Key Skills

Data Preprocessing · Exploratory Data Analysis (EDA) · Feature Engineering · Regression Modeling · Model Evaluation · Cross-Validation · Hyperparameter Optimization

## Project Files

- `Zyfra_Gold_Recovery.ipynb` — Notebook containing data preparation, exploratory analysis, model training, and evaluation.

## How to View

Open the notebook in GitHub to explore the analysis, code, visualizations, and model evaluation. The notebook is written in Spanish.