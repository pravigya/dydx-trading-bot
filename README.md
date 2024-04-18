# Dydx Trading Bot

## Overview
This trading bot is designed to automate trading on the Dydx decentralized exchange using statistical arbitrage strategies. It is deployed on AWS and includes Telegram notification functionality to keep you updated on trades and important events.

## Features
- Automated trading on Dydx decentralized exchange
- Integration with AWS for deployment
- Telegram notification functionality for trade updates
- Configurable trading strategies
- Statistical arbitrage using cointegrated pairs, spread, Z-scores, hedge ratios, etc.

## Requirements
- Python 3.x
- AWS account
- Telegram account and bot token

## Installation
1. Clone the repository
2. Install dependencies using `pip install requirements.txt`


## Configuration
1. Set up your AWS credentials for deployment.
2. Create a Telegram bot and obtain the bot token.
3. Configure the bot settings in `config.py`, including Dydx API credentials, AWS configuration, Telegram bot token, and statistical arbitrage parameters.

## Usage
1. Run the bot locally
2. Deploy the bot on AWS

## Statistical Arbitrage
-  **Stationarity**: A stationary time series is the one whose stastical parameters such as mean and variance do not change over time.
- **Cointegrated Pairs**: If the linear combination or spread of two stationary time series is stationary then they are said to be cointegrated with each other. 
- **Spread**: Calculate the spread between the prices of cointegrated pairs. `spread = series_1 - (hedge_ratio * series_2)`
- **Z-Scores**: Compute Z-scores to determine whether the spread is deviating from its historical mean. `zscore = (x - mean) / std`
- **Hedge Ratios**: Determine optimal hedge ratios for pairs trading.

## Example Strategies
1. Simple Moving Average (SMA) crossover strategy
2. Relative Strength Index (RSI) strategy
3. Bollinger Bands strategy
4. Statistical arbitrage using cointegrated pairs and Z-scores

## Support
For any issues or questions, please open an issue on GitHub or contact [your_email@example.com].

## Disclaimer
This trading bot is for educational and experimental purposes only. Use it at your own risk and do your own research before making any financial decisions. The developers are not responsible for any losses incurred while using this software.

## License
MIT License
