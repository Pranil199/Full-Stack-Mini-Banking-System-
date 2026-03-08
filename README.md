# Full-Stack-Mini-Banking-System
## Overview
This project is an end-to-end, Object-Oriented banking simulation designed to demonstrate core software engineering and data analytics principles. 

It moves beyond basic scripts by implementing a persistent SQLite database for transaction logging, utilizing statistical anomaly detection (3-Sigma rule) for fraud prevention, and wrapping the backend logic in an interactive Streamlit web dashboard. It serves as a practical bridge between financial domain logic and modern data engineering pipelines.

## Key Features
* **Robust OOP Architecture:** Utilizes Encapsulation to protect core account balances, and Inheritance to implement specialized `SavingsAccount` (interest accrual) and `CurrentAccount` (overdraft limits) classes.
* **Statistical Fraud Detection:** Integrates a Numpy-powered Z-score calculator to automatically flag anomalous withdrawals that deviate significantly (3 standard deviations) from a user's historical spending behavior.
* **Persistent SQLite Database:** Replaces volatile in-memory storage with a lightweight, relational database. Transactions are securely logged with ACID compliance principles in mind.
* **Data-Ready Statements:** Seamlessly queries SQL tables and transforms them into Pandas DataFrames, making the transaction history instantly ready for BI tools or visualization.
* **Interactive Streamlit UI:** Features a full frontend web dashboard allowing users to execute transactions and view real-time balance metrics and time-series charts.

## Tech Stack
* **Backend:** Python (OOP), SQLite3
* **Data Processing & Analytics:** Pandas, NumPy
* **Frontend:** Streamlit

## Getting Started

### Prerequisites
Install the required standard data science libraries:
```bash
pip install pandas numpy streamlit
