# 🏀 NBA Stats Capstone Project: Data-Driven Insights from the Court

## 📌 Project Overview

This capstone project explores professional basketball trends using NBA datasets to uncover insights into team performance, player efficiency, and playoff outcomes. The goal is to showcase my skills in data cleaning, analysis, visualization, and storytelling using Power BI and Python.

**Dataset Source:** [NBA Stats from Kaggle](https://www.kaggle.com/datasets)  
**Tools Used:** Power BI, Python, Pandas, Matplotlib, Power Query  
**Repository Contents:**
- 📁 `data/`: Cleaned and raw datasets
- 📁 `visualizations/`: Screenshots of Power BI dashboards
- 📄 `NBA_Capstone.pbix`: Power BI project file
- 📄 `README.md`: This report

---

## 🎯 Problem Statement

In an era where sports franchises are increasingly driven by data, the ability to analyze performance metrics is critical to understanding what leads to victory. This project addresses several business questions:

1. What statistical categories most strongly correlate with team success in the regular season and playoffs?
2. How do player performance metrics differ between the regular season and the playoffs?
3. What trends can be observed in team efficiency and win rates over the past two decades?

The goal is to provide actionable insights that could theoretically help coaches, analysts, or sports fans interpret what drives NBA team success.

---

## 🧹 Data Cleaning

Three primary datasets were used:
- `Regular.csv` – Player stats for the 2023–24 regular season
- `Playoffs.csv` – Player stats for the 2023–24 playoffs
- `WL_playoff_total.csv`, `pergame_stats_total.csv`, and `advanced_stats_total.csv` – Team performance data from 2000–2023

**Cleaning Steps:**
- Removed nulls and duplicate rows
- Standardized column names (e.g., `FG%`, `3P%`, etc.)
- Filtered out players with minimal minutes played to focus on key contributors
- Merged datasets where necessary (e.g., team stats with playoff win/loss data)
- Created calculated columns in Power BI (e.g., `True Shooting %`, `Offensive Rating`)
- Verified consistency in player/team names across datasets

All transformations were documented within Power Query for reproducibility.

---

## 📊 Exploratory and Final Analysis

### Key Analytical Techniques:
- **Trend Analysis:** Team win rates and offensive/defensive efficiencies from 2000–2023
- **Comparative Analysis:** Regular season vs. playoff stats for top 50 players by minutes
- **Correlation Analysis:** Offensive metrics vs. team win percentage
- **Advanced Metrics:** Used PER, TS%, eFG%, and advanced team ratings

### Key Insights:
- **Regular Season vs. Playoffs:** On average, scoring efficiency (TS%) decreases in the playoffs due to tighter defense.
- **Team Success:** Strong positive correlation between `Offensive Rating` and `Win%` (r ≈ 0.75).
- **Championship Trends:** Teams that won titles consistently ranked top 5 in both `Net Rating` and `Assist %`.
- **Evolution Over Time:** The average `3P Attempt Rate` has tripled since 2000, drastically changing play style.

Visualizations in Power BI highlighted these findings through interactive dashboards including slicers, bar charts, scatterplots, and heatmaps.

---

## 📈 Visualizations

Key visuals included in the Power BI report:
- **Player Efficiency Comparison**: Heatmap comparing regular season and playoff performance
- **Team Trends Dashboard**: Time-series visual of team ratings and win percentages
- **Correlation Matrix**: Visual representation of which metrics best predict playoff success
- **Champion Profile**: Aggregated stats of past NBA champions

See the `/visualizations/` folder for static examples of these dashboards.

---

## 🧠 Conclusion

The data analysis revealed that while individual scoring is important, team success relies more on efficient ball movement, strong defense, and shooting consistency. The growing influence of 3-point shooting continues to reshape the NBA landscape.

This project demonstrates how data analytics can illuminate key insights that might otherwise go unnoticed. If expanded, the next phase might involve:
- Incorporating player tracking or shot location data
- Predictive modeling for future playoff success
- Natural Language Processing to analyze commentary or player sentiment

---

## 🧰 How to Use This Repository

1. Clone the repository or download it as a ZIP.
2. Open `NBA_Capstone.pbix` in Power BI Desktop to explore dashboards.
3. Review the `/data/` folder for CSV files.
4. View dashboards in the `/visualizations/` folder if Power BI is not installed.

---

## 📂 Files & Structure

