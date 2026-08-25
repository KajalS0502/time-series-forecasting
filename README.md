# Time Series Forecasting using LSTM

## Overview

This project implements time series forecasting of monthly airline passenger data using a Long Short-Term Memory (LSTM) neural network.

## Dataset

The dataset contains monthly airline passenger totals from January 1949 to December 1960.

- Number of records: 144
- Frequency: Monthly
- Target variable: Passengers
- Lookback window: 12 months

## Methodology

The forecasting pipeline consists of:

1. Loading the airline passenger dataset
2. Scaling the data using MinMaxScaler
3. Creating 12-month sliding window sequences
4. Splitting the data into training and testing sets
5. Reshaping the data for LSTM input
6. Building and training an LSTM model
7. Generating predictions
8. Inverse transforming predictions
9. Evaluating the model using RMSE

## Model Architecture

- LSTM layer: 50 units
- LSTM layer: 50 units
- Dense output layer: 1 unit
- Optimizer: Adam
- Loss function: Mean Squared Error
- Epochs: 100
- Batch size: 8

## Evaluation

The model is evaluated using Root Mean Squared Error (RMSE).

## Project Structure

```text
time-series-forecasting/
│
├── data/
│   └── airline-passengers.csv
│
├── notebooks/
│   └── 01_time_series_lstm.ipynb
│
├── models/
│   └── lstm_forecast.h5
│
├── README.md
│
└── .gitignore
