# Regression Toward the Mean: Portfolio Backtesting Dataset

This repository contains the dataset used in the blog post:
**[Regression Toward the Mean: Lessons from 35 Years of Portfolio Backtesting](https://complexity-thinking.blogspot.com/2025/11/regression-toward-mean-lessons-from-35.html)**

**You can also view the [Tableau Dashboard](https://public.tableau.com/app/profile/complexity.thinking/viz/Cap-WeightedvsEqual-WeightedIndexPerformance/Dashboard-WeightStrategies) for the results.**

The dataset tracks the performance of different S&P 500 weighting strategies from 1990 to end of 2024, highlighting how regression toward the mean shapes long‑term returns and the impact of avoiding major market crashes.

---

## 📊 Dataset Overview
The dataset includes simulated portfolio results for:
- **Benchmark:** Full S&P 500 index (market‑cap weighted)
- **Top 20 Market‑Cap Weighted**
- **Top 10 Equal‑Weighted**
- **Top 11–20 Equal‑Weighted**
- **Top 20 Equal‑Weighted**

Each portfolio is:
- Constructed annually on the first trading day using prior year’s final market capitalization
- Rebalanced every January
- Based on historical data from **Yahoo Finance** and **FinHacker**

---

## 📂 Repository Contents
- `data/prices` → CSV files of S&P 500 index and individual stock prices
- `data/results` → Portfolio backtesting result
- `SP500_Yearly_Top20_Since_1990.csv` → Each year's top 20 companies of S&P 500 from FinHacker.


⚠️ Notice: In the original FinHacker dataset, market capitalization values are reported at the end of each year.
For this backtest, those year‑end market caps are used as the starting allocations for the following year, since rankings and relative sizes typically change very little between year‑end and the first trading day of the next year, especially for top companies.

---

## 🔎 Key Insights
- **Regression Toward the Mean:** Market leaders regress, mid‑tier stocks often outperform in subsequent cycles.
- **Equal vs. Market‑Cap Weighting:** Equal‑weight portfolios reduce concentration risk and capture mean reversion.
- **Timing Crashes:** Avoiding major downturns (dot‑com, 2008, COVID) can double long‑term returns.
- **Unique Finding:** The **Top 11–20 Equal‑Weight strategy** was the only one to reach a new all‑time high before the Great Recession.

---

## 📖 References
- Joel Greenblatt, *The Big Secret for the Small Investor* (2011) — Chapter 7 explores equal‑weight vs. market‑cap strategies.
- “The Real Dogs of the Dow” — Study showing deletions from the Dow often outperform additions.
- Bespoke Investment Group, *S&P Equal Weight vs. Cap Weight* (2024).
- Blog post: [Regression Toward the Mean: Lessons from 35 Years of Portfolio Backtesting](https://complexity-thinking.blogspot.com/2025/11/regression-toward-mean-lessons-from-35.html)

---

