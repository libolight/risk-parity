# risk-parity
Risk parity weight calculations and return profiles

Dependencies: pandas, numpy, matplotlib, seaborn, pylab, tqdm, scipy, sklearn

Use provided Excel file ("returns_data.xlsx") or provide your own. The file calculates optimized portfolio weights for risk parity portfolios using the following algorithms: 1) minimum variance, 2) naive risk parity (inverse realized volatility), 3) equal risk contribution or "ERC," 4) inverse beta, 5) max diversification, and 6) Marcos Lopez de Prado's hierarchical risk parity (de Prado's code is used for this algorithm only--all other code mine). 

# UGAZ_short

'UGAZ_short.ipynb' investigates volatility decay on four leveraged ETFs tracking already volatile underlying commodities. UGAZ is a 3x levered ETF that aims to track each day's percentage change in constant one-month forward natural gas futures. The underlying index has declined 25% annually since inception, and is uncorrelated with other core components of the risk parity portfolio highlighted in 'Risk parity weights.ipynb'. 

This analysis uses a kernel density estimator with a Gaussian kernel to simulate 10,000 252-day trials shorting UGAZ. The expected median return from a one-year short position is ~80% and the median expected maximum drawdown of the strategy is 45%. 

Other ETFs profiled are UWTIF (3x long WTI oil), UGLD (3x long gold), and UVXY (2x long VIX futures). 

Excel files with daily return histories for each are provided here. 

Dependencies: pandas, numpy, scipy, statsmodels, tqdm, matplotlib, pylab


