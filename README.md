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
  - Evaluates performance metrics (e.g., Sharpe ratio).
  - Visualizes backtesting results and performance.

## `src/`
> Contains the source code modules that implement the core functionality.
- `__init__.py`
  - Allows modules within `src/` to be imported elsewhere in the project.
- `config.py`
  - Stores configuration settings and default parameters.
- `data_preprocessing.py`
  - Implements data cleaning and preprocessing routines.
  - Saves processed data to the `data/` directory.
- `stock_paring.py`
  - Implements cointegration tests (e.g., Engle-Granger, Johansen tests).
  - Identifies cointegrated pairs of assets.
- `signal_processing.py`
  - Generates long/short signals from pairs based on `stock_paring.py`.
  - Manages positions and applies risk management.
- `backtester.py`
  - Executes trades based on signals from `strategy.py`.
- `parameter_tuning.py`
  - Defines parameter spaces and optimization objectives.
  - Implements parameter search algorithms.
  - Finds parameter sets that optimize performance metrics.
- `utils.py`
  - Provides utility functions used across modules.
