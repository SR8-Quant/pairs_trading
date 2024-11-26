# Pairs Trading Project Structure
```
cointegration_pairs_trading/
├── data/
├── reports/
│   ├── parameter_tuning.ipynb
│   ├── backtesting.ipynb
├── src/
│   ├── __init__.py
│   ├── config.yaml
│   ├── data_preprocessing.py
│   ├── stock_pairing.py
│   ├── signal_processing.py
│   ├── backtester.py
│   ├── parameter_tuning.py
│   ├── utils.py
├── test/
├── requirements.txt
├── README.md
├── .gitignore
```
## Description
### `data/`  
> Stores all data files used in this project.

### `reports/`  
> Contains (Jupyter) Notebook files for analysis.
- `parameter_tuning.ipynb`:
  - Explores and optimizes different parameters affecting strategy performance.
  - Evaluates and Visualizes the results of different parameters on strategy performance.
- `backtesting.ipynb`:
  - Runs backtesting.
  - Evaluates performance metrics.
  - Visualizes backtesting results and overall performance.

### `src/`
> Contains the source code modules that implement the core functionality.
- **`__init__.py`**: Allows modules within `src/` to be imported elsewhere in the project.
- **`config.yaml`**: Stores configuration settings and default parameters.
- **`data_preprocessing.py`**:
  - Implements data cleaning and preprocessing routines.
  - Saves processed data to the `data/` directory.
- **`stock_pairing.py`**:
  - Implements cointegration tests (e.g., Engle-Granger, Johansen tests).
  - Identifies cointegrated pairs of assets.
- **`signal_processing.py`**:
  - Generates long/short signals from pairs based on `stock_pairing.py`.
  - Manages positions
  - Applies take-profit/risk management.
- **`backtester.py`**: Executes trades based on signals from `signal_processing.py`.
- **`parameter_tuning.py`**: Runs optimization algorithms to find optimal parameter sets.
- **`utils.py`**: Provides utility functions used across modules.

### `test/`
> Contains unit tests to verify the correctness of code modules.

### `requirements.txt`
> Lists all Python package dependencies.
- Specifies package names and versions required for the project.
- Allows users to install all dependencies using `pip install -r requirements.txt`.

### `README.md`
> Provides project documentation.

### `.gitignore`
> Defines files and directories to be ignored by Git.
