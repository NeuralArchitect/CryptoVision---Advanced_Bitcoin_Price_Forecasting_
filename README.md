# CryptoVision : Advanced Bitcoin Price Forecasting

Here I have tried these many model for time series forecasting on Bitcoin dataset from 17-7-2010 to 9-9-2024

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
12. Silverkite (LinkedIn Greykite) (Requires Smoothening)
13. Dense Model
14. Same as 1
15. Same as 1
16. Conv1D
17. LSTM
18. Same as 1 but multivariate
19. N-BEATs Algorithm
20. Ensemble
21. Future Prediction model
22. Same as 1 but with turkey data introduced
Same as 1 but with turkey data introduced

## Preprocessing Steps
1. Checking if series is stationary
   Using `Augmented Dickey Fuller Test`
2. Making the series stationary
   Using `Differencing`
3. Plotting `ACF` and `PACF` plots
   According to the plots mostly both the plots were same and the first lag was negative second lag onwards many lags were below the threshold
