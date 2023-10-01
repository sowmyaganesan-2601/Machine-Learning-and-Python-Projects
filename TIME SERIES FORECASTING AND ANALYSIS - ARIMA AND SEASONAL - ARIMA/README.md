
#  TIME SERIES FORECASTING AND ANALYSIS - ARIMA AND SEASONAL - ARIMA

Time series analysis is a specific way of analyzing a sequence of data points collected over an interval of time. In time series analysis, analysts record data points at consistent intervals over a set period of time rather than just recording the data points intermittently or randomly.

# Time Series can be broken down into 3 components:
1)  Trend: Upward & downward movement of the data with time over a large period of time (i.e. house appreciation)
2) Seasonality: Seasonal variance (i.e. an increase in demand for ice cream during summer)
3) Noise: Spikes & troughs at random intervals.
# Types of Time Series:
1) Stationary Time Series :
The observations in a stationary time series are not dependent on time.
Time series are stationary if they do not have trend or seasonal effects. Summary statistics calculated on the time series are consistent over time, like the mean or the variance of the observations.
When a time series is stationary, it can be easier to model. Statistical modeling methods assume or require the time series to be stationary to be effective.
2) Non-Stationary Time Series:
Observations from a non-stationary time series show seasonal effects, trends, and other structures that depend on the time index.
Summary statistics like the mean and variance do change over time, providing a drift in the concepts a model may try to capture.
Classical time series analysis and forecasting methods are concerned with making non-stationary time series data stationary by identifying and removing trends and removing seasonal effects.
# For a time series to be stationary it has to satisfy the below conditions:
1) The mean of the series should not be a function of time. The red graph below is not stationary because the mean increases over time.
2) The variance of the series should not be a function of time. This property is also known as Homoscedasticity. The red graph below is not stationary because of the varying spread of data over time.
3) Finally, the Covariance of the i’th term and the (i+m)’th term should not be a function of time, i.e. it is only a function of Gap. In the red graph you can notice that the spread becomes closer as the time increases. Hence the Covariance is not constant with time
# Autoregressive models 
Autoregressive models  operate under the premise that past values have an effect on current values. AR models are commonly used in analyzing nature, economics, and other time-varying processes. As long as the assumption holds, we can build a linear regression model that attempts to predict value of a dependent variable today, given the values it had on previous days. p is a parameter of how many lagged observations to be taken in.
# Integrated(I):
A model that uses the differencing of raw observations (e.g. subtracting an observation from the previous time step). Differencing in statistics is a transformation applied to time-series data in order to make it stationary. This allows the properties do not depend on the time of observation, eliminating trend and seasonality and stabilizing the mean of the time series.
#  Moving Average Model
 Moving Average Model process  states that the current value is linearly dependent on the current and past error terms. Again, the error terms are assumed to be mutually independent and normally distributed, just like white noise.
 # AutoRegressive Integrated Moving Average (ARIMA):
The ARIMA (aka Box-Jenkins) model adds differencing to an ARMA model. Differencing subtracts the current value from the previous and can be used to transform a time series into one that’s stationary. 
Three integers (p, d, q) are typically used to parametrize ARIMA models.
p: number of autoregressive terms (AR order)
d: number of nonseasonal differences (differencing order)
q: number of moving-average terms (MA order)
#The general process for ARIMA models is the following:

1) Visualise the Time Series Data
2) Make the time series data stationary
3) Plot the Correlation and AutoCorrelation Charts
4) Construct the ARIMA Model or Seasonal ARIMA based on the data
5) Use the model to make predictions
# Seasonal-ARIMA(SARIMA):
As the name suggests, this model is used when the time series exhibits seasonality. This model is similar to ARIMA models, we just have to add in a few parameters to account for the seasons.
We write SARIMA as
ARIMA(p,d,q)(P, D, Q)m,
p — the number of autoregressive
d — degree of differencing
q — the number of moving average terms
m — refers to the number of periods in each season
(P, D, Q ) — represents the (p,d,q) for the seasonal part of the time series
Seasonal differencing takes into account the seasons and differences the current value and it’s value in the previous season eg: Difference for the month may would be value in May 2018 — value in may 2017.

Refer to - https://medium.com/analytics-vidhya/time-series-forecasting-and-analysis-arima-and-seasonal-arima-cacaf61ae863#:~:text=The%20general%20process%20for%20ARIMA%20models%20is%20the%20following%3A&text=Make%20the%20time%20series%20data,the%20model%20to%20make%20predictions
for more information about this project