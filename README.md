# Stock-Data-Analysis

# Introduction

This project analyses stock data downloaded from yfinance, focusing on the adjusted closing prices of popular stocks for the year 2023. It includes:
- Importing the stock data using yfinance package.
- Data analysis on the stocks such as simple daily rate of return, mean simple daily rate of return, annualised returns, variance & standard deviation in simple daily 
  returns and covariance between stocks simple daily returns. 
- Creating random portfolios of different stock weights.
- Finding the efficient frontier for these random portfolios.
- Adding some more stocks and comparing the impact on the random portfolios and efficient frontier.
- Recommending portfolios. Risky, average and safe.

# Dataset

The dataset includes:
- Adjusted closing prices for multiple stocks from January 1, 2023, to December 31, 2023.
- The stocks include:
  - Amazon (AMZN)
  - JP Morgan (JPM)
  - Facebook/Meta (META)
  - Microsoft (MSFT)
  - Netflix (NFLX)
  - Ferrari (RACE)
  - S&P 500 (SPY)
  - Tesla (TSLA)
  - Nvidia (NVDA)
  - Advanced Mirco Devices (AMD)
 
# Project Workflow

# 1. Adjusted Closing Prices
   - Comparing the adjusted closing prices of each stock to see how volatile each one was and the potential returns each one yields.

# 2. Daily Rate Of Return Analysis
   - Calculated the simple daily rate of return for each stock.
   - Visualised the daily returns using a line graph for each stock.

# 3. Mean Simple Daily Returns And Annualised Returns
   - Calculated the mean simple daily rate of return and visualised it to compare between each stock.
   - Used the mean value to calculate an annualised return for each stock.
   - Visualised the annualised returns to see which stock had most potential.

# 4. Risk Analysis
   - Computed variance and standard deviation of each stocks simple daily returns.
   - Visualised these findings to compare and see which stocks were more volatile.
   - Created a covariance table showing the relationship between each stocks simple daily returns. To improve diversification and lower the volatility of the portfolio.

# 5. Portfolio Creation
   - I created a function to generate random portfolios with varying stock weight distributions.
   - For this project 10,000 portfolios were created.
   - The outcome from the function is a dictionary of portfolios with these columns Returns, Volatility, Weights and Sharpe Ratio.
   - Visualised the random portfolios on a scatter plot of volatility vs returns

# 6. Efficient Frontier Calculation
   - Created a function to compute the efficient frontier for the random portfolios.
   - For this project I calculated 1000 portfolios for the efficient frontier.
   - The outcome of the function is the same dictionary format as the random portfolios.
   - Visualised the efficient frontier with the random portfolios to see the optimal portfolios.

# 7. Additional Stocks
   - Downloaded more stock data for Nvidia and Advanced Mirco Devices.
   - Repeated all the previous steps of analysis for these new stocks.
   - Generated more random portfolios and an efficient frontier for them.
   - Visualised all random portfolios and both efficient frontiers on one graph to compare the impact of two new stocks.

# 8. Portfolio Recommendations
   - Suggested three portfolios:
   - Risky portfolio (high return, high volatility)
   - Moderate portfolio (balanced return and risk)
   - Safe portfolio (low risk, stable return)

# Installation

- Clone the repostiory using:
  git clone https://github.com/AdamBartlett7/Stock-Data-Analysis.git
- Navigate to the correct directory using:
  cd Stock-Data-Analysis
- Create your own virtual environment with the necessary python libraries using:
  conda env create -f environment.yml
- Then open and run Stock_Data.ipynb.
  
# Usage

- Run Stock_Data.ipynb in sequential order to see all the stock data analysis.

# Key Findings

- Stocks exhibit different levels of risk and return, highlighting the importance of diversification.
- Portfolio optimization through the efficient frontier improves return to risk ratios.
- Strategic allocation helps in creating portfolios that suit different risk tolerances.
- Initially META and Tesla had the highest mean daily returns but then Nvidia had the most when added.
- Although Nvidia had the highest mean daily return it only had the second highest standard deviation. Tesla had the highest and AMD had the third highest.

# Portfolio Results

- Risky portfolio
  
  |            | Returns   | Volatility | Sharpe Ratio |
  | ---------- | --------- | ---------- | ------------ |  
  | Daily      | 0.39595%  | 1.81042%   | 0.2186       |
  | Annual     | 99.77852% | 28.73948%  | 3.47009      |

  | Stock      | Weight    |
  | ---------- | --------- |
  |AMD         | 0         |
  |AMZN        | 0         |
  |JPM         | 0.05504   |
  |META        | 0.36605   |
  |MSFT        | 0         |
  |NFLX        | 0.03301   |
  |NVDA        | 0.31013   |
  |RACE        | 0.21879   |
  |SPY         | 0         |
  |TSLA        | 0.01698   |
  
- Safe portfolio
  
  |            | Returns   | Volatility | Sharpe Ratio |
  | ---------- | --------- | ---------- | ------------ |  
  | Daily      | 0.1701%   | 0.95524%   | 0.17787      |
  | Annual     | 42.86554% | 15.16396%  | 2.82351      |

  | Stock      | Weight    |
  | ---------- | --------- |
  |AMD         | 0         |
  |AMZN        | 0         |
  |JPM         | 0.17943   |
  |META        | 0.05975   |
  |MSFT        | 0.08536   |
  |NFLX        | 0.02218   |
  |NVDA        | 0.03699   |
  |RACE        | 0.21339   |
  |SPY         | 0.4029    |
  |TSLA        | 0         |
  
- Mixed portfolio

  |            | Returns   | Volatility | Sharpe Ratio |
  | ---------- | --------- | ---------- | ------------ |  
  | Daily      | 0.28291%  | 1.317%     | 0.21467      |
  | Annual     | 71.29354% | 20.90671%  | 3.40769      |

  | Stock      | Weight    |
  | ---------- | --------- |
  |AMD         | 0         |
  |AMZN        | 0         |
  |JPM         | 0.23576   |
  |META        | 0.20342   |
  |MSFT        | 0.05225   |
  |NFLX        | 0.05451   |
  |NVDA        | 0.15478   |
  |RACE        | 0.29927   |
  |SPY         | 0         |
  |TSLA        | 0         |

# Future Improvements

- Incorperate Alpha and Beta or other performance metrics.
- Expand analysis to include more years of data and different stocks.

# License
- This project is licensed under the MIT License. See the LICENSE file for details.
