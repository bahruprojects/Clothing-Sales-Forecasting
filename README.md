# Clothing-Sales-Forecasting
## Summary:

### Data Analysis Key Findings

*   The initial monthly Omzet time series was found to be non-stationary based on the Augmented Dickey-Fuller (ADF) test (p-value = 0.288).
*   Applying first-order differencing did not achieve stationarity (p-value = 0.731).
*   Applying second-order differencing also did not result in a stationary time series based on the ADF test (p-value = 0.424).
*   Despite the lack of confirmed stationarity after differencing, ACF and PACF plots were generated for the second-order differenced series to help identify potential p and q parameters for the ARIMA model.
*   An ARIMA model with order (1, 2, 1) was successfully built and trained on the `monthly_omzet` data.
*   The ARIMA model forecasted the Omzet for the next three months as approximately \Rp2.43 billion (January 2024), \Rp2.64 billion (February 2024), and \Rp2.79 billion (March 2024).
*   A visualization was successfully generated comparing the original monthly Omzet data with the forecasted values for the next three months.

### Insights or Next Steps

*   Although the ADF test did not confirm stationarity even after second-order differencing, the forecasting process was completed. It would be beneficial to investigate alternative methods for stationarity or explore other time series models better suited for non-stationary data if the model performance is not satisfactory.
*   The forecasted values show a potential increasing trend in Omzet for the next three months. It would be valuable to validate these forecasts with business knowledge and consider the confidence intervals around these predictions if they were available.
