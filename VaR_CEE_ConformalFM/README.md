<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_ConformalFM

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Applies rolling conformal calibration on top of raw foundation model VaR forecasts. For each date, computes conformal scores from the calibration window and adjusts the VaR forecast by the empirical quantile of these scores. Also recalibrates ES using tail returns below the adjusted VaR.

Keywords: conformal prediction, calibration, foundation model, Value-at-Risk, Expected Shortfall, distribution-free, post-hoc correction

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/var_forecasts/Chronos-2_*.csv, data/var_forecasts/TimesFM-2.5_*.csv, data/var_forecasts/Moirai-2.0_*.csv

Input: Raw foundation model VaR forecasts, rolling calibration window of 250 days

Output: Conformally-adjusted VaR/ES forecasts saved as {Model}-Conf_{series}.csv in data/var_forecasts/

Example: Reads Chronos-2_BET_ret.csv, applies 250-day rolling conformal correction, saves Chronos-2-Conf_BET_ret.csv

```
