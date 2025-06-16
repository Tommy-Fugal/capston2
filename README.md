# Capstone Project: NBA 2023-2024 Playoff Player & Team Stats Analysis

## Overview

In this project, I focused on analyzing various statistics from players and teams that participated in the 2023-2024 NBA playoffs. This information can be applicable to NBA coaches and managers because I analyzed statistics that correlate with higher success within the games. Using the correlations and patterns determined through my data processing, NBA executives can leverage this information to create the best teams and lineups that maximize their probability of winning games.

---

## Data Cleaning

The raw dataset used contained no duplicates or missing/null values. The only data correction involved fixing a few player name misspellings to ensure accuracy and consistency across analyses.

---

## Research Questions

I analyzed four key questions to uncover valuable insights:

1. How does minutes per game correlate with points per game?
2. How does player age correlate with points per game?
3. How does scoring efficiency change with points per game?
4. What is the relationship between 2-point shot percentage and 3-point shot percentage?

---

## Question 1: Minutes per Game vs Points per Game

![Scatter Plot of Minutes vs Points](visuals/minutes_vs_points.png)

This scatter plot shows a positive correlation between minutes played and points scored, with points on the y-axis and minutes on the x-axis. The trend line indicates that on average, more minutes result in more points scored. The calculated R² value is approximately 0.54, indicating a moderate positive relationship. 

**Implication:** NBA coaches and managers can use this insight to justify giving their best players more playing time to maximize scoring potential and improve game outcomes.

---

## Question 2: Age vs Points per Game

![Age vs Points Scatter Plot](visuals/age_vs_points.png)

This graph investigates the relationship between player age and points per game. Contrary to my initial hypothesis that peak scoring would occur between ages 25-30, the data shows no significant correlation (R² ≈ 0.038). Notably, players under 20 generally scored less than 10 points per game, and most players over 35 scored under 15 points, except for one outlier.

**Implication:** Age alone is not a reliable predictor for scoring ability, so age should not heavily influence decisions about player roles in scoring lineups.

---

## Question 3: Efficiency vs Points per Game

![Efficiency vs Points](visuals/efficiency_vs_points.png)

This chart shows field goal percentage (FG%) versus points per game, with players sorted descending by points. High scorers (20+ PPG) maintain FG% between 40-63%, averaging around 50% shooting efficiency. Players scoring less than 10 PPG showed a wide range of efficiency from 0-100%.

- Pearson correlation coefficient (r): ≈ -0.762
- R² (coefficient of determination): ≈ 0.580

This indicates a moderate to strong negative correlation between FG% and points per game, which suggests that players who take more shots (and score more) tend to be less efficient, while role players have higher FG% but fewer points.

**Implication:** Coaches should consider this trade-off when allocating shot opportunities, balancing volume and efficiency to optimize team scoring.

---

## Question 4: Relationship Between 2-Point and 3-Point Shot Percentage

![2P% and 3P% vs Points](visuals/2p_vs_3p_percentage.png)

This graph compares 2-point percentage (light blue) and 3-point percentage (dark blue) across points per game:

- 2P% fluctuates mostly between 45% and 60%, showing less volatility.
- 3P% ranges mostly from 25% to 40%, typically lower than 2P%.
- Low scorers (<10 PPG) have very volatile 3P% values.
- High scorers (>20 PPG) show slightly declining 2P% and stable but lower 3P%.

**Implication:** High-volume scorers tend to take more difficult or longer shots (3-pointers), which impacts their efficiency. Coaches can use this to assess shot selection strategy and player roles.

---

## Files Included

- `capstone.pbix`: Power BI file containing the detailed visualizations and analysis.
- `notebooks/`: Jupyter notebooks or Python scripts used for data cleaning and analysis.
- `data/`: Dataset files (or links to datasets if too large).
- `visuals/`: Exported images of charts and graphs used in this report.

---

## Links to External Resources

- [Google Sheet with Analysis](https://docs.google.com/spreadsheets/d/1s_1s5N6vpHy79Hd70US4o7F6JOCmXB5Xwn0WyZvVMfg/edit?usp=sharing)
- [Kaggle Dataset - 2023-2024 NBA Player Stats](https://www.kaggle.com/datasets/vivovinco/2023-2024-nba-player-stats)

---



---

## Conclusion

This project provides actionable insights into key factors affecting NBA player scoring and efficiency during the 2023-2024 playoffs. By understanding relationships between minutes played, age, efficiency, and shot types, NBA decision-makers can better optimize player utilization and lineup strategies to increase their chances of winning.

---

