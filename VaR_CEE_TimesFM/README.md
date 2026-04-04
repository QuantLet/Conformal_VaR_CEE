<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_TimesFM

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Generates zero-shot VaR and ES forecasts using Google TimesFM 2.5 foundation model. Fits a Student-t distribution to the model's output quantiles via quantile matching optimization and derives VaR/ES from the fitted parametric distribution.

Keywords: TimesFM, foundation model, zero-shot forecasting, Value-at-Risk, Expected Shortfall, Student-t distribution, quantile matching, time series

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/processed/{country}_returns.parquet

Input: Log return series, 512-day context window, VaR levels (1%, 2.5%, 5%)

Output: CSV files with daily VaR and ES forecasts per series in data/var_forecasts/

Example: Loads TimesFM-2.5-200M, forecasts quantiles for BET_ret, fits Student-t and computes VaR at 1%

```
