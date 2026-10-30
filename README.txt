# Sure Tomorrow — Insurance Machine Learning

## Business Problem

Sure Tomorrow, an insurance company, wanted to explore how machine learning could support customer identification, insurance benefit prediction, and personal data protection.

The project focused on evaluating different machine learning approaches while examining how data preprocessing and obfuscation techniques affect model performance and customer privacy.

## Tools & Technologies

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, K-Nearest Neighbors (kNN), Linear Regression, Feature Scaling, Data Obfuscation, and Model Evaluation.

## Project Highlights

The project addressed four main tasks:

### 1. Customer Similarity

- Explored customer similarity using distance-based algorithms.
- Applied feature scaling to improve the reliability of distance calculations.
- Compared similarity results using original and scaled data.

### 2. Customer Classification

- Used K-Nearest Neighbors (kNN) to identify customers belonging to a specific group.
- Evaluated the impact of feature scaling on classification performance.
- Improved the F1-score from 0.68 to 0.93 through appropriate feature scaling.

### 3. Insurance Benefit Prediction

- Developed a Linear Regression model to predict insurance benefits.
- Compared model performance using original and scaled features.
- Evaluated predictions using RMSE and R².

**Model Performance:**
- **RMSE:** 0.36
- **R²:** 0.43

The results remained identical with both original and scaled data, demonstrating the model's robustness to feature scaling.

### 4. Data Obfuscation and Privacy Protection

- Implemented a data obfuscation technique by multiplying the feature matrix (X) by an invertible matrix (P).
- Demonstrated analytically and computationally that the transformation preserves Linear Regression predictions.
- Verified that RMSE and R² remain unchanged after data obfuscation.
- Explored how mathematical transformations can help protect sensitive customer information without compromising predictive performance.

## Key Findings

- Feature scaling is crucial for distance-based algorithms such as kNN, as it prevents features with larger numerical ranges from dominating distance calculations.
- Proper scaling significantly improved classification performance, increasing the F1-score from 0.68 to 0.93.
- Linear Regression proved robust to feature scaling, maintaining an RMSE of 0.36 and an R² of 0.43.
- Data obfuscation using an invertible matrix preserved Linear Regression predictions and evaluation metrics.
- Mathematical data transformations offer a potential approach to protecting customer privacy while maintaining model effectiveness.

## Business Impact

The project demonstrated how machine learning can support insurance operations through customer similarity analysis and benefit prediction.

It also highlighted a potential privacy-preserving approach that allows sensitive customer data to be transformed without affecting the predictive performance of Linear Regression models.

These findings can help inform the development of machine learning solutions in environments where personal data protection is essential.

## Key Skills Demonstrated

Machine Learning, Customer Similarity Analysis, Classification, Regression, Feature Scaling, K-Nearest Neighbors, Linear Regression, Model Evaluation, Data Obfuscation, Privacy Protection, and Mathematical Analysis.

## Project Files

- Jupyter Notebook: Customer similarity, classification, insurance benefit prediction, and data obfuscation.
- README: Project overview, methodology, results, and conclusions.