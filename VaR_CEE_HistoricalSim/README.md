<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_HistoricalSim

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Implements rolling 250-day Historical Simulation for VaR and ES forecasting. VaR is computed as the empirical quantile of the rolling window, and ES as the mean of returns below the VaR threshold.

Keywords: historical simulation, Value-at-Risk, Expected Shortfall, rolling window, non-parametric, risk management

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/processed/{country}_returns.parquet

Input: Log return series, rolling window of 250 days, VaR levels (1%, 2.5%, 5%), out-of-sample start date

Output: CSV files with daily VaR and ES forecasts per series in data/var_forecasts/

Example: Computes 1-day VaR at 1% for BET_ret using a rolling 250-day historical window

```
