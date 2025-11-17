GDP Forecasting with ARIMA

In some cases machine learning models as well as statistical models may be applied as a black-box to the satisfaction of all concerned. However, more often, a carful examination of the mathematical reasonning behind common practices is in order. In this notebook, I use GDP data to forecast future values in order to illustrate how a deeper understanding of the ARIMA algorithm improves the modelling process. As a second focus, I will sieze this opportunity to revisit some basic building blocks of ARIMA.

Gross Domestic Product (GDP) measures a country’s economic productivity and serves as an indicator of the size and health of its economy.

ARIMA is a well-known algorithm for time-series forecasting based on autoregressive and moving-average components.

I use WorldBank data GDP data between 1975 and 2024 to predict 2025-2040 GDP for the G7 countries: USA, Canada, United Kingdom, France, Germany, Italy, and Japan.