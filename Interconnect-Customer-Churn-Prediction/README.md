# Interconnect — Customer Churn Prediction

## Business Problem

Interconnect, a telecommunications provider, was experiencing customer churn and needed a way to identify subscribers at risk of canceling their services. Since retaining existing customers is generally less expensive than acquiring new ones, the goal was to develop a predictive model that could help the company take proactive retention measures and reduce potential revenue losses.

## Tools & Technologies

Python, Pandas, NumPy, SciPy, Scikit-learn, Matplotlib, Seaborn, Exploratory Data Analysis (EDA), Feature Engineering, One-Hot Encoding, Standardization, Support Vector Machines (SVM), Logistic Regression, Decision Trees, Random Forest, Gradient Boosting, Cross-Validation, and Hyperparameter Optimization.

## Project Highlights

- Performed exploratory data analysis to identify customer behavior patterns and factors associated with churn.
- Prepared and transformed data through feature engineering, categorical encoding, and numerical standardization.
- Calculated contract duration and created relevant features for model training.
- Trained and compared multiple classification algorithms using cross-validation.
- Optimized model performance and evaluated results using AUC-ROC, Recall, and confusion matrices.
- Selected a Support Vector Machine (SVM) with a linear kernel as the final model.

## Model Performance

The selected SVM model achieved the following results on the test set:

- **AUC-ROC:** 0.8314
- **Recall:** 82.09%
- **Customers at risk correctly identified:** 307 out of 374 actual churners.

Recall was particularly important for this project because identifying customers who are likely to leave allows the company to intervene before losing them.

## Business Impact & ROI Simulation

An annualized financial simulation was developed to estimate the potential business value of implementing the selected churn prediction model.

The scenario assumes that 50% of the 307 customers correctly identified as at risk (153 customers) accept a targeted retention incentive consisting of a $15 monthly discount for one year.

### Projected Financial Results

| Financial Concept | Projected Value (USD) |
|---|---:|
| Estimated revenue loss without intervention (status quo) | $274,236.96 |
| Gross revenue recovered (153 retained customers) | $136,671.84 |
| Retention campaign investment (discounts) | $27,540.00 |
| **Projected annual net savings** | **$109,131.84** |

These figures represent a hypothetical financial projection based on the assumptions defined in the executive presentation. They should not be interpreted as actual realized savings.

## Strategic Implementation Recommendation

Deploy the model to support automated monthly customer risk segmentation. Prioritize fiber-optic customers with month-to-month contracts and offer targeted incentives to encourage migration to one-year contracts.

This approach aims to improve customer retention while making more efficient use of the company's marketing budget.

## Project Files

- Jupyter Notebook: Model development, evaluation, and analysis.
- Executive Presentation (PDF): `Presentacion_Ejecutiva_Churn_SVM.pdf`, including model performance, projected ROI, and strategic implementation recommendations.

