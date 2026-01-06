# AAPL Options Dashboard – Black-Scholes Pricing & Greeks Analysis

## Project Overview

This project demonstrates real-world **quantitative finance analysis** using Python.  
It pulls **real AAPL stock and option chain data** from Yahoo Finance, prices European call and put options using the **Black-Scholes model**, computes all main **option Greeks**, and visualizes key metrics.

The project is designed to be **interactive and portfolio-ready**, showing both your programming and financial modeling skills.

---

## Key Features

1. **Real Market Data**
   - Pulls current AAPL stock price.
   - Retrieves the nearest AAPL option chain (calls and puts) with strike prices and market prices.

2. **Option Pricing**
   - Implements the **Black-Scholes formula** for European call and put options.
   - Computes option prices for all strikes in the selected expiration.

3. **Greeks Calculation**
   - Computes all major Greeks for each option:
     - **Delta**: Sensitivity to stock price changes
     - **Gamma**: Rate of change of Delta
     - **Vega**: Sensitivity to volatility
     - **Theta**: Time decay
     - **Rho**: Sensitivity to interest rates

4. **Visualizations**
   - **Market vs Black-Scholes Prices**
   - **Greeks vs Strike Price** for calls and puts
   - **Interactive exploration** of option prices by adjusting volatility and time to expiration using sliders

5. **Interactive Dashboard**
   - Adjust volatility or days to expiration to instantly update pricing visualization.
   - Helps visualize how option prices respond to market factors — an essential skill in quantitative finance.

---

## Technology Stack

- **Python** – core programming
- **yfinance** – fetch real stock and option chain data
- **numpy & pandas** – numerical calculations and data manipulation
- **scipy.stats.norm** – normal distribution for Black-Scholes
- **matplotlib** – data visualization
- **ipywidgets** – interactive sliders for live scenario analysis

---

## How to Run

1. Open the notebook in **Google Colab** (recommended) or Jupyter Notebook.
2. Install required packages (Colab will handle this automatically with `!pip install yfinance ipywidgets`).
3. Run all cells **top-to-bottom**.
4. Interact with sliders to explore **volatility** and **time-to-expiry** effects on AAPL options.

---

## Insights

- **Delta**: Increases as stock price rises for calls; decreases for puts.
- **Gamma**: Highest near the strike price, indicating the most sensitivity to stock price changes.
- **Vega**: Peaks at-the-money — volatility has the largest impact on option prices for ATM options.
- **Theta**: Negative, showing the daily time decay of options, more pronounced for short-term options.
- **Rho**: Small for short-dated options; more important for long-term options.

- Market prices may differ slightly from Black-Scholes prices due to supply-demand, dividends, or market inefficiencies, which is realistic in actual trading environments.

---

## Portfolio Value

This project showcases:

- **Quantitative Finance Knowledge**: Option pricing, Black-Scholes, Greeks
- **Python Programming**: Data handling, visualization, interactive widgets
- **Data Analysis & Visualization**: Real market comparison, Greeks plots
- **Portfolio Readiness**: Clean, documented, professional notebook suitable for GitHub

---

## Optional Extensions

- Pull **multiple expiration dates** and analyze across maturities
- Compute **implied volatility** from market prices
- Monte Carlo simulation for option pricing under different scenarios
- Include **other tickers** to expand portfolio examples
