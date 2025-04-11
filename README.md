### A Replication of *Quality Minus Junk*

This project replicates the Quality Minus Junk (QMJ) factor following Asness, Frazzini, and Pedersen's methodology. It covers US and global equities from December 2016 to January 2024, examining profitability, growth, safety, and the quality effect on stock prices and excess returns.

## Data Sources

The project relies on the following datasets:

- **Global Stock Returns and Characteristics Dataset**  
  Provided by Wharton Research Data Services (WRDS). This includes firm-level fundamentals and monthly stock return data across multiple countries.

- **Factor Performance Data**  
  Sourced from the Kenneth R. French Data Library.

Make sure the following files are saved in the appropriate project directory:

- `data.csv` — stock characteristics dataset  
- `ff.xlsx` — Fama-French factor returns

## Execution

Run the scripts in `code.ipynb`. We used Python 3.12.4. You can "Run All" cells to reproduce the analysis, but make sure to specify the correct path to your data files first.

### Steps:

1. **Specify** the correct path to the data files in the "1) Cleaning Data" section.
2. **Load** `data.csv`.
3. **Clean** the data: select relevant columns, remove missing values and outliers, and filter by selected countries.
4. **Display** summary statistics for Countries and Industries.
5. **Perform persistence analysis** on quality and its components (for Figure 1).
6. **Skip Figure 2 visualization initially**, as it is shown at the end in section 6.
7. **Load** `ff.xlsx` and evaluate quality deciles (Figure 3).
8. **Compute and evaluate** the QMJ factor and its components (Figure 4).
9. **Plot** cumulative returns of US and global samples (section 5).
10. **Analyze the price of quality** (final Figure 2 visualization).
11. **Export results** to Excel for further visualization.  
    - *Note: The export code is included but commented out using `#` to avoid automatic file saving unless needed.*
