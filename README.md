# 📈 Stock Price Prediction with Linear Regression

A Python-based project to predict and visualize stock closing prices using a linear regression model trained on historical stock data.

---

## 🛠️ Overview

This script allows users to input a stock ticker or company name (mapping to a local CSV file), loads the historical stock data, preprocesses it, and trains a linear regression model to predict future closing prices based on features like Open, High, Low, and Volume.

---

## ⚙️ Features

- ✅ Reads historical stock `.csv` files (expects columns: Date, Open, High, Low, Close, Volume, Adj Close)
- 🔄 Parses and converts date-based features
- 📉 Drops irrelevant columns and handles missing values
- 🧠 Trains a **Linear Regression** model on OHLC+Volume data
- 📊 Outputs predicted vs. actual closing prices
- 📈 Displays time-series plots for both actual and predicted values
- 🧮 Prints model coefficients, intercept, and R² score for performance assessment

---

## 🔧 Prerequisites

Tested on Python 3.x. Required libraries—install via:

```bash
pip install pandas numpy scikit-learn matplotlib
1. Ensure your dataset CSV is named <company>.csv and placed in the path:
C:\Users\<YourUser>\OneDrive\Desktop\SEM4\CSV\

2. Run the script:

python stock_predictor.py

3.When prompted, enter the company filename (without .csv), e.g.:
Enter a string: TCS

4.Workflow:

Model trains on historical data

Prints regression coefficients and intercept

Displays first few predicted & actual values

5. File structure
stock_predictor.py
CSV/
  └── <COMPANY>.csv
README.md

