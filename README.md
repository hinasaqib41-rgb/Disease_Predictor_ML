# Disease_Predictor_ML
Disease Prediction - Heart Disease Classifier using Machine Learning
Heart Disease Prediction using Machine Learning

Predict heart disease risk using clinical data with Logistic Regression and Random Forest models.

This project was built as part of a health-focused AI bootcamp. It provides an end-to-end pipeline for predicting heart disease presence using the UCI Heart Disease Dataset, with tools for model training, evaluation, feature analysis, and user-driven prediction.

📌 Project Overview

Heart disease remains a leading cause of death globally. This project applies machine learning to clinical data to predict whether a patient is likely to have heart disease. The workflow includes:

Downloading & preparing data from Kaggle

Handling missing values

Exploratory Data Analysis (EDA)

Feature encoding & scaling

Model training: Logistic Regression & Random Forest

Performance evaluation

Saving models

Real-time prediction with uploaded CSV files

📁 Dataset Source

Kaggle Dataset: Heart Disease Data by Redwankarimsony

Data includes demographic, clinical, and ECG attributes

Target: num (0 = no heart disease, 1+ = presence of heart disease)

⚙️ Features Used

Numerical Features: age, trestbps, chol, thalch, oldpeak, ca

Categorical Features: sex, cp (chest pain), thal, slope, restecg, dataset

Boolean Features: fbs (fasting blood sugar), exang (exercise-induced angina)

All features are one-hot encoded and scaled before model training.

🧪 Machine Learning Pipeline
✔️ 1. Preprocessing

Missing numerical values → filled with mean

Categorical columns → filled with 'Unknown' (if needed)

Booleans → cast to integers

One-hot encoding applied to all categorical variables

✔️ 2. Modeling

Logistic Regression

Accuracy: 84.23%

F1-score: 0.87 (heart disease), 0.81 (no disease)

Random Forest Classifier

Accuracy: 88.04%

Used for final prediction due to better generalization

✔️ 3. Evaluation

Confusion Matrix, Precision, Recall, F1-Score

Feature Importance (via Random Forest)

✔️ 4. Prediction

Saved model with joblib

Custom CSV file uploads for new predictions

Output appended with Heart_Disease_Prediction column (0 = No, 1 = Yes)
