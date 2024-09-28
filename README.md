# CryptoVision : Advanced and Scalable Crypto Price Forecasting

Here I have tried 20 models for time series forecasting on Bitcoin dataset from 17-7-2010 to 9-9-2024 and Best performance was given be `Ensemble Model`
Scalability was done by predicting on Top 50 Crypto creating a `PandasUDF` integrating it with `Pyspark`

## Scalabiltiy Results
Percentage Improvement in Speed: `7784.80%`

PySpark is `78.85` times more scalable than Pandas.

## Model Comarison Results
![newplot](https://github.com/user-attachments/assets/9c876dca-4725-4173-bd86-250d761a4d4e)

## Statistical Models
1. AR 
2. MA
3. ARMA
4. AIRMA
5. SARIMA
6. Naive Forecast
7. AutoARIMA
8. ExponentialSmoothing (Requires Smoothening)

## Machine Learning Methods
9. Random Forest (TF-DF)
10. Gradient Boosted Trees (TF-DF)
11. Prophet (Facebook Kats) (Requires Smoothening)
12. Dense Model (Window = 7, Horizon = 1)
13. Dense Model (Window = 30, Horizon = 1)
14. Dense Model (Window = 30, Horizon = 7)
15. Conv1D (Window = 7, Horizon = 1)
16. LSTM (Window = 7, Horizon = 1)
17. Dense (Multivariate Time series)
18. N-BEATs Algorithm
19. Ensemble
20. Simple ANN Model (Future Predictions)

## Preprocessing Steps
1. Checking if series is stationary
   Using `Augmented Dickey Fuller Test`
2. Making the series stationary
   Using `Differencing`
3. Plotting `ACF` and `PACF` plots
   According to the plots mostly both the plots were same and the first lag was negative second lag onwards many lags were below the threshold

# Conclusion 
1. The test dataset was of 362 days (around 1 year) this is the main reason why the forecast of FB-Prophet, ARIMA, ARMA, AR, MA etc are not so good.
