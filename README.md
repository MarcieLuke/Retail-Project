# Retail-Project

The dataset consists of turnover across time for cafes, restaurant, and catering services in South Australia. 

Firstly, I explore statistical features of the data such as the trend, volatility, and seasonality. 

The data is modelled using ETS and ARIMA. 
After fitting the model, forecast is then produced for the last 24 months of the original dataset, to compare how similar the forecast and the actual data which can tell how well the model has captured the information. It is then determined that in this case, ARIMA has better accuracy due to lower RMSE AND MASE comapred to ETS model. 

Forecast for the next 2 years of the turnover is also produced using the best ETS and ARIMA model which has been trained previously. The forecast is the compared to the next 2 years actual data and it shows that in this case ETS model performs better in terms of accuracy, which is in contrast to the result obtained when I use the model to forecast the last 24 months data, where ARIMA model has better accuracy. 

From the project, there are benefit and limitation of the model. 
The advantage of ARIMA on this data is that we see a strong autocorrelation in the data. So, an ARIMA model can do well in incorporating past data to forecast into the future.

Some major disadvantages of ARIMA forecasting are the process of choosing the order can be subjective. Thus, the reliability of the chosen model can depend on the skill and experience of the forecaster. Also, ARIMA model cannot perform well in change of trend as well as the ETS model.

The benefit of ETS model is that it gives more weight to recent observations. It is also possible to adjust the parameter values to change how quickly older observation lose their importance. ETS model also do not need the data to be stationary.
