# Oily Giant — Oil Well Region Selection

## Project Overview

This project aims to identify the most profitable region for developing 200 new oil wells for Oily Giant, an oil extraction company. The analysis evaluates geological data from three regions to estimate oil reserves, forecast potential profits, and assess investment risks.

The business scenario involves a $100 million investment, with a maximum acceptable probability of loss of 2.5%.

## Objectives

- Analyze geological data from three different regions.
- Train and evaluate a Linear Regression model for each region to predict oil reserves.
- Estimate the minimum oil reserve volume required to avoid losses.
- Calculate potential profits by selecting the 200 most promising wells from samples of 500 candidates.
- Use bootstrapping to estimate expected profits, confidence intervals, and the risk of losses.
- Recommend the region with the best balance between profitability and risk.

## Methodology

- **Data Exploration and Preparation:** Examined three datasets, each containing 100,000 oil well records. Checked data quality, descriptive statistics, and feature distributions.
- **Model Development:** Trained a separate Linear Regression model for each region using a 75/25 train-validation split.
- **Model Evaluation:** Compared model performance using Root Mean Squared Error (RMSE) and average predicted reserves.
- **Profit Estimation:** Calculated potential profits by selecting the 200 wells with the highest predicted reserves from samples of 500 candidates.
- **Risk Analysis:** Applied bootstrapping with 1,000 iterations to estimate average profit, 95% confidence intervals, and probability of losses.

## Results

**Model performance**

| Region | RMSE | Average Predicted Reserves |
|---|---:|---:|
| Region 0 | 37.58 | 92.59 |
| Region 1 | 0.89 | 68.73 |
| Region 2 | 40.03 | 94.97 |

**Bootstrapping results**

| Region | Average Profit (USD) | 95% Confidence Interval (USD) | Risk of Loss |
|---|---:|---:|---:|
| Region 0 | $6,007,352.44 | $129,483.31 – $12,311,636.06 | 2.00% |
| Region 1 | $6,652,410.58 | $1,579,884.81 – $11,976,415.87 | 0.30% |
| Region 2 | $6,155,597.23 | -$122,184.95 – $12,306,444.74 | 3.00% |

## Conclusion

Region 1 is the recommended location for new oil well development. It achieved the highest average expected profit of approximately **$6.65 million** and the lowest probability of loss at **0.30%**, comfortably below the company's maximum acceptable risk threshold of 2.5%.

Although Region 0 also met the risk requirement, Region 1 offers a better combination of expected profitability and lower investment risk. Region 2 was excluded because its probability of loss exceeded the acceptable threshold.

## Tools & Technologies

Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Linear Regression · Bootstrapping · Statistical Analysis

## Key Skills

Data Analysis · Exploratory Data Analysis (EDA) · Regression Modeling · Model Evaluation · Profit Estimation · Risk Assessment · Statistical Resampling

## Project Files

- `OilyGiant.ipynb` — Notebook containing data exploration, model training, profit calculations, bootstrapping, and final recommendations.

## How to View

Open `OilyGiant.ipynb` in GitHub to explore the analysis, code, visualizations, and results. The notebook is written in Spanish.
