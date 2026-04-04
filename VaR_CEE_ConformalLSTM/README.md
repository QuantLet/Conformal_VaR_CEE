<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_ConformalLSTM

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Implements LSTM neural network with conformal prediction for VaR and ES forecasting. Uses a 60-day lookback window, 64 hidden units, retrained every 21 days on a rolling 250-day window. Conformal residuals calibrate the prediction intervals.

Keywords: LSTM, neural network, conformal prediction, deep learning, Value-at-Risk, Expected Shortfall, PyTorch, rolling window

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/processed/{country}_returns.parquet

Input: Log return series, rolling window of 250 days, lookback of 60 days, VaR levels (1%, 2.5%, 5%)

Output: CSV files with daily VaR and ES forecasts per series in data/var_forecasts/

Example: Trains LSTM on BUX_ret rolling window, computes conformal residuals, forecasts 1-day VaR at 1%

```
