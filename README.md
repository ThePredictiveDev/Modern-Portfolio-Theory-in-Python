# Modern Portfolio Theory (MPT) in Python
Modern Portfolio Theory (MPT) is a financial theory that aims to create a portfolio of assets that offers the maximum possible expected return for a given level of risk. 
This project implements MPT in Python to help investors optimize their portfolio by finding the ideal combination of assets for their investment. 
The primary goal is to create a portfolio that maximizes return and minimizes risk. 

## The key components of the project are as follows:

### Downloading Financial Data
We start by downloading historical financial data for a set of stocks. In this example, we are using the Yahoo Finance API to obtain data for four stocks: HDFC Bank, ICICI Bank, Axis Bank, and State Bank of India. The user can customize the list of stocks and the date range.

### Creating Log Return Data Frame
We create a data frame with the log returns of the stock prices. Log returns are commonly used in finance because they have nice properties for portfolio analysis. The data is cleaned to remove missing values.

### Calculating Portfolio Return
We calculate the portfolio return using a function that takes the weights of assets in the portfolio and multiplies them by the expected returns of the assets. The result is annualized.

### Calculating Portfolio Standard Deviation (Risk)
Portfolio risk is calculated using a function that takes the weights of assets in the portfolio and uses the covariance matrix of the asset returns. The result is annualized.

### Generating Random Portfolio Weights
Random portfolio weights are generated for each asset. These weights represent the proportion of each asset in the portfolio.

### Finding Returns and Standard Deviation for Random Portfolios
We loop through a specified number of iterations to generate random portfolio weights and calculate the returns and risk (standard deviation) for each portfolio. These portfolios form the Efficient Frontier, which is a graph that shows the relationship between risk and return.

### Plotting the Efficient Frontier
We use Matplotlib to create a scatter plot of the Efficient Frontier. Each point on the graph represents a portfolio with a specific risk and return. We also highlight the portfolio with the maximum return and the portfolio with the minimum risk.

### Finding Max Returns and Associated Risk
We identify the portfolio with the maximum return and the corresponding risk. This portfolio represents the maximum return achievable within the given set of assets.

### Finding Efficient Portfolio Weights
We create a function to return the weights of portfolios whose returns are greater than or equal to the maximum return on the Efficient Frontier. These weights represent efficient portfolios that offer high returns for the level of risk.

#### This project helps investors make data-driven decisions about their portfolios by identifying the best combination of assets to maximize returns while managing risk.




