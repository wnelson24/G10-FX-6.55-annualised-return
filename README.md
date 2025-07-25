Overview
Type: Currency Carry
Asset(s): G10 Forex Pairs
Timeframe: Daily
Style: Monthly rotation, market-neutral
This strategy ranks major G10 currency pairs by their interest rate differentials. Each month, it goes long the top 3 carry pairs and short the bottom 3, aiming to capture the yield spread while maintaining a market-neutral stance. Positions are rebalanced monthly at the start of each month.

Parameters
Universe: G10 currency pairs
Rebalance Frequency: Monthly (start of month)
Top/Bottom Selection: Long top 3, short bottom 3 by carry
Leverage: 8x gross exposure
Interest Rate Source: Hardcoded central bank estimates
Strategy Logic
Signal Generation
At the start of each month, calculate interest rate differential for each currency pair:
Carry = Base Currency Rate - Quote Currency Rate
Rank all pairs by carry
Select top 3 for long, bottom 3 for short
Risk Management
Equal weight across long and short positions
Total gross leverage is distributed evenly across 6 positions
Exit Logic
Liquidate entire portfolio before monthly rebalance
Rebuild new portfolio each month based on updated rates
