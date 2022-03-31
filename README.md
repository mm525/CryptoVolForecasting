# ETH Volatility Forecasting
Aim: select the best model for forecasting the realised volatility of Ethereum's native cryptocurrency, Ether.

## Rough Outline of Project
1) Gain Ether's price history (either by downloading an Excel file and reading the data into Jupyter, or via an API)
2) Clean the data (hard to imagine there will be outliers, so mainly on the look out for missing values)
3) Calculate Ether's ln returns
4) Calculate Ether's daily realised volatility (requires selection of a suitable frequency by which to scale volatility - trade-off between too much and too little noise (i.e. basically a moving average))
5) For the various (G)ARCH form models, select the best instance of each (e.g. via inspection of ACF and PACF) and then the best overall model
6) There is reason to believe that EGARCH might be quite good (greater impact of negative shocks seems to accurately reflect the asymmetric market reaction to negative vs positive news)
