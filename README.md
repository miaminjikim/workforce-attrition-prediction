# Project Description
Python project using machine learning to predict workforce attrition from structured HR-style data. Includes data cleaning, exploratory analysis, and logistic regression modeling with pandas and scikit-learn.

# Workforce Attrition Prediction

## Overview

Employee attrition is a critical challenge for organizations because losing experienced employees can lead to increased recruitment costs, loss of expertise, and reduced productivity.

This project develops a machine learning model to predict employee attrition using the IBM HR Analytics dataset. The goal is to identify key factors that contribute to employee turnover and help organizations take proactive steps to improve retention.

The analysis applies Logistic Regression and Random Forest models to classify whether an employee is likely to leave the company.

## Dataset

The dataset used in this project is the IBM HR Analytics Employee Attrition Dataset.
It contains information about employee demographics, job characteristics, compensation, and work conditions.

The dataset contains employee-level variables such as:

- age
- overtime status
- monthly income
- attrition outcome (target variable)
- job role
- department
- years at company
- job satisfaction

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

## Model

A logistic regression model was used as a baseline classifier to predict whether an employee would leave the organization. Logistic regression was used as a baseline model, while a Random Forest classifier was tested as a non-linear alternative.

This model was selected because it is:

- interpretable
- appropriate for binary classification
- commonly used in attrition and retention analysis

## Key Findings

Key variables associated with higher attrition included:

- overtime
- lower tenure
- certain job roles
- lower monthly income
- more frequent business travel

These findings suggest that predictive analytics can complement traditional HR reporting by identifying patterns linked to retention risk.

## Results

A logistic regression model was trained using standardized features within a scikit-learn pipeline.

Model performance on the test dataset:

- Accuracy: **89.1%**
- ROC-AUC: **0.77**
- Precision (Attrition class): **0.68**
- Recall (Attrition class): **0.33**
- F1-score (Attrition class): **0.45**

The model performs strongly in identifying employees who remain with the organization. Predicting attrition is more challenging due to the smaller number of attrition cases in the dataset.

The ROC-AUC score of 0.77 indicates that the model still demonstrates good ability to distinguish between employees who stay and those who leave.

The lower recall for the attrition class reflects class imbalance in the dataset, which is common in workforce attrition prediction problems.

These results demonstrate how predictive models can complement traditional HR reporting by identifying patterns associated with workforce attrition risk. 

## Tools and Libraries

- Python
- pandas
- numpy
- matplotlib
- scikit-learn

## Repository Contents

- `attrition_prediction.ipynb` — main notebook
- `README.md` — project summary
- `data/` — dataset file if included
- `requirements.txt` — optional package list

## Future Improvements

Possible next steps include:

- testing additional models such as random forest or XGBoost
- performing feature selection
- tuning hyperparameters
- improving class imbalance handling
- comparing interpretability versus predictive performance

## Why I Built This Project

My professional background in HR and workforce analytics has shown me that many organizational questions cannot be answered through reporting alone. I built this project to strengthen my technical skills in Python, statistical modeling, and machine learning, and to explore how predictive methods can support evidence-based workforce decision-making.

## Author

Minji Kim  
GitHub: [your GitHub profile link]
