# Bitcoin Price Predictor

A polished data science project for forecasting Bitcoin prices with machine learning. This repository contains a full notebook-driven workflow that collects historical BTC data, explores price behavior, evaluates multiple regression models, and compares their performance with metrics such as RMSE and R².

## 🚀 Project Overview

The main notebook, [Bitcoin_price_predictor.ipynb](Bitcoin_price_predictor.ipynb), explores how different supervised learning approaches perform on BTC-USD historical data. The workflow includes:

- Data retrieval from Yahoo Finance
- Exploratory data analysis and visualization
- Baseline model benchmarking
- Preprocessing pipelines with scaling and polynomial transformations
- Hyperparameter tuning with GridSearchCV
- Model performance tracking and saving

## 🧠 What’s Inside

- [Bitcoin_price_predictor.ipynb](Bitcoin_price_predictor.ipynb): the core analysis notebook
- [figures](figures): visualization outputs such as price trends and model ranking plots
- [models/perfs](models/perfs): CSV files with recorded model performance metrics
- [models/saved](models/saved): saved model artifacts

## 📊 Methodology

The project evaluates a wide range of regression models, including:

- Linear Regression
- Lasso Regression
- Ridge Regression
- Support Vector Regression (SVR)
- K-Nearest Neighbors Regressor
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

It also compares several preprocessing strategies such as:

- StandardScaler
- PolynomialFeatures
- Pipeline-based model workflows

## 📈 Results Snapshot

The notebook reports strong performance for regularized linear models, especially Ridge and Lasso, which achieved very high R² values and low RMSE in the tested setup. The analysis also shows that some more complex models were less competitive in this configuration.

## 🛠️ Quick Start

1. Install the required libraries:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn yfinance xgboost jupyter
   ```

2. Launch the notebook:

   ```bash
   jupyter notebook
   ```

3. Open [Bitcoin_price_predictor.ipynb](Bitcoin_price_predictor.ipynb) and run the cells in order.

## 📁 Repository Structure

```text
.
├── Bitcoin_price_predictor.ipynb
├── figures/
├── models/
│   ├── perfs/
│   └── saved/
└── README.md
```

## 💡 Future Improvements

Possible next steps include:

- Adding technical indicators such as RSI, moving averages, and volatility features
- Incorporating lagged price features for time-series forecasting
- Comparing against deep learning approaches
- Building a simple deployment pipeline for live predictions

## ✨ Summary

This project is a hands-on example of building a practical machine learning workflow for financial forecasting, from raw market data to model evaluation and interpretation.

