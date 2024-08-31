## Customer Churn Prediction Project

Project Overview
This project aims to predict customer churn in a telecom company using classification models. We developed and compared two models—Logistic Regression and Decision Tree—to identify the key factors influencing customer churn and provide actionable insights for the company to improve customer retention.

Table of Contents
Objective
Data
Methodology
Models Used
Results
Feature Importance
Conclusions
Recommendations
How to Run the Project
Acknowledgments
Objective
The objective of this project is to develop a predictive model for customer churn and identify the primary factors that contribute to churn. By understanding these factors, the company can implement strategies to reduce churn rates and enhance customer retention.

Data
The dataset used in this project is from a telecom company and includes various customer details such as:

Account Length
Total Day Minutes and Charges
Total Evening Minutes and Charges
Total International Minutes, Calls, and Charges
Number of Customer Service Calls
International Plan status
The dataset was preprocessed to handle categorical variables and scaled for model training.

Methodology
Data Preparation:

Encoding categorical features to numerical values.
Feature scaling using StandardScaler.
Splitting the dataset into training (80%) and testing (20%) sets.
Model Development:

Implemented two models: Logistic Regression and Decision Tree.
Hyperparameter tuning using grid search to optimize model performance.
Model Evaluation:

Evaluated models using metrics such as Accuracy, Precision, Recall, F1-Score, and AUC (Area Under the Curve).
Compared model performances using ROC curves to select the best model.
Models Used
Logistic Regression: A linear model used for binary classification.
Decision Tree: A non-linear model that creates decision rules based on feature importance.
Results
Logistic Regression
Training Accuracy: 86.59%
Test Accuracy: 84.85%
AUC (Test): 0.79
Decision Tree
Training Accuracy: 100% (indicative of overfitting)
Test Accuracy: 91%
AUC (Test): 0.85
The Decision Tree model outperformed Logistic Regression in identifying churn, with a higher test accuracy and AUC.

Feature Importance
The top 5 important features influencing customer churn identified by the Decision Tree model are:

Total Day Charge: Strongest predictor of churn.
Total Day Minutes: Highly correlated with churn, similar to total day charge.
Total Evening Charge: Significant in predicting customer churn.
Total International Charge: Key indicator of churn for customers making international calls.
Total International Calls: Number of calls also affects churn likelihood.
Conclusions
The Decision Tree model was selected as the best-performing model for predicting customer churn, offering both superior predictive accuracy and interpretability regarding feature importance.

Recommendations
To reduce churn, the company should focus on:

Monitoring customers with high day and evening charges and offering them tailored retention packages.
Enhancing customer service quality to reduce churn related to frequent service calls.
Reassessing international call plan pricing to ensure competitiveness.