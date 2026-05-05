# Customer Churn Prediction

## Project Overview

This project predicts customer churn using machine learning. The goal is to identify customers who are likely to leave so that a business can take proactive steps to improve retention.

The project includes data preprocessing, exploratory data analysis, model training, hyperparameter tuning, evaluation, and feature importance analysis.

## Dataset

The data comes from four separate tables:

- `contract.csv` — contract and billing information
- `personal.csv` — customer demographic information
- `internet.csv` — internet service details
- `phone.csv` — phone service details

The tables were merged into one dataset using `customerID`.

## Preprocessing Steps

The main preprocessing steps included:

- Checked for missing values and duplicates
- Merged all datasets into one dataframe
- Filled missing service values with `"No"`
- Converted `TotalCharges` to numeric
- Created the target variable: `churn`
- Created a tenure feature using `BeginDate`
- Dropped unnecessary columns such as `customerID`, `EndDate`, and `BeginDate`
- Encoded categorical variables using one-hot encoding
- Scaled numerical features for Logistic Regression
- Split the data into training, validation, and test sets

## Exploratory Data Analysis

The EDA showed several important churn patterns:

- Customers with month-to-month contracts are more likely to churn
- Customers using electronic check payments have higher churn
- Customers without online security or tech support are more likely to churn
- Higher monthly charges are associated with increased churn
- Shorter-tenure customers are at higher risk of leaving

## Models Used

Several classification models were trained and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- LightGBM

Each model was tuned using a validation set and evaluated using accuracy, F1 score, and ROC-AUC.

## Best Model

The best-performing model was **LightGBM**.

### Final Test Results

| Metric | Score |
|---|---:|
| Accuracy | 0.9049 |
| F1 Score | 0.8139 |
| ROC-AUC | 0.9429 |

LightGBM performed best because it captured non-linear relationships between customer behavior, contract details, service features, and churn risk.

## Feature Importance

The most important features included:

- MonthlyCharges
- TotalCharges
- tenure_days
- Contract type
- Payment method
- OnlineSecurity
- TechSupport

These results suggest that pricing, customer tenure, contract structure, and support-related services are major factors in customer churn.

## Business Recommendations

Based on the model results, the business should focus on:

- Improving onboarding for new customers
- Offering incentives to high monthly charge customers
- Encouraging longer-term contracts
- Promoting support services such as tech support and online security
- Targeting high-risk customers before they churn

## Conclusion

This project successfully built a churn prediction model with strong performance. The tuned LightGBM model achieved high ROC-AUC and F1 scores, showing that it can reliably identify customers at risk of leaving. The feature importance analysis also provides useful business insights that can support customer retention strategies.
