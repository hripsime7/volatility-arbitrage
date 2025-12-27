# Volatility Arbitrage Strategy

This project explores a basic volatility arbitrage approach by comparing
realized volatility derived from historical price data with market-implied
volatility proxies.

The goal is to identify periods of volatility mispricing and analyze
their statistical properties.

## Motivation

This project was built as a portfolio piece for junior quantitative finance
and trading roles. It focuses on clarity, correctness, and financial
intuition rather than production deployment.

## Methodology

- Download historical price data using `yfinance`
- Compute log returns
- Estimate realized volatility over rolling windows
- Measure volatility mispricing
- Analyze summary statistics and visualizations

## Tools and Libraries

- Python
- NumPy
- pandas
- matplotlib
- yfinance

## Structure

- `volatility_arbitrage.ipynb`  
  Main notebook containing data collection, calculations, and analysis

- `README.md`  
  Project overview and methodology

## Notes

This implementation is for educational and research purposes only.
It does not constitute financial advice or a tradable strategy.

## Possible Extensions

- Multi-asset volatility comparison
- Options-based implied volatility integration
- Options Greeks analysis (Delta, Gamma, Vega)
- Backtesting with PnL simulation
- Risk-adjusted performance metrics

---

Author: Hripsime

