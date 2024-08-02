# Predicting MSFT (Microsoft) equity prices using historic data (time-series analysis)

I used yahoo finance for this project: https://pypi.org/project/yfinance/

This is a project using historic price data to try and predict whether or not Microsoft prices will rise or fall from the previous day's price. The target variable was set to be 1 or 0 (1 if the price was greater than the previous day's price or 0 if it were less than the previous day's price), and is specifically based on the close price. 

Using the previous day's values as features, a random forest classifier was used as the ML model. All the historic prices were used and the precision score was evaluated. When seasonal means were added as features the precision rose from 0.51 to 0.59. 

There are several reasons accounting for the poor performance of the model. Firstly, historic prices are a poor indicator for future prices. Secondly, the model may be improved by considering other stocks, volatility indices and equities after a later date. 





