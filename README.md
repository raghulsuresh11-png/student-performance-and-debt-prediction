
# Data-Driven Modelling of Student Academic Performance and Financial Debt in Higher Education

## Overview

This repository contains my Data Mining and Machine Learning project on modelling two important challenges in higher education using supervised machine learning:

1. predicting student academic outcomes
2. predicting student financial debt in higher education

The project applies classification and regression techniques to analyse how behavioural, demographic, institutional and financial factors influence student success and debt outcomes.
The aim of this project is to use machine learning to generate meaningful predictive insights from educational data and support better decision-making in higher education.

## Research Questions
- Do learning behaviour and personal attributes provide satisfactory methods for predicting student final results?
- Can institutional and socioeconomic variables be used to forecast student debt amounts?

# Datasets
### Dataset 1: Student Academic Performance
This dataset is based on the **Open University Learning Analytics Dataset (OULAD)** and is used to predict final student outcomes. It combines demographic, behavioural and assessment-related features such as:
- gender
- region
- highest education
- age band
- disability
- total VLE clicks
- average assessment score

The target variable is `final_result`, with four classes:
- Pass
- Fail
- Withdrawn
- Distinction

### Dataset 2: Student Debt Prediction
This dataset is based on the **U.S. Department of Education College Scorecard** and is used to predict median student debt at graduation (`DEBT_MDN`). Key features include:
- undergraduate enrollment (`UGDS`)
- admission rate (`ADM_RATE`)
- in-state tuition
- out-of-state tuition
- cost of attendance (`COSTT4_A`)
- Pell Grant recipient percentage (`PCTPELL`)
- institutional control type (`CONTROL`)

## Methodology
### Classification Models
- Logistic Regression
- Random Forest Classifier

### Regression Models
- Random Forest Regressor
- Gradient Boosting Regressor

## Data Preparation

### Dataset 1
- merged student information, assessment, and VLE interaction data
- encoded categorical variables
- imputed `total_clicks` and `avg_score` with 0 where appropriate
- used stratified train-test split

### Dataset 2
- converted selected features to numeric format
- handled missing values
- applied log transformation to skewed variables
- removed outliers using Z-score filtering
- scaled numeric features using StandardScaler

## Evaluation Metrics

## Classification
- Accuracy
- Precision
- Recall
- F1-score
- ROC AUC
- Confusion Matrix

## Regression
- R²
- Mean Squared Error (MSE)
- Residual analysis

## Key Results
### Dataset 1
- Logistic Regression achieved **61.7% accuracy**
- Random Forest achieved **60.1% accuracy**
- `total_clicks`, `avg_score`, and `highest_education` were among the most important predictors

### Dataset 2
- Random Forest Regressor achieved **R² = 0.51**
- Gradient Boosting Regressor achieved **R² = 0.46**
- tuition fees, cost of attendance, and admission rate were among the most influential predictors

## Repository Contents
- `DM_IEEE_FINAL.pdf` — final project report
- `Dataset1.ipynb` — notebook for student academic performance modelling
- `Dataset 2 (1).ipynb` — notebook for student debt prediction modelling

## Author
**Raghul Sureshbabu**

**Raghul Sureshbabu**
