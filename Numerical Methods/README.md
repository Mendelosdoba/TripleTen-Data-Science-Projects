
# Numerical Methods Project

## Project Description
This project applies numerical methods and machine learning models to predict used car prices using historical vehicle data.

The goal is to compare several models and evaluate their performance in terms of:
- Prediction accuracy
- Training time
- Inference speed

## Dataset
The dataset contains information about used car listings including:

- Price
- VehicleType
- RegistrationYear
- Gearbox
- Power
- Mileage
- FuelType
- Brand
- Repair status

## Models Used
The following models were trained and compared:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- LightGBM
- CatBoost
- XGBoost

## Evaluation Metrics
Model performance was evaluated using:

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

## Results
Gradient boosting models (LightGBM, CatBoost, and XGBoost) generally produced the best predictions, while simpler models like Linear Regression performed worse on this dataset.

## Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- CatBoost
- XGBoost
