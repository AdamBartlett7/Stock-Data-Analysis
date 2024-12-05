# Stock-Data-Analysis

Overview - This project focuses on stock data. It includes:
- Importing the stock data
- Data analysis on the stocks
- Creating random portfolios of different stock weights
- Finding the efficient frontier for these random portfolios
- Recommending portfolios

Features
- Importing in the stock data using the yfinance package
- Stocks including MSFT, AMZN, RACE, JPM, TSLA, NFLX, SPY, META, NVDA, AMD
- Analysing key stock metrics like adjusted closing price, daily returns, variance, standard deviation and covariance
- Visualisations that compare the metrics between the stocks
- Creating a function that will generate a number of predetermined amount of different portfolios with different stock weights
- Creating another function that given those random portfolios will find the effcient frontier
- Importing some additional stocks and analysing the key metrics
- Generating random portfolios with the additional stocks
- Finding the efficient frontier and visualising the impact of the additional stocks on it
- Recommending a risky, balanced and safe portfolio

Installation
- Clone the repostiory using:
- git clone https://github.com/AdamBartlett7/Stock-Data-Analysis.git
- cd Stock-Data-Analysis
- Create your own virtual environment if needed
- To install the necessary python libraries:
- pip install -r requirements.txt
  
Usage
- Run Stock_Data.ipynb in sequential order

Dataset
- The data was obtained by installing the package yfinance and using it to download the various stock data.
- It includes the stock data for the year 2023 for some of the biggest companies in the world.

Results
- Some interesting findings from this were the returns for certain stocks and the volatility that came with that.
- META and Tesla having the highest mean daily returns but also having the highest variance and standard deviation.
- Also when creating a portfolio of stocks the trade off between maximising returns but minimising volatility.
- Risky portfolio returns: 0.00396%
- Risky portfolio volatility: 0.01813%
- Safe portfolio returns: 0.0017%
- Safe portfolio volatility: 0.00959%
- Balanced portfolio returns: 0.00283%
- Balanced portfolio volatility: 0.01317%

License
- This project is licensed under the MIT License. See the LICENSE file for details.
