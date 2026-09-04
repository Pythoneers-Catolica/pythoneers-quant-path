# Pythoneers: Quantitative Finance Curriculum

## From Zero to Beginner Quantitative Analyst in 25 Workshops

Welcome to the Pythoneers Quantitative Finance Curriculum, a comprehensive, hands-on masterclass designed to take aspiring quants from their very first line of Python code to building professional, production-grade algorithmic trading systems.

### Curriculum Overview

Modern quantitative finance requires two distinct skill sets:
1. Rigorous data engineering to process, clean, cache, and align complex market and economic datasets without look-ahead bias or survivorship distortion.
2. Financial econometrics and portfolio theory to formulate predictive alpha signals, balance risk factors, and optimize capital allocations.

This curriculum bridges the gap between pure programming tutorials and academic finance theory. Across 25 structured Jupyter Notebook workshops organized into 5 progressive stages, you will build a production-ready quantitative research stack from scratch. Every workshop includes clear explanations of intuition, fully executable code examples with realistic market data, interactive practice exercises, and verified solutions.

### Curriculum Stages

#### Stage 0: Python Survival Bootcamp (6 workshops)
Designed for complete beginners with zero prior programming experience. You will master core Python syntax, control flow, functions, modular architecture, file systems, path manipulation, and debugging methodologies through practical financial examples.

#### Stage 1: Pandas Deep Dive (5 workshops)
Master the industry-standard data analysis library for tabular time series. You will learn to construct Series and DataFrames, execute fast boolean indexing, group and aggregate records, apply rolling windows and time lags, and perform relational joins across disparate datasets.

#### Stage 2: Finance Fundamentals (4 workshops)
Enter quantitative finance by downloading real-world stock market data with Yahoo Finance. You will compute arithmetic and logarithmic returns, calculate annualized volatility, construct trend-following Simple Moving Average (SMA) crossover strategies, and evaluate performance using Cumulative Return, Sharpe Ratio, Maximum Drawdown, and Win Rate.

#### Stage 3: Advanced Production Engineering (6 workshops)
Transition from single-stock analysis to institutional portfolio infrastructure. You will manage MultiIndex universes, eliminate cross-asset data leakage using grouped transformations, implement Parquet caching with exponential-backoff retry policies, mitigate survivorship bias through dynamic point-in-time constituent mapping, and align non-synchronous macroeconomic releases (Treasury yields, CPI inflation) using backward point-in-time matching.

#### Stage 4: Alpha Generation & Portfolio Optimization (4 workshops)
Develop institutional-grade factor models and portfolio construction engines. You will build and combine cross-sectional alpha factors (momentum, low-volatility anomaly, short-term reversal), apply volatility targeting and hard position limits, implement Markowitz mean-variance optimization along the Efficient Frontier, and build a complete end-to-end modular backtester (`QuantBacktester`) that orchestrates the entire quantitative pipeline.

### Workshop List

| Stage | Workshops |
| :--- | :--- |
| Stage 0 | 0.1 First Python Program, 0.2 Lists and Loops, 0.3 Dictionaries and Functions, 0.4 Conditions and Logic, 0.5 Files and Paths, 0.6 Errors and Debugging |
| Stage 1 | 1.1 Series and DataFrames, 1.2 Indexing and Selecting, 1.3 Grouping and Aggregating, 1.4 Rolling and Shifting, 1.5 Merging DataFrames |
| Stage 2 | 2.1 Fetching Stock Data, 2.2 Returns and Volatility, 2.3 SMA Strategy, 2.4 Evaluating Performance |
| Stage 3 | 3.1 MultiIndex and Universes, 3.2 GroupBy on MultiIndex, 3.3 Production Caching (Single), 3.4 Production Caching (Multi), 3.5 Survivorship Bias, 3.6 Merging Macro Data |
| Stage 4 | 4.1 Alpha Factors, 4.2 Risk Management, 4.3 Portfolio Optimization, 4.4 Capstone Backtester |

### Prerequisites

No prior programming experience is required. This curriculum starts from the absolute beginning:
- Basic computer literacy (creating folders, downloading files, using a web browser).
- High school level mathematics (percentages, fractions, basic algebra).
- A desire to understand how financial markets work through code.

### Setup Instructions

Follow these steps to set up your local development environment:

