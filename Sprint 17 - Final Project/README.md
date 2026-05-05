
📊 Customer Churn Prediction
📌 Project Overview

This project aims to predict customer churn using machine learning techniques. By identifying customers likely to leave, businesses can take proactive steps to improve retention and reduce revenue loss.

📂 Dataset

The data consists of multiple tables:

contract.csv – customer contract details
personal.csv – demographic information
internet.csv – internet services
phone.csv – phone services

These datasets were merged into a single dataframe for analysis.

⚙️ Data Preprocessing

Key preprocessing steps included:

Handling missing values and duplicates
Merging multiple datasets on customerID
Encoding categorical variables (one-hot encoding)
Creating target variable (churn)
Feature engineering (e.g., tenure calculation)
Train/test split
🤖 Models Used

Several models were tested and compared:

Logistic Regression
Random Forest
LightGBM

LightGBM performed best overall.

📈 Results
Accuracy: 0.91
F1 Score: 0.84
ROC-AUC: 0.95

The model successfully identifies churn patterns with high reliability.

📊 Key Insights
Customers with shorter tenure are more likely to churn
Higher monthly charges correlate with increased churn
Certain service combinations (e.g., lack of support features) increase churn risk
