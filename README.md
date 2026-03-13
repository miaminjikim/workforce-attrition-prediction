# Project Description
Machine learning project predicting employee attrition using Logistic Regression and Random Forest with HR analytics insights and feature importance analysis.

# Workforce Attrition Prediction

## Overview

Employee attrition is a critical challenge for organizations because losing experienced employees can lead to increased recruitment costs, loss of expertise, and reduced productivity.

This project develops a machine learning model to predict employee attrition using the IBM HR Analytics dataset. The goal is to identify key factors that contribute to employee turnover and help organizations take proactive steps to improve retention.

The analysis applies Logistic Regression and Random Forest models to classify whether an employee is likely to leave the company.

## Dataset

The dataset used in this project is the IBM HR Analytics Employee Attrition Dataset.
It contains information about employee demographics, job characteristics, compensation, and work conditions.

Key variables include:

- Age
- Overtime status
- Monthly income
- Attrition outcome (target variable)
- Job role
- Department
- Years at company
- Job satisfaction

Dataset source:
[IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

## Project Workflow

The analysis follows a standard machine learning workflow:

1. Data loading and inspection
2. Data preprocessing
3. Feature Encoding
4. Train-test split
5. Model Training
6. Model Evaluation
7. Feature Importance Analysis

## Models Implemented

A logistic regression model was used as a baseline classifier, while a Random Forest classifier was tested as a non-linear alternative.

## Logistic Regression

A logistic regression classifier was trained to predict employee attrition.

To improve convergence and model stability, the pipeline includes:
- StandardScaler
- Logistic Regression (max_iter = 5000)

Performance
Accuracy: 0.89

Classification Report:

| Class | Precision | Recall | F1-score | 
|------|------|------|------|
No Attrition | 0.91 | 0.98 | 0.94
Attrition | 0.68 | 0.33 | 0.45

The model performs well for predicting employees who remain in the company, though recall for attrition cases is lower due to class imbalance in the dataset.

## Random Forest

A Random Forest classifier was trained to capture potential nonlinear relationships between features and employee attrition.

Model parameters:
- n_estimators = 200
- random_state = 42

Performance
Accuracy: 0.87

Although slightly lower than Logistic Regression in terms of accuracy, the Random Forest model provides useful insights through feature importance analysis.

## Model Performance

| Model | Accuracy | ROC-AUC |
|------|------|------|
Logistic Regression | 0.89 | 0.77 |
Random Forest | 0.87 | — |

## Model Comparison

Model	Accuracy
Logistic Regression	0.89
Random Forest	0.87

Logistic Regression slightly outperformed Random Forest in this dataset.

## ROC-AUC Evaluation

ROC-AUC was used to evaluate the model's ability to distinguish between employees who leave and those who stay.

ROC-AUC Score:
0.77

This indicates the model has a reasonable ability to discriminate between attrition and non-attrition cases.

## Key Predictors of Attrition

Feature importance analysis from the Random Forest model identified several important predictors of employee turnover:

- Monthly Income
- Overtime
- Age
- Daily Rate
- Job-related compensation variables

These factors suggest that workload, compensation, and employee demographics play important roles in employee retention.

## Tools and Libraries

- Python
- Pandas
- Numpy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Repository Contents

- `attrition_prediction.ipynb` — main notebook
- `README.md` — project summary
- `WA_Fn-UseC_-HR-Employee-Attrition.csv` — dataset file 

## Future Improvements

Possible next steps include:

- Handling class imbalance using SMOTE
- Testing additional models such as XGBoost
- Hyperparameter tuning
- Feature engineering
- Cross-validation
- Building a dashboard for HR decision-making

## Why I Built This Project

This project was developed as part of my exploration of machine learning applications in workforce analytics and people data science.

## Author

Minji Kim  
GitHub: [https://github.com/miaminjikim]
