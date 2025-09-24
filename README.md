# S&P 500 Stock Prediction Using Random Forest Classifier

This project uses historical data from the S&P 500 Index to predict whether the closing price of the S&P 500 will go up the following day. A Random Forest Classifier model is employed to make binary predictions (1 for "up" and 0 for "down"). The model is trained using features like the opening, closing, high, low prices, and volume of stock traded. We also utilize technical indicators and rolling averages to enhance model performance.

## Project Overview

1. **Data Collection**:
   - The project fetches historical S&P 500 data using the `yfinance` library.
   - The data is preprocessed to include key features and generate labels based on price movements (up or down).

2. **Model**:
   - A Random Forest Classifier is used to predict the `Target` variable, which is 1 if the closing price will rise the next day and 0 otherwise.
   - A backtesting approach is employed to simulate trading and evaluate the model's performance.

3. **Backtesting**:
   - The model is trained on progressively larger datasets and tested on unseen data.
   - Precision, recall, and other metrics are calculated to assess the performance of the model.

4. **Enhancements**:
   - Technical indicators such as rolling averages, ratios, and trends are incorporated as additional features.
   - The model predicts probabilities and classifies them based on a threshold (`0.6`).

## Features

- **Predictive Model**: Random Forest Classifier used for stock price prediction.
- **Backtesting**: Evaluate the model over time with simulated trading results.
- **Rolling Averages**: Includes multiple time horizons to predict price movements.
- **Probability Classification**: Uses prediction probabilities for more refined decisions.

