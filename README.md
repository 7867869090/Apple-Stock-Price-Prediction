# 📈 Apple Stock Price Prediction

This project predicts the **closing price** of **Apple Inc. (AAPL)** stock using historical stock data and a **Linear Regression** model.

---

## 🎯 Objective
The objective of this project is to **predict the closing price** of Apple Inc. (AAPL) based on historical data and engineered features such as moving averages.

---

## 📂 Dataset

- **Source:** Downloaded using the [`yfinance`](https://pypi.org/project/yfinance/) library  
- **Date Range:** January 1, 2020 → December 31, 2023  
- **Ticker:** AAPL

**Features:**
- `Open` → Opening price of the day  
- `High` → Highest price of the day  
- `Low` → Lowest price of the day  
- `Close` → Closing price of the day (**Target Variable**)  
- `Volume` → Number of shares traded  
- `MA10` → 10-day Moving Average (new feature)  
- `MA50` → 50-day Moving Average (new feature)  

---

## 🤖 Model Used
- **Algorithm:** Linear Regression (`sklearn.linear_model.LinearRegression`)  
- **Workflow:**
  1. Load and inspect data  
  2. Calculate moving averages (MA10 & MA50)  
  3. Split data into **training** and **testing** sets  
  4. Train Linear Regression model  
  5. Evaluate performance using MAE, MSE, and R²  

---

## 📊 Key Results

- **Mean Absolute Error (MAE):** `0.7295`  
- **Mean Squared Error (MSE):** `0.8888`  
- **R² Score:** `0.9990`  

**Insights:**
- The scatter plot of **actual vs. predicted** prices shows a **strong positive correlation**, indicating high accuracy.  
- **Box plots** revealed possible outliers in the `Volume` feature.  
- Adding moving averages improved model performance.  
- A high **R² score** suggests the model explains most of the variance in closing prices.

---

## 📈 Visualizations
- **Scatter Plot:** Actual vs. Predicted Closing Prices  
- **Box Plot:** Volume outlier detection  
- **Line Chart:** Closing price trends over time  

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- scikit-learn  
- yfinance  

---

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).