#### 1. Install Python 3.8 or Newer
Download and install the latest stable version of Python 3 from [python.org](https://www.python.org/downloads/). During installation on Windows, ensure the checkbox "Add Python to PATH" is selected. On macOS and Linux, Python is often pre-installed or easily installed via your package manager.

#### 2. Clone the Repository
Open your command line terminal and clone this repository:
```bash
git clone https://github.com/pythoneers/pythoneers-quant-path.git
cd pythoneers-quant-path
```

#### 3. Install Required Packages
Install all necessary dependencies using pip:
```bash
pip install pandas numpy matplotlib yfinance tenacity jupyter pyarrow
```

#### 4. Launch Jupyter Notebook
Start the Jupyter Notebook environment from your project folder:
```bash
jupyter notebook
```
Your default web browser will open displaying the project directory.

### How to Work Through the Material

To maximize your learning and retention, follow these guidelines:
- Work sequentially: Each workshop builds directly upon the concepts, functions, and datasets established in preceding notebooks. Do not skip stages.
- Type the code yourself: Avoid copying and pasting. Manually typing code builds muscle memory, forces you to notice syntax patterns, and deepens conceptual understanding.
- Attempt all exercises before checking solutions: Every workshop ends with interactive exercises and complete official solutions. Spend at least 15 minutes attempting each exercise independently before reviewing the solution.
- Inspect intermediate variables: Use print statements and exploratory cells to inspect the shapes, columns, and data types of intermediate DataFrames.
- Experiment with parameters: Change lookback windows, universe tickers, risk targets, and factor weights to observe how strategy behavior changes under different market conditions.

### Repository Structure

```
pythoneers-curriculum/
├── README.md
├── requirements.txt
├── Stage_0_Python_Basics/
│   ├── 00_01_First_Python_Program.ipynb
│   ├── 00_02_Lists_and_Loops.ipynb
│   ├── 00_03_Dictionaries_and_Functions.ipynb
│   ├── 00_04_Conditions_and_Logic.ipynb
│   ├── 00_05_Files_and_Paths.ipynb
│   └── 00_06_Errors_and_Debugging.ipynb
├── Stage_1_Pandas_Deep_Dive/
│   ├── 01_01_Series_and_DataFrames.ipynb
│   ├── 01_02_Indexing_and_Selecting.ipynb
│   ├── 01_03_Grouping_and_Aggregating.ipynb
│   ├── 01_04_Rolling_and_Shifting.ipynb
│   └── 01_05_Merging_DataFrames.ipynb
├── Stage_2_Finance_Fundamentals/
│   ├── 02_01_Fetching_Stock_Data.ipynb
│   ├── 02_02_Returns_and_Volatility.ipynb
│   ├── 02_03_SMA_Strategy.ipynb
│   └── 02_04_Evaluating_Performance.ipynb
├── Stage_3_Advanced_Production/
│   ├── 03_01_MultiIndex_and_Universes.ipynb
│   ├── 03_02_GroupBy_on_MultiIndex.ipynb
│   ├── 03_03_Production_Caching_Single.ipynb
│   ├── 03_04_Production_Caching_Multi.ipynb
│   ├── 03_05_Survivorship_Bias.ipynb
│   └── 03_06_Merging_Macro_Data.ipynb
└── Stage_4_Alpha_Optimization/
    ├── 04_01_Alpha_Factors.ipynb
    ├── 04_02_Risk_Management.ipynb
    ├── 04_03_Portfolio_Optimization.ipynb
    └── 04_04_Capstone_Backtester.ipynb
```

### Contributing

Contributions, feature suggestions, and educational enhancements are welcome.
If you find a typo, bug, or calculation issue:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/improvement`).
3. Commit your changes with clear, descriptive commit messages.
4. Push to your branch (`git push origin feature/improvement`).
5. Open a Pull Request detailing your enhancements.

### License

This project is licensed under the MIT License. You are free to use, modify, distribute, and build upon this curriculum for personal, educational, and commercial projects.

### Contact

For questions, community discussions, or feedback regarding the curriculum:
- GitHub Issues: Open an issue on this repository for technical questions or bug reports.
- Community Forum: Join our Pythoneers quant study group and Discord community.
- Website: Visit https://pythoneers.vercel.app/ for additional quantitative articles and video walkthroughs.

Start your journey now open 00_01_First_Python_Program.ipynb and write your first line of code!
