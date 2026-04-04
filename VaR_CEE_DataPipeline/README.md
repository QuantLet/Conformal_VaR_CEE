<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_DataPipeline

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Computes log returns from raw price data and produces descriptive statistics including mean, standard deviation, skewness, kurtosis, Jarque-Bera, ADF, and ARCH-LM tests for all CEE market series.

Keywords: log returns, descriptive statistics, Jarque-Bera test, ADF test, ARCH-LM test, data pipeline, CEE markets

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/raw/BET.csv, data/raw/WIG20.csv, data/raw/PX.csv, data/raw/BUX.csv, data/raw/SOFIX.csv, and corresponding FX CSV files

Input: Raw CSV price files for stock indices and FX rates

Output: Parquet files with log returns per country in data/processed/, descriptive statistics CSV in data/stats/

Example: Computes log returns for BET index and EUR/RON, saves Romania_returns.parquet and descriptive_stats.csv

```
