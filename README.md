# LinearRegression
This is the house prediction model, using Linear Regression and Decision Tree Regressor

The Dataset used, is from Kaggle "House Prices - Advanced Regression Techniques" (kaggle competitions download -c house-prices-advanced-regression-techniques)

In the train set there are 79 feature attributes plus ID and the label or class attribute, and 1460 rows or tuples.
the test set has the same features, but there is not any label class.

These are the steps taken for the prediction:
1- the tabular datasets were loaded.
2- the 10 most contributing attributes we found using the heatmap
3- some of the attributes from the last step were correlated, so one of them was chosen.
4- the outliers were checked and then removed
5- the 'SalePrice' column was removed from the train set
6- the null values were checked and as there were very few null values in the important attributes, so they were imputed with zero.
7- Robust Scaler was used to scale the numerical attributes
8- three models (Linear Regression, Decision Tree, and Random Forest) were trained using the 80% of the train set (5-fold), and the MAE and RMSE of the three models were compared. 
9- the best model was Linear Regression with the least error
10- Linear Regression was used to predict the house prices.
