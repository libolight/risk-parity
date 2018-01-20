# risk-parity
Risk parity weight calculations and return profiles

Dependencies:
pandas, 
numpy, 
matplotlib, 
seaborn, 
pylab, 
tqdm, 
scipy, 
sklearn


Use provided Excel file ("returns_data.xlsx") or provide your own. The file calculates optimized portfolio weights for risk parity portfolios using the following algorithms: 1) minimum variance, 2) naive risk parity (inverse realized volatility), 3) equal risk contribution or "ERC," 4) inverse beta, 5) max diversification, and 6) Marcos Lopez de Prado's hierarchical risk parity (de Prado's code is used for this algorithm only--all other code mine). 

