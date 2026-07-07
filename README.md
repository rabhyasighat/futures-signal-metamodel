
# Financial Machine Learning Meta-Model for Futures Trading

*A graduate-level financial machine learning project completed as part of the MSc Risk Management & Financial Engineering at Imperial College London.*

## Overview

This project develops a **financial machine learning metamodel** that predicts whether a systematic trading signal is likely to be profitable before execution.

Instead of generating trading signals directly, the model evaluates the probability that an existing signal should be followed using **triple-barrier event labelling**, advanced feature engineering, and supervised machine learning.

The framework was developed on equity index futures and follows an institutional quantitative research workflow, from feature engineering and model selection to explainability and strategy backtesting.

---

## Objectives

* Predict the profitability of systematic trading signals
* Improve signal selection using machine learning
* Compare multiple classification models
* Interpret model behaviour using explainable AI
* Evaluate performance on an out-of-sample dataset

---

## Universe

The project covers equity index futures:

* S&P 500 (ES)
* Nasdaq-100 (NQ)
* Euro Stoxx 50 (FESX)

Historical OHLCV market data and primary trading signals were used to construct the dataset.

---

## Methodology

### Feature Engineering

* Technical Indicators
* Hidden Markov Models (HMM)
* Gaussian Mixture Models (GMM)
* Rolling PCA
* Market Microstructure Features
* Cross-sectional Features

---

### Event Labelling

Implemented the **Triple-Barrier Method** to generate binary labels indicating whether a trading signal reached its profit target before its stop-loss or time barrier.

---

### Machine Learning Models

The following models were implemented and compared:

* Logistic Regression
* Linear Discriminant Analysis (LDA)
* Quadratic Discriminant Analysis (QDA)
* K-Nearest Neighbours
* Random Forest
* Support Vector Machine
* XGBoost
* LightGBM
* CatBoost
* Multi-layer Perceptron
* Variable Selection Network
* Stacking Ensemble

---

### Model Explainability

* SHAP Values
* Cluster-Level Feature Importance
* Feature Correlation Analysis

---

### Strategy Construction

The predicted probabilities were converted into position-sizing decisions and evaluated using a systematic trading strategy.

Performance was assessed through:

* CAGR
* Sharpe Ratio
* Sortino Ratio
* Annualised Volatility
* Maximum Drawdown
* Turnover
* Average Holding Period

---

## Results

| Metric                 |    Value |
| ---------------------- | -------: |
| Models Evaluated       |       13 |
| Best ROC-AUC           |    0.616 |
| CAGR                   |    12.3% |
| Sharpe Ratio           |     1.42 |
| Annualised Volatility  |    8.46% |
| Maximum Drawdown       |   -2.87% |
| Average Holding Period | 3.4 Days |

---

## Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* LightGBM
* XGBoost
* CatBoost
* Matplotlib
* Plotly

---

## Key Concepts

* Financial Machine Learning
* Triple-Barrier Labelling
* Meta-Labeling
* Supervised Learning
* Explainable AI
* Systematic Trading
* Quantitative Research
* Feature Engineering
* Time-Series Classification
* Portfolio Backtesting

---


