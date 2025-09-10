Student Performance Prediction
1. Overview

This project predicts student final grades based on demographic, academic, and social factors.
It demonstrates an end-to-end ML workflow: from preprocessing → EDA → → model training → evaluation.
The repository is structured for clarity, reproducibility, and professional presentation.

2. Dataset

Source: UCI Machine Learning Repository – Student Performance https://archive.ics.uci.edu/dataset/320/student+performance

student-por.csv – Portuguese course performance

Features:

Demographics: Age, gender, family background

Academic Info: Study time, past failures, absences

Social Factors: Family support, free time, alcohol use, relationships

Target: Final Grade (G3, numeric score 0–20)

Dataset description is in data/README.md.

3. Methodology

Exploratory Data Analysis (EDA):

Distribution of grades and demographic variables

Correlations between features and final grade

Visualization of social and academic factors

Preprocessing:

Handle missing values

Encode categorical features (OneHot/Label encoding)

Scale numerical features

Modeling:

Linear Regression, Ridge, Lasso

Support Vector Regression (SVR)

Random Forest, Gradient Boosting, XGBoost

Artificial Neural Network (ANN)

Evaluation:

Metric: Mean Absolute Error (MAE)

Train/Test split ratio: 80:20

4. Results

Best Model: Support Vector Regression (SVR)
Best MAE: 0.667
Top Predictors: Study time, absences, family support, alcohol consumption
Insight: SVR captured non-linear relationships most effectively, making it the most reliable model for predicting student grades.
