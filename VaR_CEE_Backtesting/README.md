<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_Backtesting

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Performs comprehensive VaR and ES backtesting using Kupiec unconditional coverage test, Christoffersen conditional coverage test, Acerbi-Szekely Z2 test for ES, and Basel traffic light classification. Evaluates all 10 models across all CEE series.

Keywords: backtesting, Kupiec test, Christoffersen test, Acerbi-Szekely test, Basel traffic light, Value-at-Risk, Expected Shortfall, model validation

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/var_forecasts/*.csv

Input: VaR and ES forecast CSV files for all models and series, VaR levels (1%, 2.5%, 5%)

Output: backtesting_results.csv, traffic_light_dashboard.csv, green_rate_by_model.csv in data/backtesting/

Example: Runs Kupiec test on GJR-GARCH VaR 1% for BET_ret, classifies as Green/Yellow/Red under Basel rules

```
