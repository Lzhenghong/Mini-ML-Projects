Summary:
Predict prices of Bitcoin using Neural Network Time Series

Dataset:
Coindesk data (https://raw.githubusercontent.com/mrdbourke/tensorflow-deep-learning/main/extras/BTC_USD_2013-10-01_2021-05-18-CoinDesk.csv)

Description:
- Split data into training and testing set
- Build and fit a Vanilla Neural Network using window size of 7 days and horizon of 1 day (model 1)
- Build and fit a Vanilla Neural Network using window size of 30 days and horizon of 1 day (model 2)
- Build and fit a Vanilla Neural Network using window size of 30 days and horizon of 7 days (model 3)
- Build and fit a Convolutional 1D model using window size of 7 days and horizon of 1 day (model 4)
- Build and fit an LSTM model using window size of 7 days and horizon of 1 day (model 5)
- Feature engineer block rewards into datasets and fit a Multivariate model using window size of 7 days and horizon of 1 day (model 6)
- Replicate and fit an N-BEATS model using window size of 7 days and horizon of 1 day (model 7)
- Build and fit an Ensemble of 3 models using MAE, MSE and MAPE as loss functions, and HeNormal Kernel Initialiser
- Compare the MAE of models 1 to 8
- Plot predictions and their 95% confidence interval bands

Results:
- Model 1 (569)
- Model 2 (606)
- Model 3 (1238)
- Model 4 (571)
- Model 5 (595)
- Model 6 (568)
- Model 7 (572)
- Model 8 (567)
