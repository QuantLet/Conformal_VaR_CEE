<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: VaR_CEE_Figures

Published in: Can Foundation Models Manage Risk? Zero-Shot VaR and ES Forecasting for CEE Markets

Description: Generates all six publication-quality figures: VaR breach plots, violation rate comparison, Basel traffic light dashboard heatmap, ES adequacy bar chart, Kupiec p-value heatmap, and cross-country model ranking. All figures use transparent backgrounds and legends positioned outside the plot area.

Keywords: data visualization, matplotlib, VaR breach plot, traffic light dashboard, heatmap, model comparison, publication figures

Author: Daniel Traian Pele

Submitted: 2025

Datafile: data/var_forecasts/*.csv, data/backtesting/backtesting_results.csv

Input: VaR forecast files and backtesting results for all models and series

Output: Six figures (PNG and PDF) saved in data/figures/: fig1_var_breach, fig2_violation_rates, fig3_traffic_light, fig4_es_adequacy, fig5_kupiec_heatmap, fig6_model_ranking

Example: Creates a 3x2 panel of VaR breach plots comparing GJR-GARCH vs TimesFM-2.5-Conf for five CEE stock indices

```
