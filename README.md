🫀 Heart Disease Prediction Using Machine Learning
📌 Overview
This project predicts whether a person is at risk of heart disease using medical attributes. It uses the Heart Disease UCI Dataset and implements machine learning models (Logistic Regression and Decision Tree Classifier) to classify patients into:

0 = No Heart Disease

1 = At Risk of Heart Disease

The project is structured to include data preprocessing, feature scaling, model training, evaluation, and visualization.

🎯 Objective
Predict heart disease risk from patient health metrics.

Build and evaluate classification models.

Identify important health features contributing to risk.

Visualize performance using ROC curve and feature importance.

📊 Dataset Details
Dataset: Heart Disease UCI

🔑 Features:
Feature	Description
age	Age of the patient
sex	1 = Male, 0 = Female
cp	Chest pain type (0–3)
trestbps	Resting blood pressure
chol	Serum cholesterol (mg/dl)
fbs	Fasting blood sugar > 120 mg/dl (1 = true)
restecg	Resting electrocardiographic results
thalach	Max heart rate achieved
exang	Exercise-induced angina (1 = yes)
oldpeak	ST depression induced by exercise
slope	Slope of peak ST segment
ca	No. of major vessels colored by fluoroscopy
thal	1 = normal; 2 = fixed defect; 3 = reversible defect
condition	Target (1 = heart disease, 0 = healthy)

⚙️ Tech Stack & Libraries
Library	Purpose
pandas	Data handling and cleaning
matplotlib & seaborn	Visualization and plotting
scikit-learn	ML models, preprocessing, evaluation
StandardScaler	Feature normalization
LogisticRegression, DecisionTreeClassifier	Classification models

🧠 Models Used
1. Decision Tree
Captures complex non-linear patterns.

Works well without feature scaling.

Provides feature importance insights.

🧪 Workflow
Load Dataset

Data Cleaning & EDA

Summary statistics

Correlation heatmap

Target distribution plot

Preprocessing

Drop target column to isolate features

Normalize features with StandardScaler

Train/Test Split

80% training, 20% testing

Model Training

Logistic Regression

Decision Tree

Evaluation Metrics

Accuracy

Confusion Matrix

Classification Report

ROC AUC & Curve

Feature Importance (Decision Tree)

📈 Evaluation Example

Confusion Matrix:
[[24  4]
 [ 3 30]]

Classification Report:
              precision    recall  f1-score   support
           0       0.89      0.86      0.88        28
           1       0.88      0.91      0.89        33

ROC AUC: 0.93
💡 What the Model Learns
Input: A patient’s health metrics.

Output: A prediction — heart disease risk or not.

The model uses patterns from the training data to identify which combinations of features indicate higher or lower risk.

📌 Feature Importance (Decision Tree)
A bar chart is generated showing the most impactful features (e.g., cp, thal, ca, oldpeak, etc.), helping doctors or analysts understand which symptoms/metrics are most influential.
