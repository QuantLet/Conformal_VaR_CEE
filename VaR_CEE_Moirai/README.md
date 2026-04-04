<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_Moirai

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Generates zero-shot VaR and ES forecasts using the Moirai foundation model (Salesforce). Produces 1000 Monte Carlo forecast samples per date using a 512-day context window via the uni2ts/GluonTS interface and derives VaR/ES from the empirical distribution of samples.

Keywords: Moirai, foundation model, zero-shot forecasting, Value-at-Risk, Expected Shortfall, uni2ts, GluonTS, probabilistic forecasting

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/processed/{country}_returns.parquet

Input: Log return series, 512-day context window, 1000 samples per forecast, VaR levels (1%, 2.5%, 5%)

Output: CSV files with daily VaR and ES forecasts per series in data/var_forecasts/

Example: Loads Moirai-1.1-R-small, generates 1000 samples for EURPLN_ret, computes VaR at 2.5%

```
