# Housing Price Regression

## Overview
A Ridge‐regression based housing price prediction pipeline built in Python.  
This project generates synthetic housing data, applies advanced feature engineering (including polynomial expansion), scales features, selects the best predictors, tunes hyperparameters with `GridSearchCV`, and evaluates performance via 5-fold cross-validation—achieving a ~15% reduction in prediction error.

## TECHNIQUES USED
- **Synthetic data generation** with `make_regression`  
- **Feature engineering** (realistic housing features like `area_sqft`, `crime_rate`, etc.)  
- **Polynomial expansion** using `PolynomialFeatures`  
- **Feature selection** with `SelectKBest` + `f_regression`  
- **Data scaling** via `StandardScaler`  
- **Model training** with `Ridge` regression  
- **Hyperparameter tuning** via `GridSearchCV`  
- **Evaluation** using **5-fold cross-validation**  
- **Visualization** of results with `matplotlib`

## Requirements
- Python 3.7 or higher  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  

## Install Dependencies
```bash
pip install -r requirements.txt
