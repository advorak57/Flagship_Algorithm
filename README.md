# Trading Strategy Backtesting
---
This code is an implementation of a simple trading strategy backtesting. The strategy uses technical indicators such as Bollinger Bands, Moving Averages Convergence Divergence (MACD), and Relative Strength Index (RSI) to identify potential buy and sell signals for a particular stock (TSLA).

The strategy involves entering a long position when the RSI is above 50 and the closing price is above the upper Bollinger Band or when the MACD fast moving average crosses above the slow moving average and RSI is below 50. The position is exited when the MACD fast moving average crosses below the slow moving average or the RSI is above 50 or when the price hits the stop-loss or take-profit levels.

The code fetches historical data for TSLA from the Interactive Brokers API and calculates the technical indicators. It then iterates over the data and generates signals based on the strategy. Finally, it calculates the profit and loss, win rate, and other metrics.

### Requirements
The following Python packages are required to run this code:

ibapi
pandas
numpy
Usage


Ensure that you have an Interactive Brokers account and have the API enabled.
Set the starting_balance and risk_amount variables to your desired values.
Run the code and wait for the backtesting to complete.
The code will output the results of the backtesting, including the original balance, win rate, number of trades, profit/loss ratio, and total balance after trades.

### Disclaimer
This code is provided for educational purposes only and should not be used for actual trading. The results of the backtesting are based on past performance and do not guarantee future results. Trading carries a risk of loss and you should only trade with funds that you can afford to lose.
