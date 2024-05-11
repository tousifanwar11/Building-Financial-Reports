# Building-Financial-Reports
Financial Analysis Tool for Hedge Fund Managers

This tool helps hedge fund managers analyze financial data across different industries. It leverages two key datasets, Balance_Sheet.xlsx and Income_Statement.xlsx, which contain comprehensive financial information from various companies. The tool calculates financial ratios, merges datasets, and provides insights into industry-specific financial health.

The analysis utilizes two primary datasets:
Balance_Sheet.xlsx: Contains balance sheet information for various companies. Each row represents a company's annual financial data.
Income_Statement.xlsx: Contains income statement details, structured similarly to the balance sheet data.

Both datasets include the following columns:
Company: Company's ticker symbol.
comp_type: Industry type (tech for technology, fmcg for fast-moving consumer goods, real_est for real estate).
Year: Fiscal year of the data.

Features
Data Merging: Combines data from both the balance sheet and income statement based on common keys (Year, Company, comp_type).

Ratio Calculation:
Profitability Ratio: Gross margin ratio calculated as (Total Revenue - Cost Of Goods Sold) / Total Revenue.
Leverage Ratio: Initially calculated as Total Liabilities / Total Stockholder Equity. Updated to Total Assets / Total Stockholder Equity for a specific analysis.
Industry Comparison: Uses pivot tables to compare average ratios across industries, identifying which industry has the lowest average profitability and highest leverage.

Usage
Data Input: Place your Balance_Sheet.xlsx and Income_Statement.xlsx files in the data/ directory.
Script Execution: Run the Python script to perform the analysis.

Output Interpretation:
Check the console output for pivot tables showing average profitability and leverage ratios by industry.
Review scatter plots to examine the relationship between leverage and profitability in the real estate sector.
Dependencies
Ensure you have the following Python libraries installed:

numpy
pandas
seaborn

You can install them using pip:
pip install numpy pandas seaborn

Example Analysis Output
The script will output data like the following:
Pivot table of average profitability ratios by industry.
Pivot table of average leverage ratios by industry.
Scatter plot illustrating the correlation between leverage and profitability in the real estate industry.
