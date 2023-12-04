# Trading Bot Framework
This repository provides a framework for building your own trading bot using Python, CCXT, and Pandas. It includes a set of helper files that can speed up your development process and help you create a customized trading bot.

The framework is designed to be open-source and extensible, allowing users to build upon it and tailor it to their specific needs.

## Included Files
- ccxt_utils.py: A collection of boilerplate methods that simplify the use of CCXT for fetching and processing trading data.
- indicators.py: A set of implemented trading indicators that accept a Pandas DataFrame as input.
- oms_logger.py: A rudimentary Order Management System (OMS) logger to record all transactions.
- BotTemplate.py: A fully functional bot template that provides basic bot functionality, but does not execute any transactions.

## Exclude File
In order to keep your API keys secure, you need to create a separate configuration file named dontshare_config.py. This file will store your API keys for the exchanges you want to use with the trading bot. Make sure not to include this file in your public repository, as it contains sensitive information. The trading bot will not run if the dontshare_config.py file is not created and properly configured with your API keys. Make sure to follow the steps above to set up the file before running the bot.

### Creating the dontshare_config.py file
Create a new file named dontshare_config.py in the root directory of your project.
Add your API keys for the exchanges you want to use, following the format below:
```
BYBIT_API_KEY='<insert your key here>
BYBIT_SECRET_KEY='<insert your secret here>
#Add other keys for exchanges you like to use
```
Replace <insert your key here> and <insert your secret here> with your actual API key and secret key for each exchange.

Save the file and make sure it is not included in your public repository. You can add it to your .gitignore file to prevent it from being accidentally committed.
  
## Usage
To use this framework, simply clone the repository and start building your own trading bot using the provided helper files. Modify and extend the code as needed to create your own customized trading bot.

## Legal Disclaimer
By using this framework and any of its provided files, you agree that the author(s) of this repository are not responsible for any financial losses or damages that may occur as a result of using, modifying, or implementing the provided code. Trading cryptocurrencies and other financial instruments carries a risk, and you should be aware of the potential for financial loss before engaging in any trading activities.

It is your responsibility to ensure that your trading bot adheres to any applicable laws, regulations, and exchange-specific rules. The author(s) of this repository make no guarantees regarding the performance, reliability, or accuracy of the provided code, and cannot be held liable for any consequences that may arise from its use.

Please use this framework at your own risk, and exercise due diligence when developing and deploying your trading bot.
