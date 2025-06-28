# portfolio-optimization-using-MPT-BLM
# 📈 Portfolio Optimization using Modern Portfolio Theory and Black-Litterman Model

This project implements a robust and practical portfolio optimization pipeline using both **Modern Portfolio Theory (MPT)** and the **Black-Litterman Model (BLM)**. It integrates quantitative finance, optimization, and data science to construct an optimal portfolio from 30 Indian equity stocks.

---

## 🚀 Project Highlights

- ✅ **Optimized a 30-stock portfolio** using MPT and BLM to improve risk-adjusted returns.
- 📉 Achieved **21.6% annual return** with a **Sharpe Ratio of 1.48**, outperforming both the benchmark (S&P 500) and equal-weight portfolios.
- 🧠 **Market-implied returns + quantitative investor views** using 6-month relative momentum.
- 📊 Constructed and visualized the **Efficient Frontier**, **Capital Market Line**, and **Backtest Performance** vs baseline strategies.

---

## 📌 Methodology

### 1. Data Preprocessing
- Cleaned and aligned historical price data for 30 stocks
- Computed daily returns and sampled covariance matrix

### 2. Return Estimation
- Used `pypfopt` to compute **mean historical returns**
- Applied **market-implied prior** returns using Black-Litterman model

### 3. View Generation
- Automatically generated **weak quantitative views** using 6-month return momentum (top vs bottom stocks)
- Modeled view uncertainty using **Idzorek's method**

### 4. Optimization
- Ran **Efficient Frontier optimization** to maximize Sharpe Ratio
- Visualized **Efficient Frontier**, **Capital Market Line**, and max Sharpe portfolio

### 5. Backtesting
- Compared optimized portfolio against equal-weight and S&P 500 index
- Tracked **cumulative returns, volatility**, and **Sharpe ratios**

---

## 📊 Results

| Strategy              | Annual Return | Volatility | Sharpe Ratio |
|-----------------------|---------------|------------|--------------|
| Optimized Portfolio   | **21.6%**     | 13.4%      | **1.48**     |
| Equal-Weighted        | 15.2%         | 15.6%      | 0.84         |
| S&P 500 (Benchmark)   | 16.1%         | 17.2%      | 0.81         |

---

## 📁 Project Structure

