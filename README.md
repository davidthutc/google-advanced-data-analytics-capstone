# google-advanced-data-analytics-capstone
This repository contains the completed project for the Google Advanced Data Analytics Capstone. The project focuses on leveraging advanced data analytics techniques to predict employee attrition using a real-world HR dataset.

## Overview
This project aims to predict employee turnover (retention or resignation) using machine learning models. The dataset contains features such as employee satisfaction level, last evaluation score, and tenure, which were used to build predictive models. The goal is to identify patterns and key factors contributing to employee attrition, enabling organizations to take proactive measures.

## Features
- **Dataset**: The HR dataset contains 14,999 rows and 10 columns, including variables like employee satisfaction, evaluation scores, number of projects, tenure, and salary.
- **Prediction Task**: Binary classification to predict whether an employee left the company (`left = 1`) or stayed (`left = 0`).
- **Models Evaluated**:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Random Forest
  - XGBoost
  - LightGBM
  - CatBoost

## Key Steps
1. **Data Preprocessing**:
   - Renamed columns for consistency.
   - Removed duplicate rows.
   - Checked for missing values and outliers.
   - Encoded categorical variables.
   - Standardized numerical features for specific models (e.g., Logistic Regression, SVM).

2. **Exploratory Data Analysis (EDA)**:
   - Visualized relationships between variables.
   - Plotted distributions and correlation heatmaps.
   - Highlighted key trends influencing employee turnover.

3. **Model Building and Evaluation**:
   - Implemented models with k-fold cross-validation for robust evaluation.
   - Evaluated performance using:
     - AUC-ROC
     - Precision
     - Recall
     - Accuracy
     - F1-Score
   - Compared model performance and selected the best models for deployment.

4. **Insights and Recommendations**:
   - Identified key factors influencing turnover (e.g., satisfaction level, working hours, tenure).
   - Recommended actionable steps for employee retention based on model insights.

## Results
| Model                  | K-Fold AUC-ROC Mean | Test Accuracy | Precision | Recall | F1-Score |
|-------------------------|---------------------|---------------|-----------|--------|----------|
| Logistic Regression     | 0.793               | 83.02%        | 47.98%    | 15.75% | 23.72%   |
| Support Vector Machine  | 0.968               | 97.25%        | 93.15%    | 90.22% | 91.66%   |
| Random Forest           | 0.980               | 98.30%        | 98.39%    | 91.38% | 94.75%   |
| XGBoost                 | 0.980               | 98.03%        | 96.67%    | 91.38% | 93.95%   |

**Best Performing Models**: Random Forest and XGBoost with nearly identical metrics.
