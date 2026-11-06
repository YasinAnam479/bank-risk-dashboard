# Bank Transaction Risk Dashboard

An end-to-end data project: ETL pipeline, normalized SQLite data warehouse,
rule-based risk detection, ML anomaly detection, and a Streamlit dashboard.

## Features
- ETL pipeline (Python/pandas) that builds a normalized warehouse
- Risk rules: HIGH_VALUE, VELOCITY, ODD_HOUR, plus customer-profile flags
- Isolation Forest model to find anomalies the rules miss
- Interactive Streamlit dashboard with filters and 4 tabs

## Tech stack
Python, pandas, SQLite, scikit-learn, Plotly, Streamlit

## How to run
1. Install packages: `pip install streamlit plotly pandas scikit-learn`
2. Put the Bank Marketing CSV in the project folder as `test.csv`
3. Build the database: `python bank_etl_v2.py`
4. Run the ML model: `python ml_risk.py`
5. Launch the dashboard: `streamlit run dashboard.py`

## Data
Customer profiles come from the UCI Bank Marketing dataset.
Transactions are synthetic.
