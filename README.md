# Portfolio Optimization with Community Detection and GPU-Accelerated Analysis

## Project Overview
This repository contains a comprehensive data analysis pipeline for stock portfolio optimization using community detection algorithms and volatility-based metrics. The implementation leverages GPU acceleration through CUDA for high-performance processing of large financial datasets to rapidly identify market structures and investment opportunities.

The project demonstrates how network science techniques can reveal hidden relationships between individual stocks in financial markets. This is particularly useful at a time of high trade tensions, high volatility expectations, and geopolitical upheaval. I explain how these concepts can provide financial professionals with powerful tools to construct diversified portfolios, manage risk, and identify market opportunities that might be missed by traditional sector-based approaches.

## Contents
- `mod-opt/eda_modularity_opt_cuda.ipynb`: Initial data exploration and preprocessing notebook
- `mod-opt/Analysis_Modularity_Opt_CUDA.ipynb`: Core analysis implementing community detection algorithms and portfolio optimization

## Key Features

### Community Detection Approach
- Transformation of stock correlations into network representations
- Implementation of multiple community detection algorithms (Spectral Clustering, Modularity Optimization, Leiden Algorithm)
- Identification of natural stock clusters based on volatility relationships
- GPU acceleration for processing 400+ million data points efficiently

### Volatility Analysis
- Community-level volatility metrics revealing market structure
- Volatility variance analysis for identifying internal community stability
- Volatility change tracking for early detection of market regime shifts
- Transition analysis between communities over time

### "Drill Down" Capabilities
- Aggregate community metrics for macro-level market analysis
- Stock movement tracking across communities
- Volatility-based filtering for rapid identification of risk concentrations
- Time-series analysis of community stability and change

## Notebook Details

The `Analysis_Modularity_Opt_CUDA.ipynb` notebook contains the implementation of our community detection approach to portfolio optimization. In this notebook, you'll find:

1. Construction of volatility-weighted networks from stock time series data
2. Implementation and comparison of three community detection algorithms
3. Visualization of community structures and transitions over time
4. Analysis of community-level volatility metrics and their implications for portfolio construction
5. Demonstration of "drill down" capabilities for financial decision-making
6. GPU-accelerated computation enabling real-time analysis of complex market structures

This notebook builds upon the exploratory data analysis from Part 1 (`eda_modularity_opt_cuda.ipynb`) and transforms the engineered features into actionable investment insights through the application of network science to aid human and algorithmic decision making. The approach is particularly valuable in today's high-volatility market environment where risk concentrations and potential opportunities emerge uniquely across market segments.

## Technologies
- CUDA: GPU acceleration for network analysis
- Polars: High-performance DataFrame operations
- NetworkX/CDLib: Community detection algorithms
- Python data visualization tools

This repository demonstrates how advanced network analysis techniques can transform financial data analysis during periods of market uncertainty. GPU acceleration techniques make the software side of realizing this project entirely feasible, and this particular implementation enables real-time analysis of complex network structures that would be computationally prohibitive with traditional processing methods.

By revealing underlying community structures that traditional sector-based or factor-based aggregations often miss. This approach provides a more high-level understanding of market dynamics and still allows very granular drill down. The interplay between volatility and stability across different stock communities offers superior diversification opportunities when market correlations shift unexpectedly. This combination of network science and high-performance computing empowers financial professionals to construct more resilient portfolios regardless of prevailing market conditions.

