﻿
# machinelearning_1
# 📈 Reliance Stock Price Prediction using Regression Models

This project focuses on predicting the closing stock price of **Reliance** using different regression techniques:

- ✅ Simple Linear Regression
- ✅ Multiple Linear Regression
- ✅ Polynomial Regression (degrees 2 to 4)

## 🧠 Objective

To explore and compare the performance of different regression models on real stock data of Reliance, and determine which model offers the best predictive capability.

## 📊 Dataset

- Source: [Kaggle / Yahoo Finance / CSV file]
- Columns include: `Date`, `Open`, `High`, `Low`, `Last`, `Close`, `VWAP`, `Volume`, `Turnover`, etc.

## 🧹 Data Preprocessing

- Converted `Date` to datetime format
- Handled missing values using `SimpleImputer`
- Scaled features using `StandardScaler`
- Chose most correlated features for modeling (`VWAP`, `Open`, `High`, etc.)

## 📌 Models Used

1. **Simple Linear Regression**
   - Feature: `VWAP`
   - Target: `Close`
   - R² Score: ~0.99917

2. **Multiple Linear Regression**
   - Features: `VWAP`, `Open`, `High`, `Low`
   - Target: `Close`
   - R² Score: ~0.99966

3. **Polynomial Regression**
   - Degree: 2, 3, and 4
   - Feature: `VWAP` only
   - Degree 2 R² Score: 0.99965

## 📉 Evaluation Metrics

- R² Score
- Mean Squared Error (MSE)
- Train-Test Split (80-20%)

## 📈 Visualizations

- Correlation Heatmap
- Regression Line vs Actual Values
- Predicted vs Actual plots

## 🛠️ Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
