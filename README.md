# 📊 Machine Learning Pipeline for Predictive Modeling - Crop Yield Prediction

## 🚀 Overview
This project implements an end-to-end machine learning pipeline, including data preprocessing, feature engineering, model training, and evaluation.

The objective is to build robust predictive models and compare multiple algorithms to identify the best-performing approach.

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
- Perform initial inspection and cleaning

### 2. Data Preprocessing
- Handle missing values
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
