# Credit-Risk-Modeling

This project focuses on estimating Probability of Default (PD) using different machine learning models and performing risk-based portfolio evaluations such as Expected Loss (EL), Exposure at Default (EAD), and Loss Given Default (LGD).


1️⃣ Project Objective

Compare different machine learning models for PD prediction:

Logistic Regression

Decision Tree

Random Forest

Gradient Boosting

Use the PD predictions to calculate Expected Loss (EL), Exposure at Default (EAD), and Loss Given Default (LGD).

Identify high-risk loan segments for portfolio risk assessment.

2️⃣ Data Loading & Overview

Dataset: Credit Risk Dataset on Kaggle

Columns include:

person_age, person_income, person_home_ownership, person_emp_length

loan_intent, loan_grade, loan_amnt, loan_int_rate, loan_status

loan_percent_income, cb_person_default_on_file, cb_person_cred_hist_length

Initial steps:

Check missing values and data types

Understand distributions of numeric and categorical features

3️⃣ Data Cleaning & Preprocessing

Handle missing values using median/mode or KNN imputation

Detect and treat outliers using IQR or z-score methods

Remove duplicate rows

Encode categorical variables:

OneHot Encoding for loan_intent and loan_grade

Label Encoding where appropriate

Feature scaling: StandardScaler or MinMaxScaler applied to numeric features

4️⃣ Exploratory Data Analysis (EDA)

Visualizations:

Histograms, boxplots, and density plots for numeric features

Value counts for categorical variables to check class balance

Correlation matrix and pairplots to examine feature relationships

Extracted insights to understand patterns affecting loan defaults

5️⃣ Feature Selection

Selected features based on:

Correlation analysis

Feature importance from tree-based models

Ensured models are trained on meaningful variables only

6️⃣ PD Model Training

Models trained:

Logistic Regression

Decision Tree

Random Forest

Gradient Boosting

Hyperparameter tuning with GridSearchCV

Evaluation metrics:

Accuracy, Precision, Recall, F1-Score

ROC-AUC

Cross-validation with K-Fold for robust performance

7️⃣ Risk Metrics Calculation

PD (Probability of Default): Risk of borrower default

EAD (Exposure at Default): Loan amount at risk (loan_amnt)

LGD (Loss Given Default): Estimated loss proportion by loan type

Example mappings: Personal/Education: 0.85, HomeImprovement/Medical: 0.60, Venture: 0.90

Portfolio-level analysis:

Total and average EL

Average EL by loan type

PD distribution and EL visualizations

8️⃣ Key Insights

Gradient Boosting performed best in PD prediction

Certain loan types present higher expected losses, identifying higher-risk segments

Visualizations provide actionable insights for portfolio risk management
