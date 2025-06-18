# 📊 Apple Inc. Stock Analysis – Capstone Project

## 📝 Overview

This Capstone project analyzes historical stock data for **Apple Inc. (AAPL)** to uncover relationships between key market indicators: **price volatility**, **trading volume**, and **closing price**. By combining data visualizations with quantitative analysis, we aim to better understand patterns in Apple’s stock behavior and what they can tell us about investor sentiment and market dynamics.

Apple Inc. is one of the most influential technology companies in the world. Because of its global presence, massive customer base, and groundbreaking product releases (like the iPhone, iPad, and MacBooks), Apple’s stock tends to respond sharply to both company-specific news and broader economic events. These responses are often visible in the form of volatility spikes, volume surges, and price swings.

In this report, we answer the following three questions using historical AAPL data and Power BI-generated visuals:

1. What is the volatility trend, and what could be causing the spikes?
2. Is there a relationship between volume and closing price?
3. What is the overall trend in price over time?

---

## 📈 1. What is the volatility trend, and what could be causing the spikes?

### 📊 Chart Overview

The first chart is a **line graph** showing the **sum of daily volatility** over the course of a month (August). Daily volatility was calculated using the formula:

```
Volatility = (High - Low) / Open
```

This ratio shows how much the price moved in a day relative to its opening price — a useful indicator of risk and market uncertainty.

### 🔍 Key Findings

- We observe significant **volatility spikes** on:
  - **August 10**
  - **August 17**
  - **August 27**
- These spikes reached **above 0.6**, which is quite high for a single day.
- For reference, if Apple opened at **$150**, a volatility of 0.6 would imply a price movement range of:
  ```
  $150 * 0.6 = $90
  ```
  Meaning Apple could have swung between $105 and $195 during the day.

### 📅 Possible Explanations for Volatility Spikes

Volatility is often triggered by **external or internal catalysts**:

- **Quarterly earnings reports** often occur in mid-to-late August, which can dramatically affect investor sentiment.
- **Product launch rumors** (such as new iPhones or Apple Watch updates) can lead to increased speculative trading.
- **Macroeconomic news** such as Federal Reserve announcements, interest rate hikes, or inflation data could also spike volatility.
- **Geopolitical events** or global market turbulence may have created broader uncertainty.

### 📌 Conclusion

The observed spikes in volatility are not random — they likely align with **key events** that influence investor behavior. For traders, these are crucial windows for potential gains (or losses), and for long-term investors, they are moments to watch for price corrections or buying opportunities.

---

## 🔄 2. Is there a relationship between volume and closing price?

### 📊 Chart Overview

The second chart is a **scatter plot** comparing **trading volume (X-axis)** with **closing price (Y-axis)**. Each dot represents a trading day, and a **trendline** has been added to show the correlation.

### 🔍 Key Findings

- There is a **clear negative correlation** between volume and closing price.
- High closing prices (above $100) typically occur when the trading volume is **low** (under 0.1 billion shares).
- Lower closing prices (below $50) often occur when the volume is **very high** (approaching or exceeding 0.5 billion shares).
- The scatter plot shows clustering:
  - **Top-left**: High prices, low volume
  - **Bottom-right**: Low prices, high volume

### 📉 Quantitative Analysis

The trendline suggests a **linear inverse relationship** that can be modeled (approximately) as:

```
Closing Price = a + b(Volume), where b < 0
```

Although we don’t have the exact regression equation, the downward slope of the trendline confirms the negative relationship. If we approximate:

- A day with **0.1 billion volume** → average closing price near **$120**
- A day with **0.5 billion volume** → average closing price near **$40–$50**

This implies a ~**60–70% drop** in price associated with massive increases in volume. While this doesn't imply causation, it strongly indicates that **volume spikes are often tied to sell-offs**, panic trading, or reaction to bad news.

### 📌 Conclusion

There is a significant inverse relationship between Apple’s volume and closing price. This suggests that traders and investors may be reacting to bad news with heavy selling, which increases volume but pushes the price downward. Long-term investors might interpret these dips as buying opportunities.

---

## 📊 3. What is the overall trend in price over time?

### 📊 Chart Overview

The third chart displays the **30-Day Rolling Average Closing Price** of AAPL stock from **2006 to 2017**. This smooths out short-term fluctuations and highlights longer-term trends in the stock price.

### 🔍 Key Findings

- The trend is overwhelmingly **upward**.
- Major growth periods:
  - **2006–2009**: Modest rise
  - **2010–2013**: Steady climb due to iPhone expansion
  - **2014–2017**: Significant jump in price momentum
- In 2006, the 30-day average closing price was approximately **$15**
- By 2017, it had climbed to over **$170**

### 📈 Quantitative Growth Calculation

To calculate total growth from 2006 to 2017:

```
Growth = ((170 - 15) / 15) * 100 = 1033.33%
```

This means Apple stock grew by over **1000%** in just over a decade.

### 💡 Interpretation

This growth can be attributed to:
- Continuous innovation (iPhone, iPad, App Store)
- Growing global market share
- Strong balance sheets and consistent profitability
- Strategic stock buybacks and dividend payments

Even though short-term volatility exists, the long-term trend has shown massive capital appreciation for Apple shareholders.

### 📌 Conclusion

Apple’s long-term price trajectory is a strong upward trend, reflecting its transformation from a hardware company into a global tech ecosystem. The 30-day rolling average shows sustainable growth and supports Apple’s reputation as a reliable long-term investment.

---

## ✅ Final Summary

| **Metric**            | **Insight**                                                                 |
|-----------------------|------------------------------------------------------------------------------|
| **Volatility**        | Spikes occur around key events; often >0.6 (60% daily movement)              |
| **Volume vs. Price**  | Negative correlation: high volume = lower price (indicates reactionary selloffs) |
| **Long-Term Trend**   | Apple grew over 1000% from 2006–2017, showing strong long-term performance   |

This analysis illustrates how daily data and broader trends can work together to explain Apple’s stock behavior. For traders, understanding volume and volatility is key to timing. For investors, the long-term trend provides reassurance of Apple’s enduring value.

---
