# Fund Performance Evaluation
This repository will introduce analyze the performance of a multi-asset fund, UPAMC All Weather-A fund (0P00006AC3.TW), improve its risk-return profile by hedging the exposure to equity market risk using options, and evaluate its sensitivity to a number of risk factors.

> Data: Data for all instruments and indices below can be downloaded from Yahoo Finance (ticker in parenthesis). Consider monthly data frequency for the analysis and simulations.

3 steps are as follows:
- Provide the statistics for the fund since inception: annualized return and volatility, Sharpe ratio, max. drawdown, correlation and beta to S&P 500.
- Backtest a long put option hedge for the strategy in the previous point, aiming at reducing the beta of the hedged strategy to S&P 500 by 50%. In order to do that, simulate rolling monthly an OTM put for protection. The parameters to be chosen are: i) moneyness of OTM put (95%, 90%, etc.), and ii) option expiry (1 month, 3 months, etc.). Compare Sharpe ratio and max. drawdown of hedged and unhedged strategies.
- Using regression modeling, evaluate the sensitivity (beta) of the hedged strategy returns to the following market risk factors: gold (GLD), oil (USO), commodities (DBC), real estate (VNQ), US equities (SPY), world equities (VEU), emerging markets (EEM), volatility (^VIX), US 10 year interest rates (^TNX), US dollar (UUP).
