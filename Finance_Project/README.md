# Finance Data Project – Bank Stock Analysis

## Overview
This project conducts an exploratory data analysis (EDA) on major U.S. bank stocks from January 1, 2006 to January 1, 2016, capturing the run-up to, crash during, and recovery from the 2008 financial crisis. We focus on:

- **Bank of America (BAC)**
- **CitiGroup (C)**
- **Goldman Sachs (GS)**
- **JPMorgan Chase (JPM)**
- **Morgan Stanley (MS)**
- **Wells Fargo (WFC)**

Key analyses include price trends, returns, risk metrics (volatility, kurtosis, Sharpe ratios), and technical indicators (moving averages, Bollinger Bands).

## Repository Structure
```
├── FinanceProject.ipynb   # Jupyter Notebook with all analyses and visualizations
├── all_banks/             # Pickle file containing historical data for each bank
├── requirements.txt       # List of Python dependencies
└── README.md              # Project overview and setup instructions
```

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/Nahid-ahmdv/EDA_Projects.git
   cd EDA_Projects/Finance_Project
   ```
2. Create a virtual environment and install packages:
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate    # Windows
   .\venv\Scripts\Activate.ps1   # Windows (PowerShell)
   pip install -r requirements.txt
   ```

## Usage
1. Open the Jupyter Notebook:
   ```bash
   jupyter lab FinanceProject.ipynb   # or jupyter notebook FinanceProject.ipynb
   ```
2. Run each cell in order. The notebook is organized into these sections:
   1. **Introduction:** Project goals and data sources.
   2. **Data Loading & Preparation:** Library imports and data retrieval via `pandas_datareader` or `yfinance`.
   3. **Data Cleaning:** Handling missing values and formatting.
   4. **Exploratory Data Analysis (EDA):** Summary statistics, distributions, and correlations.
   5. **Visualizations:** Static (Matplotlib/Seaborn) and interactive (Plotly/Cufflinks) charts.
   6. **Technical Indicators:** Simple moving averages, Bollinger Bands.
   7. **Conclusions:** Key insights and takeaways.

## Dependencies
All required packages are listed in `requirements.txt`. Key libraries include:

- pandas
- numpy
- matplotlib
- seaborn
- pandas_datareader or yfinance
- plotly
- cufflinks

## Key Findings
- **Citigroup** suffered the steepest crash in 2008 and slowest recovery.
- **Goldman Sachs** and **JPMorgan Chase** were the most resilient, showing strong rebounds.
- **Volatility metrics** (standard deviation, kurtosis) highlight extreme risk in Citigroup.
- **Sharpe Ratios** indicate Wells Fargo and JPMorgan offered the best risk-adjusted returns.
- **Technical plots** (rolling averages, Bollinger Bands) reveal clear periods of over- and under-valuation.

## License
This project is released under the MIT License.

---
*This README was generated alongside the EDA notebook. For detailed methodology and full results, please refer to `FinanceProject.ipynb`.*
