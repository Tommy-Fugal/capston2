# Capstone Project: Comprehensive Stock Price Analysis Over Time

---

## Overview

This project undertakes a detailed analysis of historical stock price data to explore trends, volatility, and patterns that are critical for investors and financial analysts. By examining daily stock prices over multiple years, this analysis identifies key insights that inform trading strategies, risk management, and portfolio optimization.

The dataset used comes from Kaggle and contains daily stock prices and volumes for multiple companies from 2005 through 2017. Through exploratory data analysis (EDA), visualization, and statistical methods, the project reveals how stock prices evolve over time, the nature of their volatility, and how technical indicators such as moving averages relate to price trends.

This information is valuable for portfolio managers, traders, and financial advisors looking to optimize their decision-making process based on quantitative evidence.

---

## Data Cleaning

The dataset initially contained daily stock prices for various companies, with columns including `Date`, `Open`, `High`, `Low`, `Close`, `Volume`, and `Name` (ticker symbol).

### Initial Assessment:

- **Missing Values**: Several records had missing values in `Volume` and occasionally in `Close` prices due to holidays or market anomalies.
- **Duplicates**: No duplicate rows were found.
- **Data Types**: The `Date` column was converted to datetime format for proper time series analysis.
- **Inconsistent Tickers**: Some ticker names were inconsistent in case or contained trailing spaces; these were standardized.

### Cleaning Steps:

1. **Imputation**: Missing `Volume` and `Close` values were forward-filled (`ffill`) to maintain continuity without biasing with zeros.
2. **Filtering**: Analysis was focused on a selected subset of companies with complete data records over the full time period to ensure comparability.
3. **Sorting**: Data sorted by `Name` and `Date` to preserve chronological order for each stock.
4. **Feature Engineering**: New columns for daily returns (`pct_change()` of `Close`) and rolling statistics (moving averages and rolling volatility) were added.

This thorough cleaning ensures reliable inputs for the subsequent analysis.

---

## Research Questions

Four primary questions guided this analysis:

1. **What are the long-term trends in stock closing prices across selected companies?**
2. **How does daily volatility behave over time, and what are its patterns?**
3. **How do technical indicators, specifically moving averages, relate to price movements?**
4. **Are there identifiable seasonal or cyclical patterns in stock price behavior?**

---

## Question 1: What are the long-term trends in stock closing prices?

![Closing Price Trend](visuals/closing_price_trend.png)

The plot above shows the historical closing prices for three major companies over 12 years (2005–2017). We observe distinct upward trends for most stocks, punctuated by periods of downturns, notably during the 2008 financial crisis and market corrections in 2011 and 2015.

- **Insights:**
  - Long-term growth is evident but not linear, emphasizing the importance of timing in investment decisions.
  - Price dips correspond to well-documented macroeconomic events, validating the dataset's accuracy.
  - Investors can leverage these trends to strategize buy-and-hold versus active trading approaches.

---

## Question 2: How does daily volatility behave over time?

![Volatility Over Time](visuals/rolling_volatility.png)

Volatility was computed as the 30-day rolling standard deviation of daily returns. The graph highlights spikes in volatility during crisis periods, for example:

- 2008–2009: Global financial crisis, highest volatility observed.
- Mid-2011: Eurozone debt crisis with sharp price fluctuations.
- Early 2016: Oil price collapse reflected in increased volatility.

- **Insights:**
  - Volatility clustering shows that turbulent periods tend to persist.
  - Recognizing volatility regimes can help investors adjust risk exposure.
  - Volatility forecasts can be integrated into portfolio management and option pricing models.

---

## Question 3: How do moving averages relate to price trends?

![Moving Averages](visuals/moving_averages.png)

This chart compares the 20-day short-term and 100-day long-term moving averages against the closing price of a stock.

- Crossovers where the short-term MA crosses above the long-term MA are often considered **bullish signals** (buy).
- Crossovers below the long-term MA may indicate **bearish signals** (sell).
- The moving averages smooth out short-term noise and help identify trend direction.

- **Insights:**
  - Moving average signals align with major trend shifts in the stock price.
  - Investors can use these to time entries and exits.
  - The strategy’s effectiveness varies across market conditions, requiring complementary indicators for robustness.

---

## Question 4: Are there seasonal or cyclical patterns in stock prices?

![Seasonality Analysis](visuals/seasonality.png)

Seasonal decomposition of stock prices reveals:

- Mild seasonality in some months — for example, higher average returns in December and January, often attributed to the "January effect."
- Lower performance or higher volatility observed in summer months (June–August), consistent with lower market activity.
- No uniform pattern across all stocks, suggesting seasonality is company or sector-specific.

- **Insights:**
  - Recognizing seasonal effects can provide tactical advantages.
  - Portfolio managers can allocate or hedge positions based on expected seasonal trends.
  - Seasonal analysis should be combined with fundamental data for better accuracy.

---



## External Resources and Dataset Links

- Kaggle Dataset: [Historical Stock Prices 2005-2017](https://www.kaggle.com/datasets/szrlee/stock-time-series-20050101-to-20171231)
- Additional Financial Data and Documentation (if used)

---



## Conclusion

This project presents a thorough exploration of stock price dynamics using historical data. Key findings include:

- Stock prices show strong but non-linear long-term growth trends affected by economic events.
- Volatility exhibits clear clustering during crisis periods, offering opportunities for risk assessment.
- Moving averages serve as valuable trend-following indicators but should be used in conjunction with other tools.
- Seasonal patterns exist but are not universal, highlighting the complexity of market behavior.

These insights can guide investors and financial professionals in crafting informed, data-driven strategies that balance risk and reward in volatile markets.

---

