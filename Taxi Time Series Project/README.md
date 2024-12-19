# Problem Description:
https://github.com/Nate-hub5/Portfolio/blob/main/Taxi%20Time%20Series%20Project/Taxi%20Time%20Series%20Project.ipynb 

Analyzed historical data on airport taxi orders to explore patterns and predict the number of taxi orders expected in the next hour. The goal was to create a predictive model that can help optimize driver availability during peak times, ensuring better service and increased efficiency.

# Table of Contents

1. Download and Prepare Data:
2. EDA
3. Feature Engineering
4. Model Training
5. Validation and Model Selection
6. Testing and Performance Evaluation
7. Conclusion and Recommendations


# Project Instructions:

**1. Download and Prepare Data:**
* Loaded the dataset and parsed the datetime column.
* Resampled the data to hourly intervals using resample('1h').

**2. EDA**
* Visualized trends in the time series with hourly taxi orders.
* Analyzed the distribution of orders using histograms.
* Performed seasonal decomposition to explore trends, seasonality, and residuals.
* Printed summary statistics for trends, seasonality, and residuals.
* Analyze the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) plots to identify significant lags.

**3. Feature Engineering**
* Created lag features such as lag_1, lag_3, lag_5, lag_24, and lag_48 to capture short-term and daily dependencies.
* Added rolling mean and standard deviation features over 3-hour, 7-hour, 14-hour, 24-hour, and 48-hour windows.
* Engineered time-based features like hour, day_of_week, and is_weekend.
* Decomposed the data into trend, seasonal, and residual components.
* Addressed multicollinearity by removing highly correlated features using a correlation
* Used PolynomialFeatures with degree=2 to add squared terms and interactions for non-linear relationships.

**4. Model Training**
* Trained multiple models (Decision Tree, Random Forest, Linear Regression).
* Performed hyperparameter optimization using GridSearchCV for Decision Tree and Random Forest.
* Performed linear regression with polynomial features.

**5. Validation and Model Selection**
* Use TimeSeriesSplit (5 splits) to validate model performance on the training data.
* Perform hyperparameter tuning with GridSearchCV to find the optimal parameters for each model.
* Compare models (Decision Tree, Random Forest, Linear Regression with polynomial features) using Root Mean Squared Error (RMSE) as the evaluation metric.

**6. Testing and Performance Evaluation**
* Evaluate the Best Model on the Test Set
* Visualize Model Predictions
* Plot residuals (Actual - Predicted) for the best-performing models to check for systematic patterns.
* Plot histograms to analyze the distribution of errors.

**7. Conclusion and Recommendations**
* Model Performance
* Practical Recommendations
* Future Improvements 


