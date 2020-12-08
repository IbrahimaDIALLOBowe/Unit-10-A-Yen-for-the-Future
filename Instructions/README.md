# Unit 10—A Yen for the Future

![Yen Photo](Images/unit-10-readme-photo.png)

## Background

The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.



#### Time-Series Forecasting

The first part of the analysis, privide by the 'time_series_analysis.ipynb' notebook, contains code to model the short-term price movement of Yen with respect to the US Dollar.

The Hodrick-Prescott Filter is used to extrac noise data and isolate the daily returns. The price modeling is perfomed using ARIMA and ARMA models. The volatility  is modeled with GARCH 




### CONCLUSIONS:

Based on the time series analysis, I would not recommand buying the Yen, both models (ARIMA and ARMA) have a P > 0.05. However, they are not significant. 

The risk of YEN is expected to increase, therefore we are seeing the GARCH model is predicting volatility, the Yen will keep increasing in the next few days.

Base on the models, I would not feel confortable using either ARIMA or ARMA for trading which is requires directional prediction. ARIMA and ARMA are not accurate. Even though showing or helping us to understand better the volatitlity in this case there encouraging to diversified our portfolio for a future investments.

#### Linear Regression Forecasting

In the second part of the analysis in notebook, the Scikit-Learn linear regression model to predict Yen futures ("settle") returns with *lagged* Yen futures returns and categorical calendar seasonal effects. 
 
After splitting the returns and lagged returns into training and testing data, the linear Regression Model is a fit. Predictions are compared with known test data and the model performance is evaluated.

The following performance metrics were computed:

|Metric| In-Sample |Out-Of-Sample|
|-|-|-|
|Mean Squared Error (MSE) |0.35565249959422596|0.17262635470120388|
|Root Mean Squared Error|0.5963660785073426|0.4154832784856737|





#### 1. Does this model perform better or worse on out-of-sample data compared to in-sample data?
the Scikit-Learn linear regression model performs with similar error metrics in both the in-sample and out-of-sample datesets. In-sample has a slightly better MSE, and out-of-sample a very slightly better RMSE. Performance can be considered "consistent" accross both datasets.

### CONCLUSIONS:

In the regression analysis, the comparaison of the two models give us: the out-of-sample performed than the In-sample data. The out-of-sample have a root mean squared error of 0.415, while the in-sample data has an RMSE of 0.596
- - -


