# Portfolio Optimization with Domain Knowledge (WIP)

We will use the portfolio optimization techniques highlighted in the paper, “Portfolio Cuts: A Graph-Theoretic Framework to Diversification” ([arXiv:1910.05561](https://arxiv.org/pdf/1910.05561)), to find an ideal allocation of resources when investing in the stock market.



## GENERAL OVERVIEW
For each stock, we get:
- Downloadable data from Yahoo Finance (P/E Ratio, etc.)
- Moving Averages
- Current Price (log of price may yield more accurate results)
- Sector, Industry
- etc.
These become our predictor variable (X). Using these variables we predict where the stock will be after a certain, predetermined time frame.
This will be our prediction (Y). For instance, we may want to predict where the stock will be in 1 month or in 1 year.


## STATISTICAL IDEAS
Some statistical practices we could include are:
- Variable Transformations (log, square)
- Interaction Variable
- Variable Selection

### Interaction Variables
Some of the predictor variables may be correlated. For instance, the sector of the company may influence the stock prices.
In this case, we would introduce interaction variable to make our predictions more accurate.

## MODELS
Some models to test:
- Polynomial Regression (linear may underfit)
- Logistic Regression (win/lose)
- Decision Tree (XGBoost)
- Neural Networks (may overfit)
- KNN for predicting new stocks

