# Monte Carlo Simulation for Stock Portfolio Analysis

## Project Overview
This project demonstrates a Monte Carlo simulation to analyze the potential returns and risks of investing in a stock portfolio. Using historical data from Yahoo Finance, the script simulates 1,000 potential outcomes for an initial investment of $10,000 in Apple (AAPL), based on historical mean returns and volatility.

## Features
1. **Data Retrieval:** Historical monthly data is fetched using the `yfinance` library.
2. **Return and Volatility Calculation:** Calculates annualized mean return and volatility based on historical data.
3. **Monte Carlo Simulation:** Generates random portfolio returns and final values.
4. **Risk Analysis:** Includes key metrics such as:
   - Mean and standard deviation of simulated returns
   - Value at Risk (VaR) at a 95% confidence level
   - Probability of loss
5. **Performance Insights:** Provides details like:
   - Best and worst portfolio performance
   - Highest and lowest returns
   - Mean and median final portfolio values
6. **Visualization:** Creates histograms for:
   - Simulated portfolio returns
   - Final portfolio values

## Requirements
To run this project, you need the following:
- Python 3.7 or later
- Libraries:
  - `numpy`
  - `matplotlib`
  - `yfinance`

Install the required libraries using:
```bash
pip install numpy matplotlib yfinance
```

## How to Run
1. Clone this repository or copy the script file.
2. Run the script in a Python environment.
3. View the generated plots and console output for the simulation results.

## Outputs
- **Console:**
  - Mean simulated return
  - Standard deviation of returns
  - Value at Risk (95% confidence level)
  - Loss probability
  - Best and worst portfolio performance
  - Mean and median final portfolio values
  
- **Plots:**
  - Histogram of simulated returns with key metrics highlighted
  - Histogram of final portfolio values with key metrics highlighted

## Example Results
After running the simulation, example output metrics include:
- **Mean Simulated Return:** ~8.5%
- **Standard Deviation:** ~20%
- **Value at Risk (95%):** -10%
- **Loss Probability:** ~30%
- **Mean Final Portfolio Value:** $12,500
- **Median Final Portfolio Value:** $12,200

## Customization
- **Stock Symbol:** Change the `symbol` variable to analyze different stocks (e.g., "MSFT", "GOOGL").
- **Date Range:** Modify the `start` and `end` dates in the `yfinance.download()` call.
- **Simulation Parameters:** Adjust `n_simulations` and `initial_investment` as needed.

## License
This project is licensed under the MIT License.
