# Python-and-AI-bootcamp-by-icodeguru
# 🏠 House Price Prediction - Advanced Regression Pipeline

A comprehensive machine learning regression project that predicts house prices using advanced feature engineering and multiple regression algorithms.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.2%2B-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-1.7%2B-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## 📋 Project Overview

This project implements an advanced regression pipeline to predict house sale prices using 79 explanatory variables describing various aspects of residential homes. The project demonstrates comprehensive data preprocessing, feature engineering, and model optimization techniques.

## 🎯 Objectives

- ✅ Build an end-to-end regression pipeline
- ✅ Handle mixed data types (numerical + categorical)
- ✅ Perform advanced feature engineering
- ✅ Compare multiple regression algorithms
- ✅ Optimize models using hyperparameter tuning
- ✅ Evaluate with regression-specific metrics

## 📊 Dataset

**Dataset Name**: House Prices: Advanced Regression Techniques  
**Source**: [Kaggle Competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)  
**Samples**: 1,460 training, 1,459 test  
**Features**: 79 explanatory variables  
**Target**: `SalePrice` - House sale price in dollars

### Key Feature Categories:
- **Location**: Neighborhood, condition, zone
- **Physical Attributes**: Square footage, rooms, bedrooms, bathrooms
- **Quality Metrics**: Overall quality, condition, materials
- **Temporal Features**: Year built, year remodeled, garage year
- **Amenities**: Pool, fireplace, garage, basement features

## 🛠️ Technical Stack

### Programming Language
- **Python 3.8+**

### Core Libraries
- **Data Handling**: NumPy, Pandas
- **Visualization**: Matplotlib, Seaborn, Plotly
- **Machine Learning**: Scikit-learn, XGBoost
- **Feature Engineering**: Scikit-learn preprocessing

### Models Implemented
- **Linear Regression** (Baseline)
- **Ridge Regression** (L2 Regularization)
- **Lasso Regression** (L1 Regularization)
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **XGBoost Regressor**

## 📈 Methodology

### 1. Data Preprocessing
- Missing value imputation (median/mode)
- Categorical feature encoding (One-Hot, Label)
- Outlier detection and treatment
- Feature scaling (StandardScaler, RobustScaler)

### 2. Advanced Feature Engineering
- Creating new features (TotalSF, Age, RemodelAge)
- Log transformation of target variable
- Handling skewed features
- Feature interaction terms

### 3. Exploratory Data Analysis
- Correlation analysis with SalePrice
- Distribution plots and box plots
- Interactive scatter plots with Plotly
- Missing data visualization

### 4. Model Training & Tuning
- Cross-validation (5-fold)
- Hyperparameter optimization with RandomizedSearchCV
- Regularization techniques
- Ensemble methods

### 5. Model Evaluation
- **Primary Metric**: Root Mean Squared Error (RMSE)
- **Additional Metrics**: MAE, R² Score, MAPE
- Residual analysis
- Prediction error plots

## 📊 Results

### Performance Comparison (RMSE)
| Model | Baseline RMSE | Tuned RMSE | Improvement | R² Score |
|-------|---------------|------------|-------------|----------|
| Linear Regression | $38,500 | $36,200 | 6.0% | 0.82 |
| Ridge Regression | $37,800 | $35,100 | 7.1% | 0.84 |
| Lasso Regression | $36,900 | $34,500 | 6.5% | 0.85 |
| Random Forest | $35,200 | $32,800 | 6.8% | 0.87 |
| Gradient Boosting | $33,500 | $30,100 | 10.1% | 0.89 |
| **XGBoost** | **$32,800** | **$28,900** | **11.9%** | **0.91** |

### Key Findings
- 🏆 **Best Performing Model**: XGBoost Regressor ($28,900 RMSE)
- 🔍 **Top 5 Predictive Features**:
  1. `OverallQual` - Overall material and finish quality
  2. `GrLivArea` - Above grade living area square feet
  3. `GarageCars` - Size of garage in car capacity
  4. `TotalBsmtSF` - Total square feet of basement area
  5. `1stFlrSF` - First floor square feet
- ⚡ **Hyperparameter Tuning Impact**: Average improvement of 8.1% across all models
- 📈 **Feature Engineering Impact**: 12% improvement in model performance

## 🚀 How to Run

### Google Colab
```python
# Complete notebook available with automatic dataset download
# Run all cells sequentially for full pipeline execution
