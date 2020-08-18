# Recruit-Restaurant-Visitor-Forecasting

Overview: https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting

The main objective of this project is to make automated future customer prediction by utilizing the restaurant data from Recruit Holdings. The analysis of available reservation and visitation data focuses on developing a reliable machine learning algorithm to help restaurants plan more efficiently and allow them to focus on creating an enjoyable dining experience for their customers.

Two different approaches for building the models and predicting the value are followed: restaurant-wise and global modeling. Mostly, restaurant-wise models are applied as the algorithms gave better results when applied to one time series at a time. The test data included 821 restaurants. Therefore, 821 models were built for each algorithm applying restaurant-wise approach. The following machine learning models were trained for the dataset: Linear Regression Model, Auto Regressive (AR) Model, Moving Average (MA) Model, Auto Regressive Moving Average (ARMA) Model, Auto Regressive Integrated Moving Average (ARIMA) Model, Seasonal ARIMA (SARIMA) Model, LightGBM, and Recurrent Neural Network (RNN) or Long Short Term Memory (LSTM) Model.

Root Mean Squared Logarithmic Error (RMSLE) is used as the performance metric for evaluating the performance of the algorithms on the dataset. A lower value of RMSLE corresponds to a better model. The performance metric of the above algorithms as measured by the Kaggle Competition can be compared as follows:

| Algorithm | Private score | Public score |
| ------------- |:-------------:| -----:|
| Regression Model | 0.60694 | 0.56537 |
| AR Model | 0.62782 | 0.60151 |
| MA Model | 0.63095 | 0.60998 |
| ARMA Model | 0.60216 | 0.57688 |
| ARIMA Model | 0.60322 | 0.57676 |
| SARIMA Model | 0.56575 | 0.52322 |
| LightGBM Model | 0.71750 | 0.69724 |
| RNN/LSTM Model | 0.69129 | 0.69710 |

Based on the experimental results, Seasonal ARIMA model gives the lowest Root Mean Squared Logarithmic Error of 0.56575 for the dataset on private fold (approximately 87% of the test data). 
