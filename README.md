# 🏥 Medical Cost Prediction using Machine Learning

## Overview

This project develops and evaluates machine learning models to predict individual medical insurance expenses using demographic, lifestyle, and health-related information. Multiple regression algorithms were trained and compared to identify the most accurate predictive model while exploring the factors that contribute to healthcare costs.

## Objectives

- Predict individual medical insurance expenses.
- Perform exploratory data analysis to understand the dataset.
- Compare multiple machine learning regression models.
- Tune model hyperparameters using cross-validation.
- Evaluate and compare model performance using RMSE.
- Identify the most influential factors affecting medical expenses.

## Dataset

The dataset contains **25,000 observations** with demographic, lifestyle, medical, and insurance-related information.

### Features

- Age
- Gender
- Body Mass Index (BMI)
- Region
- Insurance Plan
- Smoking Status
- Chronic Conditions
- Daily Steps
- Previous Claims
- Medical Expenses (Target Variable)

## Machine Learning Workflow

```text
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Exploratory Data Analysis
   │
   ▼
Feature Engineering
   │
   ▼
Train/Test Split
   │
   ▼
10-Fold Cross Validation
   │
   ▼
Hyperparameter Tuning
   │
   ▼
Model Training
   │
   ▼
Model Evaluation
```

# Exploratory Data Analysis

The following visualisations provide an overview of the dataset and highlight important characteristics of the medical expenses.

## Distribution of Medical Expenses

The distribution of medical expenses is highly right-skewed, with most individuals incurring relatively low healthcare costs while a small number of observations represent very high medical expenses.

![](images/expense_distribution)

## Medical Expenses by Region

Medical expenses are compared across geographic regions to explore regional variations and identify potential differences in healthcare expenditure.

![](images/expenses_by_region)

## Medical Expenses by Insurance Plan

Medical expenses are compared across different insurance plan types to investigate how plan selection relates to healthcare expenditure.

![](images/expenses_by_plan_type)

# Machine Learning Models

The following regression models were developed and evaluated:

- Ridge Regression
- Random Forest
- K-Nearest Neighbours (KNN)

Hyperparameter tuning was performed using **10-fold cross-validation** to identify the optimal model configuration.

# Technologies Used

## Programming

- R

## Libraries

- tidymodels
- glmnet
- ranger
- kknn
- ggplot2
- dplyr
- recipes
- workflows
- rsample
- yardstick

# Results

| Model | Cross-Validated RMSE |
|----------------------|----------------:|
| Ridge Regression | **1786.40** |
| Random Forest | **1789.25** |
| K-Nearest Neighbours | **1835.17** |

The Ridge Regression model achieved the lowest cross-validated RMSE and demonstrated the best overall predictive performance on the test dataset.

Key predictors of medical expenses included:

- Chronic Conditions
- Smoking Status
- Age
- Body Mass Index (BMI)
- Previous Claims

# Repository Structure

```text
medical-cost-prediction/
│
├── README.md
├── LICENSE
│
├── data/
│   └── healthinsurance.csv
│
├── source/
│   └── medical_cost_prediction.qmd
│
├── report/
│   └── Medical_Cost_Prediction_Report.pdf
│
└── images/
    ├── expense_distribution
    ├── expenses_by_region
    └── expenses_by_plan_type
```

# Future Improvements

Potential extensions for this project include:

- Evaluate Gradient Boosting models such as XGBoost and LightGBM.
- Deploy the best-performing model as an interactive web application using Streamlit or Shiny.
- Incorporate explainable AI techniques such as SHAP values for model interpretation.
- Automate the machine learning workflow using reproducible pipelines.
- Investigate additional feature engineering techniques to further improve predictive performance.

# Skills Demonstrated

- Machine Learning
- Predictive Modelling
- Regression Analysis
- Feature Engineering
- Hyperparameter Tuning
- Cross-Validation
- Exploratory Data Analysis (EDA)
- Data Cleaning
- Model Evaluation
- Statistical Analysis
- Data Visualisation

# Author

**Sri Manju Baargavi Rangaraj Ganesh**
