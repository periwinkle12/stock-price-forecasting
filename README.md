 Advanced Multi-Stock Forecasting Using RF, XGBoost, LSTM & Weighted Ensemble

This project implements a high-accuracy stock forecasting system using a combination of:

Advanced Feature Engineering (70+ features)

Random Forest Classifier

XGBoost Classifier

LSTM Neural Network

Weighted Ensemble Model

The system loads multiple stock CSV files from Google Drive or local storage, extracts predictive features, trains individual models, computes ensemble weights based on validation accuracy, and evaluates performance with detailed metrics and visualizations.

 Key Features
✔ Multi-stock training (AAPL, GOOGL, MSFT, TSLA, NVDA, META, NFLX, etc.)
✔ 70+ engineered features including:

Multi-period returns

Moving averages & MA ratios

Volatility features (5d, 20d, 50d)

Price position indicators

MACD, RSI (multiple periods)

Bollinger bands

Volume features (ratios, spikes)

Market structure signals (Inside Bar, Higher High, Lower Low)

✔ Three powerful ML models:

Random Forest

XGBoost

LSTM (2-layer)

✔ Weighted ensemble:

Weights are dynamically computed based on validation accuracy of each model.

✔ Automatic saving of:

RF model

XGBoost model

LSTM model

Scaler

Ensemble weights
