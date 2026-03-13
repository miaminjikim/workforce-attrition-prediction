# workforce-attrition-prediction
Python project using machine learning to predict workforce attrition from structured HR-style data. Includes data cleaning, exploratory analysis, and logistic regression modeling with pandas and scikit-learn.

# Workforce Attrition Prediction

This project uses Python and machine learning to predict employee attrition based on structured workforce-related data. The goal is to move beyond descriptive analytics and explore how predictive modeling can support workforce planning and retention analysis.

## Project Overview

In many organizations, dashboards can summarize historical trends such as turnover, tenure, and employee characteristics. However, these descriptive tools often do not answer forward-looking questions, such as which employees are at greater risk of attrition. This project applies a supervised machine learning workflow to model attrition risk using a public dataset.

## Objective

The objective of this project is to:

- clean and prepare workforce-style tabular data
- explore patterns associated with attrition
- build a predictive model in Python
- evaluate model performance
- identify variables most associated with attrition

## Dataset

This project uses the IBM HR Analytics/Employee Attrition dataset, publicly available on Kaggle.

Dataset source:
[IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

The dataset contains employee-level variables such as:

- age
- department
- job role
- monthly income
- years at company
- overtime
- business travel
- attrition outcome

## Tools and Libraries

- Python
- pandas
- numpy
- matplotlib
- scikit-learn

## Methods

The workflow for this project included:

1. Data loading and inspection
2. Data cleaning and preprocessing
3. Exploratory data analysis
4. Encoding categorical variables
5. Train-test split
6. Logistic regression modeling
7. Model evaluation using classification metrics

## Model

A logistic regression model was used as a baseline classifier to predict whether an employee would leave the organization.

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

The model was evaluated using standard classification metrics such as:

- accuracy
- confusion matrix
- precision / recall

While this is a simplified project using public data, it demonstrates how Python-based modeling can support workforce analytics beyond descriptive dashboards.

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
