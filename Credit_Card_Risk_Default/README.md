# Loan Status Classification using Credit Risk Dataset

## Overview
This project focuses on predicting the loan status (whether a loan will default or not) using a Credit Risk Dataset that contains simulated credit bureau data. The goal is to develop a machine learning model that can classify loan applications as either likely to default or not based on various features related to the applicant's financial and personal background.

**Dataset** : https://www.kaggle.com/datasets/laotse/credit-risk-dataset 

## Dataset Description
The dataset includes the following features:

- person_age: The age of the loan applicant.
- person_income: The annual income of the applicant.
- person_home_ownership: The home ownership status of the applicant.
- person_emp_length: The length of employment of the applicant in years.
- loan_intent: The intent behind taking the loan.
- loan_grade: The grade assigned to the loan application.
- loan_amnt: The amount of loan applied for.
- loan_int_rate: The interest rate of the loan.
- loan_status: The target variable indicating loan status (0 for non-default, 1 for default).
- loan_percent_income: The percentage of income allocated to the loan.
- cb_person_default_on_file: Historical default status of the applicant.
- cb_preson_cred_hist_length: The length of the applicant's credit history.

## Project Objective
The objective of this project is to build a robust classification model that can accurately predict the loan status based on the features provided. This model will help in assessing the risk associated with a loan application, aiding financial institutions in making informed lending decisions.

## Methodology
- **Data Preprocessing:** Clean and preprocess the dataset to handle missing values, categorical variables, and scale numerical features.
- **Modeling:** Train various machine learning models, such as Logistic Regression, Decision Trees, and Random Forests, to classify the loan status.
- **Evaluation:** Evaluate the performance of the models using metrics like accuracy, precision, recall, and ROC-AUC score.

## Model Performance Summary
| **Model**                              | **Accuracy (%)** |
|------------------------------------|--------------|
| MultiNomialNB                      | 65.85        |
| SVM                                | 79.26        |
| BernoulliNB                        | 79.32        |
| Logistic Regression                | 80.10        |
| Naive Bayes                        | 81.06        |
| K-Nearest Neighbors (KNN)          | 83.08        |
| Randomized Random Tree Classifier  | 84.07        |
| Random Decision Tree               | 85.49        |
| Decision Tree                      | 88.45        |
| Gradient Boosting Machine (GBM)    | 91.07        |
| Random Tree Classifier             | 92.18        |
| CatBoost                           | 93.00        |
| XGBoost                            | 93.07        |
