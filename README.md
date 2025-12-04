#  **Multi-Stock Price Forecasting Using Advanced Feature Engineering + RF/XGBoost/LSTM Ensemble**

This project builds a highly accurate **multi-model ensemble** for predicting strong directional movements in stock prices.  
It uses **79%+ accuracy methodology** with advanced feature engineering, a weighted ensemble of **Random Forest, XGBoost, and LSTM**, and automatic saving of trained models.

---

##  **Project Overview**

This ML pipeline performs:

- ✔ Loading stock data from Google Drive  
- ✔ Generating **30 advanced technical features**  
- ✔ Creating **strong signal classification targets**  
- ✔ Training an ensemble of:
  - **Random Forest**
  - **XGBoost**
  - **LSTM Deep Learning Model**
- ✔ **Dynamic ensemble weighting** based on validation accuracy  
- ✔ Model saving for each stock  
- ✔ Complete evaluation:
  - Accuracy  
  - F1-score  
  - Precision  
  - Recall  
  - Confusion Matrix  
  - AUC-ROC  

---

##  **Dataset Source**

The project expects CSV files from **Yahoo Finance**, stored like:
Each CSV must contain:

- Date  
- Open  
- High  
- Low  
- Close  
- Volume
##  **Feature Engineering (30+ Features)**

The notebook generates an extensive feature set including:

### ** Price-based features**
- Multi-timeframe returns: 3d, 5d, 10d, 20d  
- Moving averages: 3, 5, 7, 10, 15, 20, 30, 50  
- MA ratios and normalized distances  

### ** Volatility features**
- 5-day, 20-day, 50-day volatility  
- Volatility ratios & volatility regime classifier  

### ** Market structure**
- Higher High / Lower Low  
- Inside bar detection  

### ** Trend/Momentum indicators**
- MACD (12/26), Signal Line, Histogram  
- Multi-period RSI: 7, 14, 21, 30  

### ** Bollinger Bands**
- Upper/Lower bands, Band width, Band position  

### ** Volume analytics**
- Volume MA (10, 30)  
- Volume ratio  
- Volume spike flag  
- Price-volume trend indicator
### ** Models**
Random Forest (scikit-learn)
XGBoost (XGBClassifier)
LSTM (Keras / TensorFlow) configured for binary classification
Ensemble: Weighted average of model probabilities with weights proportional to validation accuracy

ensemble = RF_weight * RF
          + XGB_weight * XGB
          + LSTM_weight * LSTM
### ** Author**
Kiran Behera
