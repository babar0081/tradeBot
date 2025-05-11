

What is Trading Bot?
Trading Bot is a crypto trading bot written in Python. It is designed to support all major exchanges and be controlled via Telegram or its webUI. It contains backtesting, plotting, and money management tools, as well as strategy optimization by machine learning.
Disclaimer
Always start by running a trading bot in Dry-run and do not engage money before you understand how it works and what profit/loss you should expect.
It's highly recommended to have coding and Python knowledge. Do not hesitate to read the source code and understand the mechanism of this bot.
Supported Exchange Marketplaces
This Trading Bot is designed to support many major crypto exchanges, including:
Binance
Bitmart
BingX
Bybit
Gate.io
HTX
Hyperliquid (A decentralized exchange, or DEX)
Kraken
OKX
MyOKX (OKX EEA)
Many others might potentially work via the underlying exchange library (CCXT), though their functionality cannot be guaranteed without specific integration.
Supported Futures Exchanges (Experimental)
Experimental support for futures trading is available on:
Binance
Gate.io
Hyperliquid (A decentralized exchange, or DEX)
OKX
Bybit
Please make sure to read any exchange-specific notes provided by the Trading Bot, as well as its documentation on trading with leverage before diving in.
Community Tested Exchanges
Some exchanges confirmed working by the community (when this was Freqtrade) include:
Bitvavo
Kucoin
Please read any exchange-specific notes to learn about eventual, special configurations needed for each exchange.
Documentation
Users are invited to read the Trading Bot's documentation to ensure they understand how it works. Complete documentation should be available on the Trading Bot's official website or resource page.
How It Works & Features
The Trading Bot offers a comprehensive suite of features for automated cryptocurrency trading:
Python-Based: Developed in Python (typically 3.10+), allowing it to run on various operating systems like Windows, macOS, and Linux.
Data Persistence: Achieves persistence, often through databases like SQLite, to store trading data, configurations, and history.
Dry-run Mode: Allows users to run the bot with simulated trades using real-time market data, without risking actual capital. This is crucial for testing strategies.
Backtesting Engine: Enables users to simulate their trading strategies on historical market data to evaluate potential performance.
Strategy Optimization via Machine Learning: Provides tools to use machine learning techniques to optimize the parameters of trading strategies based on historical exchange data.
Adaptive Prediction Modeling: Can incorporate advanced AI features (like "FreqAI" in its original form) to build smart strategies that self-train and adapt to changing market conditions using machine learning.
Edge Position Sizing: Includes capabilities to calculate win rates, risk-reward ratios, and optimal stop-loss levels, and to adjust position sizes accordingly for specific markets before entering a trade.
Cryptocurrency Whitelisting: Allows users to select specific cryptocurrencies they want the bot to trade, or use dynamic whitelists based on certain criteria.
Cryptocurrency Blacklisting: Enables users to specify cryptocurrencies they want the bot to avoid trading.
Built-in Web User Interface (WebUI): Often comes with a web-based interface for managing and monitoring the bot's operations, viewing trades, and adjusting settings.
Telegram Integration: Can be managed and monitored via Telegram, allowing users to receive notifications and issue commands remotely.
Fiat Profit/Loss Display: Can display profit and loss figures in a chosen fiat currency for easier understanding of performance.
Performance Status Reporting: Provides reports on the performance of current and past trades, often grouped by pair or strategy.
Quick Start / Getting Started
To get started with this Trading Bot, you would typically refer to its official documentation. This might include Docker Quickstart guides for easy setup or instructions for native installation methods on your operating system.
Basic Usage / How to Use It
Using the Trading Bot generally involves:
Configuration: Setting up a configuration file that defines your exchange API keys, trading pairs, strategy, stake amount, and other operational parameters.
Strategy Development/Selection: Choosing or developing a trading strategy. Strategies define the rules for when the bot should buy or sell.
Data Download (for Backtesting): Downloading historical market data for the pairs you intend to trade if you plan to backtest your strategy.
Backtesting: Running your chosen strategy against historical data to see how it would have performed.
Optimization (Optional): Using tools like Hyperopt (if available) to find the best parameters for your strategy.
Dry-Run: Running the bot in a simulated mode on live markets to observe its behavior without risking real funds.
Live Trading: Once confident, running the bot with real capital on an exchange.
Monitoring: Using the WebUI or Telegram to monitor the bot's performance, open trades, and logs.
The bot is operated through a set of commands (via a command-line interface or its UI) for actions like starting trades, creating user directories, managing configurations, downloading data, running backtests, etc. Telegram can also be used for remote control, allowing users to start/stop the bot, check status, force-exit trades, and view performance.
Requirements
To run this Trading Bot effectively, certain requirements usually need to be met:
Accurate System Clock: The computer running the bot must have an accurately synchronized clock (e.g., via NTP) to avoid issues with exchange API communication.
Minimum Hardware: While varying, a typical recommendation might be a cloud instance or local machine with at least 2GB RAM, 1GB of disk space, and a 2-core CPU.
Software Dependencies:
Python (a recent version, e.g., 3.10 or higher).
pip (Python package installer).
git (for obtaining the software if distributed via Git).
Technical Analysis libraries (e.g., TA-Lib).
virtualenv (recommended for creating isolated Python environments).
Docker (often recommended for easier deployment and dependency management).
