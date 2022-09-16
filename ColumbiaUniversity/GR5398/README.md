# AI4Finance-Education

##Title: FinRL for Live Trading
GitHub: https://github.com/AI4Finance-Foundation/FinRL
Purpose: Based on the open-source financial reinforcement learning framework-FinRL, develop an AI stock-selection and trading strategy based on Supervised Machine Learning (Supervised ML) and Deep Reinforcement Learning (DRL) algorithms and deploy it to an online trading platform for paper trading.

### Phase I: Data Processing and Feature Engineering
1. Download and install FinRL, download S&P 500 Open, High, Low, Close, and Volume (OHLCV) and Fundamental Indicators (company fundamental data), and convert the data into a daily format

2. Perform feature engineering: based on OHLCV data to make company technical analysis indicators such as MACD, RSI; based on company fundamental data to make fundamental indicators such as EPS, ROI, ROE, P/E, P/S; and convert it into machine learning data format

**Your Delivery**: code and a CSV file with quarterly data of S&P 500 stocks
image.png

### Phase II: Stock Selection and Portfolio Allocation with Backtesting Results
1. Stock Selection: Perform supervised machine learning using classic machine learning algorithms (LSTM, Random Forest, SVM, Linear Regression, Lasso, Ridge) to select stocks based on fundamental multi-factor data, and select the top 25% of stocks every quarter; 
• Reference paper: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3302088
• GitHub Code: https://github.com/AI4Finance-Foundation/Machine-Learning-for-Stock-Recommendation-IEEE-2018

2. Portfolio Allocation: Use Deep reinforcement learning Ensemble strategy (PPO, DDPG, A2C, SAC, TD3) in FinRL for asset allocation of the selected stocks, trade with daily data, and output positions; 
• Reference paper: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3690996
• GitHub Code: https://github.com/AI4Finance-Foundation/FinRL-Meta/blob/master/tutorials/1-Introduction/FinRL_PortfolioAllocation_NeurIPS_2020.ipynb

**Your Delivery**: code and a backtesting chart with return results of 1) Our Trading Strategy (ML Selection+FinRL Portfolio Allocation); 2) Minimum-Variance Portfolio Allocation Strategy; 3) Equally Weighted Portfolio Allocation Strategy of Selected Stocks; 4) S&P 500 Index 
image.png

### Phase III: Deploy the DRL trading strategy to an online trading platform
1. Deployment: Deploy strategies to online trading platforms such as Alpaca for paper trading
• GitHub Code: https://github.com/AI4Finance-Foundation/FinRL-Meta/blob/master/tutorials/3-Practical/FinRL_PaperTrading_Demo.ipynb

**Your Delivery**: code and a screenshot of your paper trading portfolio, ideally 5% greater than the S&P 500 Index return
image.png