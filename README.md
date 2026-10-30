# Limit Order Book & Market Microstructure

A quantitative research project investigating **limit order book dynamics, order-flow imbalance, and short-horizon price prediction**.

The project aims to understand whether information contained in the limit order book can provide predictive information about very short-term price movements, and whether such predictive signals remain useful after accounting for transaction costs.

## Research Questions

- How does a limit order book evolve over time?
- How informative is order-book imbalance about future price movements?
- Does order-flow imbalance contain additional predictive information?
- Which order-book features are most useful for short-horizon prediction?
- Does statistical predictability translate into a tradable signal after fees, spread, and slippage?

## Project Roadmap

- [ ] Build a limit order book simulator
- [ ] Implement order matching and cancellation
- [ ] Write unit tests for the order-book engine
- [ ] Obtain and process real order-book data
- [ ] Reconstruct order-book snapshots
- [ ] Analyze spread, depth, and mid-price dynamics
- [ ] Engineer order-book and order-flow features
- [ ] Study the relationship between features and future returns
- [ ] Build statistical prediction models
- [ ] Evaluate machine-learning models
- [ ] Develop a simple trading strategy
- [ ] Backtest with transaction costs and slippage
- [ ] Perform robustness and out-of-sample analysis

## Planned Features

### Order Book

- Bid/ask prices
- Bid/ask quantities
- Mid-price
- Bid-ask spread
- Market depth
- Multi-level order-book imbalance

### Order Flow

- Limit-order additions
- Order cancellations
- Market-order executions
- Order-flow imbalance
- Changes in bid/ask depth

### Statistical Features

- Short-horizon returns
- Volatility
- Autocorrelation
- Rolling statistics

## Models

The project will progressively evaluate:

1. Baseline statistical models
2. Logistic Regression
3. Random Forest
4. Gradient Boosting
5. Neural-network models, if justified by the results

## Evaluation

Models and strategies will be evaluated using:

- Accuracy
- Precision / Recall
- ROC-AUC
- Prediction calibration
- Feature importance
- Out-of-sample performance
- P&L
- Sharpe ratio
- Maximum drawdown
- Turnover

Trading performance will be evaluated after accounting for **transaction costs, bid-ask spread, and slippage**.

## Project Structure

```text
order-book-microstructure/
│
├── data/
│
├── notebooks/
│
├── src/
│   ├── orderbook.py
│   ├── features.py
│   ├── labels.py
│   ├── models.py
│   └── backtest.py
│
├── tests/
│
├── results/
│   ├── figures/
│   └── tables/
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Technology

- Python
- NumPy
- Pandas
- SciPy
- Matplotlib
- Scikit-learn
- Jupyter

Additional libraries will be added as the project develops.

## Status

**In development**

The project is being developed progressively, beginning with a custom limit order book simulator and order-matching engine before moving to real market data and quantitative prediction.

## Disclaimer

This project is for **research and educational purposes**. Backtested results do not guarantee future trading performance.
