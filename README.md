# GDP Forecasting with ARIMA

Time-series forecasting of GDP for the G7 countries (USA, Canada, UK, France, Germany, Italy, Japan) using ARIMA, with an emphasis on understanding the statistical theory behind the model rather than treating it as a black box.

## Approach

- **Data**: World Bank GDP data (USD), 1975–2024, for all seven G7 countries
- **Model selection**: `auto_arima` selects a country-specific ARIMA(p,d,q) order per country (e.g. Italy: ARIMA(0,2,1), Japan: ARIMA(2,2,3), UK: ARIMA(3,2,2))
- **Validation**: 80/20 train-test split — each country's model is evaluated on the held-out test period before refitting on the full series
- **Forecast**: refit models project GDP 16 years forward (2025–2040)
- **Theory**: includes a written derivation (`ARIMA theory.pdf` / `.tex`) revisiting the mathematical foundations of ARIMA — autoregression, differencing, and moving-average components — rather than applying the model as a black box

## Technologies

Python · pandas · pmdarima (`auto_arima`) · statsmodels · World Bank GDP data
