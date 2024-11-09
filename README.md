# Multimodal Bitcoin Forecasting

## 👋 Introduction

This repository presents a multimodal approach for Bitcoin price forecasting, utilizing various machine learning models to predict future prices of Bitcoin based on historical data. The models used in this project include traditional deep learning architectures, such as Dense Neural Networks, LSTMs, and 1D Convolutional Neural Networks (CNNs), as well as more advanced methods like N-BEATS and ensemble models.

## 🥷 Models

### 1. Naive Model
This is our baseline model, serving as a reference point for performance comparison.

### 2. Dense Model (model_1_dense_w7_h1)
A simple dense model that learns patterns in the input data to make predictions.

### 3. Dense Model with 30 weights (model_2_dense_w30_h1)
A more complex dense model designed to capture intricate relationships in the data.

### 4. Dense Model with 30 weights and 7 hidden layers (model_3_dense_w30_h7)
A deeper model with more complexity and increased capacity for learning from the data.

### 5. 1D Convolutional Neural Network (model_4_CONV1D)
A CNN-based model that can detect patterns and features within the data sequence.

### 6. LSTM Model (model_5_LSTM)
LSTM captures long-range dependencies and is ideal for sequential time series data.

### 7. Multivariate Model (model_6_multivariate)
A model using multiple variables as inputs to forecast Bitcoin prices.

### 8. N-BEATS Model (model_8_NBEATs)
A powerful model for time series forecasting that captures trends and seasonalities.

### 9. Ensemble Model (model_9_ensemble)
Combines the predictions from multiple models for improved accuracy and performance.

## 💻 Results

We evaluate each model's performance using the following metrics: **MAE (Mean Absolute Error)**, **MSE (Mean Squared Error)**, **RMSE (Root Mean Squared Error)**, **MAPE (Mean Absolute Percentage Error)**, and **MASE (Mean Absolute Scaled Error)**.

| Model                        | MAE        | MSE        | RMSE       | MAPE      | MASE        |
|------------------------------|------------|------------|------------|-----------|-------------|
| Naive Model                  | 567.98     | 1,147,547  | 1071.24    | 2.52      | 0.99957     |
| model_1_dense_w7_h1           | 568.55     | 1,172,588  | 1082.86    | 2.55      | 0.99879     |
| model_2_dense_w30_h1          | 608.85     | 1,284,315  | 1133.28    | 2.77      | 1.06427     |
| model_3_dense_w30_h7          | 1228.52    | 5,328,784  | 2308.42    | 5.48      | 2.1861      |
| model_4_CONV1D                | 569.03     | 1,169,841  | 1081.59    | 2.55      | 0.99963     |
| model_5_LSTM                  | 593.53     | 1,264,156  | 1124.35    | 2.67      | 1.04267     |
| model_6_multivariate          | 568.45     | 1,166,160  | 1079.89    | 2.55      | 0.99861     |
| model_8_NBEATs                | 1702.24    | 5,988,355  | 2447.11    | 8.50      | 2.99036     |
| model_9_ensemble              | 567.27     | 1,150,359  | 1072.55    | 2.58      | 0.99653     |
