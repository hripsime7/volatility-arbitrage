# Volatility Arbitrage Project

This repository contains a Python/Jupyter Notebook project that explores **volatility arbitrage** opportunities in equity options using the Black–Scholes model and market data from Yahoo Finance.

The notebook downloads historical price data, estimates volatility, compares it with implied volatility, and highlights potential mispricings that could be used in a volatility arbitrage strategy.

---

## Overview

Volatility arbitrage is based on the idea that **implied volatility** (what the options market expects) can deviate from **realized/historical volatility** (what the underlying actually does). When these differ significantly, traders may construct delta‑neutral strategies to profit from the convergence.

This project:

* Implements the **Black–Scholes model** for option pricing
* Fetches real market data using `yfinance`
* Estimates volatility from historical returns
* Compares theoretical option prices with market expectations
* Flags potential arbitrage opportunities

---

## Key Components

### 1. Black–Scholes Model

A custom `BlackScholes` class is implemented to price European call and put options:

* Call price
* Put price
* Handles dividends, interest rates, and edge cases

### 2. Market Data

* Stock price data is downloaded via **Yahoo Finance**
* Daily returns are computed
* Annualized historical volatility is estimated

### 3. Volatility Analysis

* Historical volatility vs. assumed/implied volatility
* Identification of volatility mispricing
* Output of potential arbitrage signals

### 4. Automation

* Multiple tickers can be analyzed in one run
* Results are aggregated for comparison

---

## Project Structure

```
volatility_arbitrage.ipynb   # Main analysis notebook
README.md                   # Project documentation
```

---

## Requirements

Install the required Python packages:

```bash
pip install numpy pandas matplotlib scipy yfinance
```

Python version: **3.9+** recommended

---

## How to Run

1. Clone this repository
2. Install dependencies
3. Open the notebook:

```bash
jupyter notebook volatility_arbitrage.ipynb
```

4. Run all cells to perform the analysis

---

## Output

The notebook produces:

* Option price estimates (call & put)
* Volatility comparisons
* Console output highlighting potential arbitrage opportunities
* (Optional) plots for price and volatility behavior

---

## Disclaimer

This project is **for educational and research purposes only**.
It does **not** constitute financial advice or a trading recommendation.
Real-world volatility arbitrage involves transaction costs, liquidity constraints, model risk, and execution risk that are **not** fully captured here.

---

## Possible Extensions

* Use real implied volatility from option chains
* Add Greeks (Delta, Vega, Gamma)
* Implement delta‑neutral strategies
* Backtest performance
* Include transaction costs and slippage

---

## Author

Created as a learning project in quantitative finance and derivatives pricing.
Hripsime
