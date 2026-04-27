# 📊 Crop Yield Prediction – Machine Learning Pipeline

## 🚀 Overview
This project was developed as part of the Kaggle competition:  
**Crop Yield Prediction Challenge**

🔗 https://www.kaggle.com/competitions/crop-yield-prediction-challenge/overview

The objective of the competition is to predict crop yields based on environmental, geographical, and agricultural features.

This repository implements an end-to-end machine learning pipeline, including:
- Data preprocessing  
- Feature engineering  
- Model training across multiple algorithms  
- Model evaluation and comparison  

---

## 📁 Project Structure

```text
├── algo_clean.ipynb # Main notebook
├── crop_yield_train.xls # Training data
├── crop_yield_test.xls # Test data
└── README.md # Documentation
```

---

## ⚙️ Workflow

### 1. Data Loading
- Load dataset into a Pandas DataFrame

### 2. Data Preprocessing
- Encode categorical variables using `OneHotEncoder`
- Scale numerical features using `StandardScaler`
- Use `ColumnTransformer` to manage mixed data types

### 3. Feature Engineering
- Create derived features to improve model performance
- Prepare final dataset for training

### 4. Model Training
The following models are implemented and compared:

- **Linear Models**
  - Ridge Regression
  - Lasso Regression
  - ElasticNet

- **Tree-Based Models**
  - Random Forest

- **Boosting Models**
  - XGBoost
  - LightGBM
  - CatBoost

### 5. Model Evaluation
- Cross-validation using K-Fold
- Metrics:
  - RMSE / MSE
- Compare performance across models

---

## 🧠 Models Summary

| Model          | Type        | Key Strength              |
|----------------|------------|--------------------------|
| Ridge / Lasso  | Linear     | Regularization           |
| ElasticNet     | Linear     | L1 + L2 combination      |
| Random Forest  | Ensemble   | Captures non-linearity   |
| XGBoost        | Boosting   | High performance         |
| LightGBM       | Boosting   | Fast & scalable          |
| CatBoost       | Boosting   | Handles categorical data |

---

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- LightGBM
- CatBoost
