# 📈 Stock Return Prediction and Feature Selection with Machine Learning

This project investigates stock return prediction using a suite of machine learning models. It compares traditional linear regression techniques with modern nonlinear methods and explores optimal feature selection to improve predictive performance.

## Overview

Stock return forecasting is a core challenge in financial analytics. Traditional models often fail to capture complex patterns in financial data. This project integrates:

- **Linear Models**: OLS, ElasticNet, Generalized Linear Models (GLM)
- **Tree-based Models**: Random Forest, Gradient Boosting Trees, LightGBM
- **Neural Networks**: Multi-layer ReLU networks with regularization
- **Feature Selection**: LASSO, PCA, PLS
- **Dataset**: CRSP, Compustat, I/B/E/S (1980–2014)

## Models and Techniques

| Model Type       | Algorithms Used                               |
|------------------|-----------------------------------------------|
| Linear Models     | OLS, ElasticNet, GLM, PCR, PLS                |
| Tree-Based Models | Random Forest, Gradient Boosting, LightGBM   |
| Neural Networks   | Deep Feedforward Networks with ReLU          |

Each model is trained and validated using a time-series rolling window strategy to simulate realistic forecasting scenarios and avoid data leakage.

## Feature Importance

Top predictive features across models include:
- **Momentum indicators** (MOM1M, MOM12M)
- **Volatility measures** (RETVOL, IDIOVOL)
- **Liquidity indicators** (DOLVOL, TURN)

## Data

- **Sources**: CRSP (returns), Compustat (financials), I/B/E/S (analyst forecasts)
- **Period**: 1980–2014
- **Observations**: ~1.9 million firm-month records
- **Preprocessing**: Standardization, missing value imputation, microcap exclusion

## Evaluation Metrics

- R² scores (in-sample and out-of-sample)
- Feature importance rankings
- Visual comparison across models

## Key Findings

- Nonlinear models (especially Random Forest and LightGBM) significantly outperform linear methods in predictive accuracy.
- ElasticNet shows limited performance due to over-regularization.
- Combining machine learning with economic theory improves both interpretability and performance.

## Future Work

- Extend to real-time high-frequency data
- Improve explainability using SHAP or LIME
- Incorporate macroeconomic regime-switching indicators

---


