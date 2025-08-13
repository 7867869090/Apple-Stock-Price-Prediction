# Apple-Stock-Price-Prediction
**Task Objective:**
The objective of this project is to predict the closing price of Apple Inc. (AAPL) stock using historical stock data.

**Dataset Used:**
The dataset used in this project is historical stock data for Apple Inc. (AAPL) from January 1, 2020, to December 31, 2023, downloaded using the yfinance library. The dataset includes the following columns:

Open: The opening price of the stock for the day.
High: The highest price of the stock for the day.
Low: The lowest price of the stock for the day.
Close: The closing price of the stock for the day (the target variable).
Volume: The number of shares traded during the day.
Additionally, two moving averages (MA10 and MA50) were calculated as new features for the model.

**Models Applied:**
A Linear Regression model from the sklearn.linear_model library was applied to predict the closing price of the stock.

**Key Results and Findings:**
The historical stock data for Apple Inc. (ticker: AAPL) was successfully downloaded and explored.
The data was split into training and testing sets.
A Linear Regression model was trained on the training data.
The model's predictions were evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared.
The scatter plot of actual vs. predicted closing prices shows a strong positive correlation, indicating good model performance.
The box plots revealed potential outliers in the Volume data.
After adding moving averages as features, the model's performance metrics were as follows:
Mean Absolute Error (MAE): 0.7295
Mean Squared Error (MSE): 0.8888
R-squared: 0.9990
The high R-squared value suggests that the model explains a significant portion of the variance in the closing price.
