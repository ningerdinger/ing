Explain the difference between implied and histotical volatility.

Implied volatility and historical volatility are two different measures of how much a stock's price has fluctuated in the past and may fluctuate in the future.

Historical volatility is a measure of the actual, realized volatility of a stock's price over a specific period of time, typically calculated using the standard deviation of the stock's price movements over that period. It reflects how much the stock price has moved up or down in the past.

Implied volatility, on the other hand, is a measure of the expected future volatility of a stock's price based on the prices of options contracts on that stock. It reflects the market's expectation of how much the stock price will move up or down in the future.

In other words, historical volatility is based on past price movements, while implied volatility is based on the market's expectations for future price movements, as reflected in the prices of options contracts.

Explain VaR and list at least two calculation methods.

Value at Risk (VaR) is a statistical measure used to estimate the potential loss that could be incurred on a portfolio of financial assets or a single asset over a given time period with a certain level of confidence. It provides a quantitative estimate of the amount of potential loss that could occur from normal market fluctuations.

There are several methods to calculate VaR, including:

Historical simulation: This method involves simulating the future price movements of a portfolio by using historical data. The VaR is then calculated based on the distribution of historical returns.

Parametric VaR: This method involves assuming that the returns on the portfolio follow a particular distribution, such as a normal distribution, and calculating the VaR based on this assumption. This method is generally used when the historical data is limited or not available.

Other methods include Monte Carlo simulation, which involves simulating the future price movements of a portfolio using random variables, and stressed VaR, which involves estimating the potential loss that could occur under extreme market conditions.

The VaR calculation typically involves three inputs: the time period over which the VaR is being calculated, the level of confidence (or probability) of the VaR estimate, and the value of the portfolio or asset being measured. For example, a VaR of $1 million with a 95% confidence level over a one-month time period indicates that there is a 5% chance that the portfolio or asset will lose more than $1 million over the next month.

The high level design I had in mind. Will elaborate later on.

![image](https://user-images.githubusercontent.com/52888356/234033338-80ff5e2f-3c73-413b-aee2-8cf40d36bcaf.png)

![image](https://user-images.githubusercontent.com/52888356/234033384-8bea4f75-ed85-4fd0-a7e6-6702b96821fd.png)

![image](https://user-images.githubusercontent.com/52888356/234034178-ae825b2c-57e7-4018-b5d7-347fd8ac283f.png)



tutorial to package this https://packaging.python.org/en/latest/tutorials/packaging-projects/

run this

py -m pip install --upgrade build

run this from the toml directory

py -m build

install twine

py -m pip install --upgrade twine

Make sure that you have a pypi account and token

run this to upload to pypi and fill in token as username, token as pw

py -m twine upload --repository testpypi dist/*

then just install from pypi and run it
