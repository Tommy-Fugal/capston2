# Capstone Project: Stock Price Analysis Over Time

## Overview

This project focuses on analyzing historical stock price data over time to uncover trends, volatility patterns, and relationships between various stock indicators. The analysis aims to provide insights that can help investors, analysts, and financial managers make more informed decisions about stock trading and portfolio management.

---

## Data Cleaning

The raw dataset, sourced from Kaggle, contained a few missing values in the 'Volume' and 'Close' price columns. These missing entries were handled by forward-filling previous known values to maintain continuity in the time series. There were no duplicate records or other anomalies in the dataset.

---

## Research Questions

I explored four primary questions:

1. How have the stock’s closing prices changed over the last 5 years?
2. What is the volatility pattern observed in the stock’s daily returns?
3. How do moving averages (short-term vs long-term) correlate with price trends?
4. Are there any seasonal patterns or anomalies in stock price movements?

---

## Question 1: Stock Closing Price Trends Over Time

![Closing Price Trend](visuals/closing_price_trend.png)

This line graph shows the stock’s closing price fluctuations over the past 5 years. The overall trend indicates a general increase, with some periods of sharp decline, often corresponding to known market events.

**Implication:** Understanding these trends can help investors time their buy/sell decisions more effectively.

---

## Question 2: Volatility of Daily Returns

![Volatility Plot](visuals/daily_volatility.png)

The daily returns’ volatility was calculated as the rolling standard deviation over a 30-day window. Peaks in volatility often correspond to economic or political events, highlighting periods of market uncertainty.

**Implication:** Investors can use volatility measures to assess risk and adjust their portfolios accordingly.

---

## Question 3: Moving Averages and Price Correlation

![Moving Averages](visuals/moving_averages.png)

Short-term (20-day) and long-term (100-day) moving averages are plotted alongside the closing prices. Crossovers between these averages often signal potential buy or sell points.

**Implication:** Traders can use these indicators as part of a technical analysis strategy to time market entry and exit points.

---

## Question 4: Seasonal Patterns in Stock Prices

![Seasonal Patterns](visuals/seasonality.png)

This chart explores seasonal trends in stock prices, highlighting recurring patterns around specific months or quarters. For instance, certain months may consistently show price increases or decreases.

**Implication:** Identifying seasonal effects can provide an edge in forecasting short-term price movements.

---

## Files Included

- `stock_analysis.ipynb`: Jupyter notebook with data cleaning, analysis, and visualization code.
- `data/`: Folder containing the Kaggle stock dataset CSV file.
- `visuals/`: Exported charts used in this report.

---

## Links to External Resources

- [Kaggle Dataset: Historical Stock Prices](https://www.kaggle.com/datasets/szrlee/stock-time-series-20050101-to-20171231)
- [Google Sheet with Summary Statistics](#) *(optional if you make one)*

---



## Conclusion

This project sheds light on key aspects of stock price behavior over time, including trends, volatility, and seasonal effects. These insights are valuable to investors and financial analysts aiming to optimize trading strategies and manage risk effectively.

---



