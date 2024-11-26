# Pairs Trading
```
cointegration_pairs_trading/
├── data/
├── notebooks/
│   ├── parameter_tuning.ipynb
│   ├── strategy_backtesting.ipynb
├── src/
│   ├── __init__.py
│   ├── config.py
│   ├── data_preprocessing.py
│   ├── stock_paring.py
│   ├── signal_processing.py
│   ├── backtester.py
│   ├── parameter_tuning.py
│   ├── utils.py
├── tests/
├── requirements.txt
├── README.md
├── .gitignore
```

## `data/`  
> Stores all data files used in this project.

## `notebooks/`  
> Contains (Jupyter) Notebook files for analysis and development.
- `parameter_tuning.ipynb`
  - Runs optimization algorithms to find optimal parameter sets.
  - Analyzes the impact of different parameters on strategy performance.
- `strategy_backtesting.ipynb`
  - Runs the trading strategy over historical data.
  - Evaluates performance metrics, e.g. Sharpe ratio.
  - Visualizes backtesting results and performance.

## `src/`
> Contains the source code modules that implement the core functionality.
- `__init__.py`
  - Allows modules within `src/` to be imported elsewhere in the project.
- `config.py`
- `data_preprocessing.py`
- `stock_paring.py`
- `signal_processing.py`
- `backtester.py`
- `parameter_tuning.py`
- `utils.py`
