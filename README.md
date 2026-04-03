# Conformal_VaR_CEE

## Can Foundation Models Manage Risk? Zero-Shot Value-at-Risk and Expected Shortfall Forecasting for Central and Eastern European Markets

**Authors:** Daniel Traian Pele, Rahul Tak, Ștefan Găman, Siang-Li Jheng, Miruna Mazurencu-Marinescu-Pele

**Submitted to:** Romanian Journal of Economic Forecasting

---

### Abstract

We evaluate whether zero-shot time series foundation models (TSFMs) can produce regulatory-adequate Value-at-Risk (VaR) and Expected Shortfall (ES) forecasts for Central and Eastern European financial markets. Testing Chronos-2, TimesFM 2.5, and Moirai 2.0 against GJR-GARCH, Historical Simulation, and conformal-calibrated ARIMA/LSTM baselines across five CEE countries (Romania, Poland, Czechia, Hungary, Bulgaria), we find that TimesFM 2.5 achieves the lowest violation rate (1.43%) while Chronos-2 fails catastrophically (37%) due to predictive distribution compression. Conformal recalibration restores Chronos-2 to regulatory adequacy but can degrade already well-calibrated models.

### Quantlets

| Quantlet | Description |
|----------|-------------|
| [VaR_CEE_DataDownload](VaR_CEE_DataDownload/) | Downloads CEE stock index and FX data from Stooq and Yahoo Finance |
| [VaR_CEE_DataPipeline](VaR_CEE_DataPipeline/) | Computes log returns and descriptive statistics |
| [VaR_CEE_HistoricalSim](VaR_CEE_HistoricalSim/) | Rolling 250-day Historical Simulation for VaR/ES |
| [VaR_CEE_GJRGARCH](VaR_CEE_GJRGARCH/) | GJR-GARCH(1,1) with skewed-t distribution |
| [VaR_CEE_ConformalARIMA](VaR_CEE_ConformalARIMA/) | ARIMA + conformal prediction for VaR/ES |
| [VaR_CEE_ConformalLSTM](VaR_CEE_ConformalLSTM/) | LSTM + conformal prediction for VaR/ES |
| [VaR_CEE_Chronos](VaR_CEE_Chronos/) | Chronos-2 zero-shot VaR/ES (1000 samples, 512 context) |
| [VaR_CEE_TimesFM](VaR_CEE_TimesFM/) | TimesFM 2.5 zero-shot VaR/ES via quantile matching |
| [VaR_CEE_Moirai](VaR_CEE_Moirai/) | Moirai 2.0 zero-shot VaR/ES (1000 samples, 512 context) |
| [VaR_CEE_ConformalFM](VaR_CEE_ConformalFM/) | Conformal recalibration of foundation model forecasts |
| [VaR_CEE_Backtesting](VaR_CEE_Backtesting/) | Kupiec, Christoffersen, Acerbi-Szekely, Basel traffic light |
| [VaR_CEE_Figures](VaR_CEE_Figures/) | Publication-quality figures |

### Configuration

All quantlets share `config.py`:
- 5 CEE markets: Romania (BET), Poland (WIG20), Czechia (PX), Hungary (BUX), Bulgaria (SOFIX)
- 10 return series: 5 stock indices + 5 exchange rates
- OOS period: 2018-01-01 to 2025-12-31
- FM parameters: 1000 samples, 512 context, stride 1
- VaR levels: 1%, 2.5%, 5%

### Keywords

Value-at-Risk, Expected Shortfall, foundation models, zero-shot forecasting, emerging markets, CEE, conformal prediction, Basel backtesting

### JEL Classification

C45, C53, C58, G17, G32
