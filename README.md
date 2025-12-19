# Flight-Fare-Prediction
Machine learning regression models to predict flight ticket prices using Python, scikit-learn, and XGBoost.



# ✈️ Flight Price Prediction – Machine Learning Regression Analysis

## 1. Problem Statement

Flight ticket pricing is a non-linear regression problem influenced by multiple categorical, temporal, and numerical features.  
The objective of this project is to build, evaluate, and optimize machine learning regression models to accurately predict flight prices using historical booking data.

---

## 2. Dataset Overview

- **Dataset**: Flight_Fare.xlsx  
- **Target Variable**: Price  
- **Learning Type**: Supervised Learning (Regression)

### Features Description

| Feature | Description |
|------|------------|
| Airline | Airline company |
| Source | Departure city |
| Destination | Arrival city |
| Date_of_Journey | Journey date |
| Duration | Total flight duration |
| Total_Stops | Number of stops |
| Additional_Info | Additional flight details |
| Price | Flight ticket price (Target) |

---

## 3. Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- GridSearchCV

---

## 4. Data Preprocessing & Feature Engineering

- Missing values handled by row elimination
- Date features extracted into day and month
- Flight duration converted into total minutes
- Categorical features encoded using One-Hot Encoding
- Ordinal encoding applied for total stops
- Redundant columns removed post transformation

---

## 5. Train-Test Split

- Dataset split into training and testing sets
- Random state fixed for reproducibility

---

## 6. Models Implemented

### Baseline Models
- Linear Regression
- Ridge Regression
- Lasso Regression
- ElasticNet Regression

### Advanced Models
- Random Forest Regressor
- XGBoost Regressor

---

## 7. Hyperparameter Tuning

GridSearchCV was applied to optimize:

### Random Forest
- n_estimators
- max_depth
- min_samples_split

### XGBoost
- learning_rate
- max_depth
- n_estimators

---

## 8. Model Evaluation

- Evaluation Metric: Mean Squared Error (MSE)
- Ensemble models significantly outperformed linear models
- Hyperparameter tuning improved generalization

---

## 9. Key Findings

- Flight price prediction is highly non-linear
- Duration, total stops, and airline are key drivers
- Tree-based ensemble models performed best
- Tuned XGBoost achieved lowest prediction error

---

## 10. Conclusion

This project demonstrates a complete machine learning regression pipeline including preprocessing, feature engineering, model training, tuning, and evaluation.  
The final optimized model is suitable for deployment in real-world pricing applications.

---

## 11. Repository Structure

Flight-Price-Prediction/
│
├── FlightPricePrediction.ipynb
├── Flight_Fare.xlsx
├── README.md

---

## 12. Future Enhancements

- K-Fold Cross Validation
- Feature importance visualization
- Model deployment using Flask or FastAPI
- Streamlit-based web application

---

## 13. Author

Sathish V  
M.Tech – Signal Processing (NIT Calicut)  
Aspiring Data Scientist

---
