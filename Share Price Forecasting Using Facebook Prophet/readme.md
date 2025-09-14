#  Share Price Forecasting Using Facebook Prophet

Time series forecast can be used in a wide variety of applications such as Budget Forecasting, Stock Market Analysis, etc. But as useful it is also challenging to forecast the correct projections, Thus can't be easily automated because of the underlying assumptions and factors. The analysts who produced accurate forecasts are also rare, and there is a big market available for them because it requires a substantial understanding of statistics and data analysis and has prior experience of producing time series forecasting.

Facebook open-sourced its time-series forecasting tool called Prophet in 2017 which produced accurate forecasts as produced by skilled analysts with a minimum amount of human efforts. The Facebook prophet is available in the form of API in Python and R/

## How Prophet Works:

Facebook Prophet using Additive Regressive models using the following four components:
```
y(t) = g(t) + s(t) + h(t) + \epsilon_t
```
- g(t): A piecewise linear or logistic growth curve trend. Prophet automatically detects changes in trends by selecting change points from the data.
- s(t): A yearly seasonal component modeled using the Fourier series and weekly seasonal component using dummy variable
- h(t): A user-provided list of important holidays.
- et:  Error term used by the prophet.
  
## Advantages of Facebook Prophet:

the prophet is optimized for business-related problems that are encountered at Facebook, it has the following characteristics:

The Facebook prophet is as accurate as a skilled analyst and can generate results in seconds
Facebook prophet requires minimal data processing and can deal with several outliers and null values.
User can add seasonality and holidays values manually, this can help easily integrate the particular domain knowledge.
In this post, we will use Facebook prophet with Python. We try to forecast the share price of Amazon Stock (from 2019-2020) using the share price data from (2015-2019).

## Implementation:

First, we need to install the prophet tool, it can be installed with the following command in python.
```
!pip install prophet
```
