🧠 Strategies Included

The repo currently focuses on three core strategies:
	•	Momentum Trend
Identifies assets trading above their 50-day SMA and filters using RSI to avoid overbought signals.
	•	Mean Reversion (coming soon)
Will use indicators like Bollinger Bands and Z-score to capture price deviations.
	•	Statistical Arbitrage (coming soon)
Will involve pair trading, cointegration, and mean-reversion logic between correlated assets.

⸻

📁 Example: Momentum Trend Strategy

Below is a snapshot of the momentum trend strategy logic currently implemented:

1. Scrape tickers from the Nasdaq-100 list
2. Download 7 months of historical prices
3. Filter stocks trading above their 50-day SMA
4. Calculate RSI and exclude overbought assets (RSI > 70)
5. Sort remaining stocks by 6-month return
6. Print top 5 and allocate $10,000 to top 3 performers

 🔍 Indicators used:
	•	50-Day Simple Moving Average
	•	RSI (Relative Strength Index)
	•	6-Month Return

 📤 Sample Output:
 Top 5 Stocks by 6-Month Return:
Ticker       6M Return (%)
-------------------------
AAPL               23.50
NVDA               21.70
MSFT               19.40

Suggested Allocation of $10,000:
Ticker       Price    Shares     Invested
------------------------------------------
AAPL         192.88        17       3278.96
NVDA         457.68         7       3203.76
MSFT         358.82         9       3229.38
Total                                9712.10

⚙️ Tools & Libraries
	•	Python 3.9+
	•	Pandas – data manipulation
	•	NumPy – numerical operations
	•	yfinance – price data collection
	•	(Planned: TA-Lib, statsmodels, scikit-learn)

 📈 Metrics & Evaluation
	•	Sharpe Ratio
	•	Return %
	•	Max Drawdown
	•	RSI and Z-score filters
	•	Backtest-ready structure (coming soon)

