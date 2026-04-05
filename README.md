# Bayer-Equity-Analysis
Time-series analysis of Bayer AG stock returns against the DAX (DE40) index using the Capital Asset Pricing Model (CAPM). Built as part of a broader equity valuation of Bayer AG for an investor recommendation.
Key Findings

Beta: 0.82 — Bayer moves directionally with the DAX but at ~82% of the magnitude
R²: 0.13 — Only 13% of Bayer's return variation is explained by market movements; the remaining 87% is driven by firm-specific risk (litigation, restructuring, pharma pipeline)
Alpha: -0.007 — Slight underperformance vs CAPM prediction, not statistically significant (p = 0.55)
Cumulative return: €100 invested in Bayer in May 2021 → ~€74 by April 2026, vs ~€153 for the DAX

Methodology

Monthly closing prices for BAYGN, DAX, and the German 10-year bond yield (April 2021 – April 2026)
Simple return computation and excess return calculation using the German 10Y yield as risk-free rate
OLS regression of Bayer excess returns on DAX excess returns (CAPM single-factor model)

Tech
Python · pandas · NumPy · matplotlib · statsmodels · scipy
Data
Monthly historical data sourced from Investing.com. 60 observations (May 2021 – April 2026).
