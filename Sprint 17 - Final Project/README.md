📊 Customer Churn Prediction
📌 Project Overview

This project focuses on predicting customer churn using machine learning techniques. By identifying customers at risk of leaving, businesses can take proactive steps to improve retention and reduce revenue loss.

📂 Dataset

The dataset consists of multiple tables that were merged into a single dataframe:

contract.csv – Customer contract details
personal.csv – Demographic information
internet.csv – Internet services
phone.csv – Phone services
⚙️ Data Preprocessing

The following preprocessing steps were performed:

Merged datasets on customerID
Handled missing values and duplicates
Encoded categorical variables using one-hot encoding
Created target variable (churn)
Engineered new features (e.g., tenure)
Split data into training and testing sets
🤖 Models Used

The following models were trained and evaluated:

Logistic Regression
Random Forest
LightGBM

LightGBM achieved the best performance.

📈 Results
Accuracy: 0.91
F1 Score: 0.84
ROC-AUC: 0.95

The model demonstrates strong performance in identifying customers likely to churn.

📊 Key Insights
Customers with shorter tenure are more likely to churn
Higher monthly charges are associated with increased churn
Customers lacking support-related services show higher churn rates
🚀 Conclusion

This model provides a reliable approach for predicting churn and can be used to guide targeted retention strategies.
