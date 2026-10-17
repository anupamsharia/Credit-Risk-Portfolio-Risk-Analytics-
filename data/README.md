# Data Directory

This folder contains pre-generated CSV datasets calibrated for institutional finance, credit scoring, and portfolio risk analysis.

---

## 1. `credit_risk_loans_data.csv`
- **Rows:** 10,000 personal loans
- **Columns (15):**
  - `loan_id`: Unique loan identifier (e.g., `L100000`)
  - `credit_score`: Calibrated FICO-like credit score (300 to 850)
  - `annual_income`: Borrower annual income in USD
  - `employment_years`: Borrower employment tenure in years
  - `loan_amount`: Amount borrowed in USD
  - `loan_term_months`: Loan duration (36 or 60 months)
  - `interest_rate_pct`: Annual percentage interest rate
  - `dti_ratio`: Debt-to-income ratio (0.01 to 0.85)
  - `revolving_utilization`: Credit card revolving line utilization (0.0 to 1.0)
  - `open_accounts`: Number of active credit accounts
  - `delinquencies_2yr`: Number of 30+ day delinquencies in the past 2 years
  - `home_ownership`: `RENT`, `MORTGAGE`, or `OWN`
  - `loan_purpose`: `debt_consolidation`, `credit_card`, `home_improvement`, `major_purchase`, `medical`, `other`
  - `loan_to_income`: Ratio of loan amount to annual income
  - `defaulted`: Target variable (1 = default, 0 = repaid)

---

## 2. `multi_asset_daily_returns.csv`
- **Rows:** 756 business trading days (~3 years)
- **Columns (5 Asset Classes):**
  - `US_Equities`: S&P 500 proxy daily log returns
  - `EM_Equities`: Emerging Market equities daily log returns
  - `Bonds`: 10-Year Treasury bond proxy daily log returns
  - `Gold`: Gold commodity daily log returns
  - `Bitcoin`: Cryptocurrency daily log returns

---

## 💡 How a Beginner Can Use These Files:
- **Excel / Google Sheets:** Open `.csv` files directly to filter, pivot, and chart data.
- **Power BI / Tableau:** Import `credit_risk_loans_data.csv` to build interactive credit risk dashboards.
- **Python / Pandas:**
  ```python
  import pandas as pd
  df = pd.read_csv("data/credit_risk_loans_data.csv")
  print(df.head())
  ```
