# prophet_time_series
Notebook to create an aggregated (monthly) time series prediction based on daily data with Prophet.
The notebook allows to set the parameters (start and end dates for training, cross-validation, test and hold-out, and forecast horizon). 
An ad-hoc cross-validation function which takes in a given list of dates (instead of Prophet's automatic calculation of such dates) and calculates predictions for the chosen horizon is created.
Regressors are considered and added.
Aggregated predictions are given with and without an estimation of the error. The first is carried out by calculating sample predictions whereas the second only by summing up the daily predictions..
A comparison to a baseline model is also carried out, to check the actual ability to predict of the model. These comparison and the goodness of the model are assessed with MAE, MSE and RMSE errors.
