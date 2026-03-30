# Energy Market Forecasting Project

## Overview
This project was developed as a team effort by three contributors and focuses on time series forecasting applied to the energy sector. The main objective was to build a complete analytical workflow — from data preparation and transformation to model building, evaluation, and forecasting.

The project combines econometric modeling techniques with data aggregation methods to better capture complex dynamics present in financial and energy-related time series.

## What We Built
- End-to-end forecasting pipeline (data → transformation → modeling → evaluation)
- Multiple synthetic indices based on:
  - Equal Weights (EW)
  - Principal Component Analysis (PCA)
  - Entropy-based weights (EWM)
- Implementation and comparison of several forecasting models:
  - ARIMA
  - SARIMA
  - Holt-Winters (Exponential Smoothing)
- Two forecasting approaches:
  - Direct forecasting of aggregated indices
  - Component-based forecasting (each variable modeled separately)

## Methodology
The project compares two approaches to forecasting:

**1. Direct Forecasting**
Aggregated indices are forecasted directly using time series models. This approach is simpler and provides a strong baseline.

**2. Component-Based Forecasting**
Each variable is modeled individually, and the final forecast is obtained through aggregation. This allows capturing different dynamics across variables and improves flexibility.

Models were evaluated using standard metrics such as RMSE, MAE, MAPE, and RMSPE on out-of-sample data.

## Key Insights
- Different variables require different models — no single model performs best across all series  
- Component-based forecasting provides more stable and interpretable results  
- PCA-based indices effectively capture common trends in the data  

## Technologies
- Python (pandas, numpy, statsmodels)
- scikit-learn (PCA, scaling)
- matplotlib
- Git / GitHub

## Authors
Tomasz Kotliński, Piotr Łukowski
