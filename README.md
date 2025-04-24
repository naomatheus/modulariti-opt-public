# Portfolio Optimization with Modularity and VWAP Analysis

## Project Overview
This repository contains a data analysis pipeline for stock portfolio optimization using multiple price-volume metrics and risk calculations, implemented in Polars for high-performance data processing.

## Contents
- `mod-opt/eda.ipynb`: Initial data exploration and preprocessing notebook containing:
  - Multiple price and volume metrics calculations
  - Risk analysis computations
  - Data cleaning and preparation for modularity analysis

## Key Metrics & Formulas

### Price Metrics
1. Price Change Percentage (PCP):
```math
PCP = \left( \frac{Close - Open}{Open} \right) \times 100
```

2. Volume-Weighted Average Price (VWAP):
```math
VWAP = \frac{\sum (Price_i \times Volume_i)}{\sum Volume_i}
```

3. Time-Weighted Average Price (TWAP):
```math
TWAP = \frac{\sum Price_i}{n}
```

### Risk Metrics
1. Daily Volatility:
```math
Volatility_{daily} = \frac{High - Low}{Open} \times 100
```

2. Sharpe Ratio:
```math
Sharpe = \frac{R_p - R_f}{\sigma_p}
```
Where:
- R_p = Portfolio Return
- R_f = Risk-free Rate
- σ_p = Portfolio Standard Deviation

## Data Processing Features
- Zero-volume day handling with stock-specific average volume
- Null value removal for clean data
- Data preparation for modularity optimization

## Technologies
- Polars: High-performance DataFrame operations
- Python data analysis tools
- Google Colab integration

## Next Steps
The processed and engineered features will be used in subsequent modularity optimization analysis to identify natural stock clusters for portfolio diversification.

This repository represents the initial data processing and feature engineering phase of a larger portfolio optimization project using community detection algorithms.
