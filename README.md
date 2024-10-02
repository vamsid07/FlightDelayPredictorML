# Flight Delay Predictor

## Author
Vamsidhar Venkataraman

## Abstract
This project implements a two-stage machine learning model to predict flight delays for 15 major airports in the United States. The model combines classification and regression techniques to provide comprehensive predictions.

### Key Features:
- Binary classifier to determine if a flight will be delayed by 15 minutes or more
- Regression model to predict the exact delay duration for flights classified as delayed
- Utilizes extensive flight and weather data
- Achieves high accuracy: 0.92 for classification and 0.94 for regression

## Dataset
The dataset includes flight and weather data from 15 major U.S. airports for 2016-2017. It contains:
- Flight-related columns: FlightDate, DepTime, ArrTime, ArrDel15, etc.
- Weather-related columns: WindSpeed, Visibility, WeatherCode, etc.

Airports covered: ATL, CLT, DEN, DFW, EWR, IAH, JFK, LAS, LAX, MCO, MIA, ORD, PHX, SEA, SFO

## Methodology

### 1. Classification Stage
- Uses XGBoost algorithm
- Predicts if a flight will be delayed by 15+ minutes
- Addresses class imbalance using SMOTE
- Achieves 0.92 accuracy

### 2. Regression Stage
- Uses Random Forest algorithm
- Predicts exact delay duration for flights classified as delayed
- Achieves R-squared value of 0.9459

## Model Performance

### Classification Metrics (after SMOTE):
- Accuracy: 0.92
- Precision (Class 1): 0.89
- Recall (Class 1): 0.70
- F1-score (Class 1): 0.78

### Regression Metrics:
- MAE: 12.9485
- MSE: 328.5659
- RMSE: 18.1264
- R-squared: 0.9459

## Conclusion
The two-stage model demonstrates high accuracy in predicting flight delays. The Random Forest regressor performs exceptionally well, achieving an R-squared value of 0.9459. This model can be valuable for airlines and airports in resource allocation, schedule planning, and improving passenger experience.

## References
1. "SMOTE: Synthetic Minority Over-sampling Technique", Available online: https://arxiv.org/pdf/1106.1813
