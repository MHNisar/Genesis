# Genesis
# Portfolio Longevity in Contemporary Markets
This model uses historical market data from the US (1928-2024) to project the longevity of a portfolio under 3000 stochastic return sequences, providing a clear visual of potential outcomes.

# Features
Historical Data Analysis: Leverages nearly a century of real-market data for stocks, bonds, and inflation.

Stochastic Modeling: Randomly samples historical years to generate realistic, non-linear return sequences.

Dynamic Parameters: Easily adjust starting balance, asset allocation, withdrawal rate, and data range.

Inflation-Adjusted Withdrawals: Models the real-world impact of inflation on annual spending power.

Comprehensive Results: Outputs a success rate (Pass Rate) and a percentile analysis of terminal wealth.

# Structure:
The model is contained within a single Excel workbook (.xlsm) with the following structure

Historical:

This sheet houses the foundational dataset for the simulation. It contains annual historical returns for stocks, bonds, and inflation, along with the calculated correlation between asset classes for each year. The model samples randomly from this data to generate stochastic return sequences.

Control:

This sheet contains all user-defined parameters to run the simulation, including the starting portfolio balance, asset allocation (stock/bond weights), withdrawal rate, and the range of historical years to sample data from.         

r1:

The core computational sheet. It runs a single, randomized 30-year retirement scenario by drawing sequences of returns and inflation from the historical data. It calculates the annual portfolio value, withdrawals, and adjusts for inflation, providing a detailed look at one potential outcome.

Simulations:

This sheet summarizes the outcomes from running thousands of simulations.

# Installation & Usage
1. Download the Repository: Click the Code button and select Download ZIP. Extract the files to a folder on your computer.

2. Enable Macros: This model uses VBA to run the Monte Carlo simulations.

    -> Right-click on the downloaded Excel file (Genesis.xlsm).

    -> Select Properties.

    -> In the General tab, check the Unblock box at the bottom (if present).

    -> Click OK.

3. Open the File: Open the workbook in Microsoft Excel.

4. Enable Content: When prompted, click "Enable Content" to allow the macros to run.

5. Configure Your Simulation:

    -> Go to the Control sheet.

    -> Adjust the parameters (Starting Balance, Withdrawal Rate, Stock/Bond Allocation, etc.) to your liking.

6. Run the Simulation:

    -> Press the "Refresh Simulations" button (this button is triggered by a VBA macro).

    -> The model will run thousands of iterations. Please be patient; this may take a moment.

7. View Results:

    -> The Control sheet will populate with the aggregate success rate and terminal wealth statistics.
   
    -> The r1 sheet will show the path of a single, randomly selected simulation for detailed inspection.

# Interpreting the Results
Pass Rate: The percentage of simulated 30-year periods where the portfolio did not deplete to zero.

Terminal Wealth: The value of the portfolio at the end of 30 years, before the final withdrawal.

    Median: The middle value of all outcomes. Half of the outcomes were higher, half were lower.

    Percentiles (5th, 25th, 75th, 95th): Show the range of possible outcomes. The 5th percentile is a particularly important worst-case scenario.

A "Success" is defined as a portfolio value greater than $0 at the end of the 30-year period.

# Limitations & Disclaimers
This is a simplified model for academic and illustrative purposes. Key limitations include:

Historical Data Bias: The simulation is based solely on U.S. historical data, which has been favorable compared to global markets. Past performance is not indicative of future results.

Fixed Withdrawals: The model uses a rigid, inflation-adjusted withdrawal rule. Real retirees often adjust spending based on portfolio performance.

Taxes and Fees: Returns are pre-tax and do not account for management fees, transaction costs, or taxes on dividends and capital gains, which can significantly impact net returns.

Asset Class Simplification: Uses "Stocks" and "Bonds" as broad proxies. Does not account for sub-asset classes (e.g., international stocks, corporate vs. government bonds).

Non-Stationary Relationships: Assumes the historical relationship (correlation) between stocks and bonds is constant, which may not hold in future regimes (e.g., rising inflation environments).

Disclaimer: This is not financial advice. Please consult with a qualified financial professional before making any decisions based on this model.


