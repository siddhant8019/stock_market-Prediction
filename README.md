# Stock Price Prediction and Forecasting using LSTM and RNN

## Overview
This project explores the application of Long Short-Term Memory (LSTM) networks and Recurrent Neural Networks (RNN) in predicting and forecasting stock prices. The goal is to analyze past stock market data to predict future price movements. The project focuses on Alphabet Inc. (GOOGL) stock prices, collected from Yahoo Finance, and utilizes LSTM and RNN models to capture complex temporal dependencies for accurate predictions.

## Table of Contents
- [Introduction](#introduction)
- [Literature Survey](#literature-survey)
- [Architecture](#architecture)
- [Experimental Setup](#experimental-setup)
- [Results Analysis](#results-analysis)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction
Businesses require accurate forecasting to make informed decisions and mitigate risks. Time-series data, such as stock prices, provides valuable insights into market trends. This project aims to develop models that can predict stock prices, facilitating better investment strategies and decision-making.

## Literature Survey
Recent studies have demonstrated the effectiveness of LSTM and RNN models in stock price prediction:
- Arnab Mondal utilized historical stock market data and LSTM networks for accurate stock price prediction.
- Lu et al. combined Convolutional Neural Networks (CNN) and LSTM for improved forecasting accuracy.
- Shriram et al. proposed a method using LSTM, RNN, and CNN to predict stock prices with sliding window models.
- Hoseinzadea and Haratizadeha presented CNNpred, a CNN-based stock market prediction model.
- Nabipour et al. discussed the application of deep learning, including LSTM, for stock market prediction.

## Architecture
### Dataset and Related Work
- The dataset contains historical stock price data for Alphabet Inc. (GOOGL) obtained from Yahoo Finance.
- Attributes include opening price, closing price, highest price, lowest price, trading volume, and date for each trading day.

### Methodology
- LSTM neural networks are used to forecast stock values based on past data.
- Data preprocessing involves normalization using Min-Max scaling.
- Model training utilizes a sliding window approach with historical stock prices as input features and the target variable as the stock price at the next time step.

## Experimental Setup
### Training and Test Data Split
- The dataset is divided into training and testing sets.
- The model is trained on historical data and tested on unseen data to evaluate performance.

### Model Training
- The Adam optimizer and Mean Squared Error (MSE) loss function are used for training.

### Validating the Model
- The model is tested with a mean squared error of 7.8014e-04.

## Results Analysis
- The LSTM model demonstrates a strong ability to capture temporal dependencies within the time series data.
- Comparative analysis with non-RNN models like ARIMA and Exponential Smoothing highlights the superiority of LSTM.
- Exploration of LSTM and GRU variants reveals insights into their impact on forecasting accuracy.

## Conclusion
This project demonstrates the effectiveness of LSTM and RNN models in predicting stock prices. By capturing complex temporal dependencies, these models provide valuable insights for investors and businesses. Future work could involve incorporating additional data sources and refining model architectures for further improvements.

## References
- [Arnab Mondal](https://www.analyticsvidhya.com/blog/2021/06/download-financial-dataset-using-yahoo-finance-in-python-a-complete-guide/)
- [Lu et al.](https://doi.org/10.1155/2020/6622927)
- [Shriram et al.](https://www.ijert.org/research/future-stock-price-prediction-using-recurrent-neural-network-lstm-and-machine-learning-IJERTV8IS100270.pdf)
- [Hoseinzadea and Haratizadeha](https://doi.org/10.1016/j.eswa.2019.03.029)
- [Nabipour et al.](https://www.mdpi.com/1099-4300/22/8/840)
