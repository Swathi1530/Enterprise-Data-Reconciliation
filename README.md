# Enterprise Data Reconciliation & CFO Dashboard

## Project Overview

The **Enterprise Data Reconciliation & CFO Dashboard** is a Python-based data processing and financial analytics project. It combines SQL database extraction, server log cleaning, foreign exchange rate integration, and revenue visualization to support financial analysis and reporting.

## Objectives

- Extract users based on their latest account status using SQL.
- Clean unstructured server logs using Regular Expressions and Pandas.
- Integrate transaction data with daily exchange rates.
- Convert Euro transaction values into US Dollar revenue.
- Visualize monthly revenue trends and identify the top 5 most valuable customers.

## Technologies Used

- **Python** — Data processing and analysis
- **SQL / SQLite** — Database querying and user status extraction
- **Pandas** — Data cleaning, transformation, and merging
- **Regular Expressions (Regex)** — Extracting structured information from server logs
- **Matplotlib** — Data visualization
- **Seaborn** — Data visualization support
- **Jupyter Notebook** — Interactive development and analysis
- **Git & GitHub** — Version control and project hosting

## Project Workflow

### Phase 1: SQL Extraction
Retrieve the latest status for each user using SQL window functions and filter users whose latest status is `Active`.

### Phase 2: Regex & Data Cleaning
Read server logs, remove records containing `ERROR`, and extract transaction dates, user IDs, product IDs, and Euro values.

### Phase 3: Financial Reconciliation
Load daily exchange rates, fill missing dates using forward-fill, merge exchange rates with transactions, join active user data, and calculate USD revenue.

### Phase 4: Aggregation & CFO Dashboard
Calculate total USD revenue by month, identify the top 5 customers by total USD spending, and create charts to visualize the results.

## Project Files

- `Student_work_file (1) (1).ipynb` — Main notebook containing the project workflow.
- `daily_exchange_rates (1) (1).csv` — Daily currency exchange rate data.
- `enterprise_database (1) (1).db` — SQLite database used for user data extraction.
- `server_logs (1) (1).txt` — Raw server log data for cleaning and transaction extraction.

## How to Run the Project

1. Install Python and Visual Studio Code.
2. Install the required Python libraries:

   ```bash
   python -m pip install pandas matplotlib seaborn
   ```

3. Clone or download this repository.
4. Open the project folder in Visual Studio Code.
5. Open the Jupyter Notebook and select a Python kernel.
6. Execute the notebook cells in order, from Phase 1 through Phase 4.
7. Review the extracted data, reconciliation results, summary tables, and dashboard charts.

## Expected Outputs

- A DataFrame containing users whose latest status is Active.
- Cleaned transaction data extracted from server logs.
- A reconciled dataset containing exchange rates and USD revenue.
- Monthly USD revenue summaries.
- A Top 5 customers summary and corresponding visualizations.

## Skills Demonstrated

SQL querying, data wrangling, Regular Expressions, financial data reconciliation, currency conversion, Pandas data manipulation, data visualization, and version control.

GitHub: [Swathi1530](https://github.com/Swathi1530)

Project Repository: [Enterprise Data Reconciliation](https://github.com/Swathi1530/Enterprise-Data-Reconciliation)
