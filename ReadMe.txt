Contributers: Aditya SE20UARI006, Rohith SE20UARI072, Abhinav SE20UCSE006

We start by importing necessary libraries: pandas, scikit-learn, and SimpleImputer.

Training dataset is loaded from the CSV file "Train.csv".
We perform data preprocessing steps, and convert the "week" column into date-time format and henceforth separate the year, month and day (week reference).

Further, independent variables in the model(X) and 'units_sold' is the target variable (y).

In case of missing values, filling them with mean of fature values using imputer.

After splitting the dataset, Training set(X_train, y)train is used for training, and testing set(X_test, y_test) for performance evaluation. (Test size = 20% of the data).

With 100 decision trees, a random forest Regerssor model is created, estimators set to 100 and fixed radom seed to 42.

Training using "model.fit(X_train, y_train)".

Predictions using "model.predict(X_test)".

For model performance, MSE is calculated by comparing test values and predicted values(y_pred).

The Lower the MSE, the better the model's predictive performance.