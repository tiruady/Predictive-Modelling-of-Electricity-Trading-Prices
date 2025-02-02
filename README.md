# Energy Trading Price Prediction

A multivariate time-series analysis project for predicting energy trading prices based on weather and stock market features using LSTM and ARIMA models.

## Overview

This project analyzes and predicts daily electricity trading prices for the PJM West Hub using multiple data sources including weather parameters, stock market data, and historical energy prices. The implementation compares traditional ARIMA models with LSTM networks for multivariate time-series prediction.

## Data Sources

- Wholesale electricity data from PJM West Hub (EIA)
- State Energy Data System (SEDS) for solar energy production estimates
- S&P index daily price data from Yahoo Finance
- PSM v3.0 weather data from National Solar Radiation Database

## Features

- Daily energy trading prices
- Weather parameters (DNI, DHI, temperature, pressure, wind speed)
- S&P index prices and trading volumes
- Solar energy production estimates
- Trading volume and number of trades

## Implementation

The project includes:
- Data preprocessing and feature engineering
- Weight calculation for different states based on solar production
- ARIMA model implementation for univariate analysis
- LSTM model with 30-day lookback for multivariate prediction
- Comparative analysis of both approaches

## Results

The LSTM model significantly outperformed the traditional ARIMA approach:
- LSTM Test RMSE: 24.06
- ARIMA RMSE: 7918.06

## Requirements

- Python 3.6
- TensorFlow 1.14 with Keras
- Pandas, NumPy, Scikit-learn
- Statsmodels
- Matplotlib, Seaborn

## Usage

1. Prepare datasets from the mentioned sources
2. Run data preprocessing scripts
3. Train ARIMA and LSTM models
4. Compare results using provided metrics

## Contributors

- Aditya Bahukhandi
- Manav Vallecha
- Neelaksh Trehan
- Nikhil Goyal

Project completed under the guidance of Prof. O.P. Vyas at IIIT Allahabad.
