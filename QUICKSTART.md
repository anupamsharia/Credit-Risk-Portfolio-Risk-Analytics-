# Beginner's Quickstart Guide 🚀

Welcome to the **Credit Risk & Portfolio Risk Analytics** project! Whether you are a beginner, student, or hiring manager, this guide will help you run and update everything in just a few minutes.

---

## ⚡ Option 1: Quickest Way — Open in Any Browser (No Setup Required!)

You don't need to install Python or SQL to view the interactive portfolio and results:

1. **Portfolio Homepage:** Double-click [`index.html`](index.html) in your file explorer.
2. **Executive Dashboard:** Double-click [`dashboard/executive_dashboard.html`](dashboard/executive_dashboard.html).
3. **Online GitHub Pages:** If you activated GitHub Pages, open:
   ```
   https://anupamsharia.github.io/Credit-Risk-Portfolio-Risk-Analytics-/
   ```

---

## 🐍 Option 2: Running the Python Jupyter Notebooks

### Step 1: Install Requirements
Open your terminal (PowerShell, Command Prompt, or Terminal) in this folder and run:

```bash
pip install -r requirements.txt
```

### Step 2: Launch Jupyter
```bash
jupyter notebook
```

### Step 3: Open and Run Notebooks
- **Credit Risk Model:** Navigate to `flagship-credit-risk/Credit_Risk_Default_Analytics.ipynb` and click **"Run All Cells"**.
- **Portfolio Risk Forecasting:** Navigate to `portfolio-risk-forecasting/Portfolio_Risk_Forecasting.ipynb` and click **"Run All Cells"**.

> **Tip for Beginners:** All exported chart PNGs are automatically saved in the respective `outputs/` folders.

---

## 🗄️ Option 3: Running the SQL Analytics Queries

1. Open any SQL client (such as **DBeaver**, **pgAdmin**, **VS Code with SQL Tools**, or **MySQL Workbench**).
2. Open [`sql/Advanced_Financial_Analytics.sql`](sql/Advanced_Financial_Analytics.sql).
3. The script contains 6 modular queries with test schema creation (`customers`, `accounts`, `transactions`) and sample data generation.
4. Highlight and execute any section from 1 to 6 to see:
   - Windowed running overdraft detection
   - Cohort retention triangles
   - RFM customer segmentation tiers
   - Rolling z-score fraud detection
   - Month-over-month revenue trends
   - Customer Lifetime Value (CLV)

---

## 📊 Option 4: Exploring the Excel Financial Model

1. Open [`excel/Financial_KPI_Dashboard.xlsx`](excel/Financial_KPI_Dashboard.xlsx) in Microsoft Excel, Google Sheets, or LibreOffice.
2. Explore the 4 tabs:
   - **`Transactions`**: 420 ledger entries across 8 expense categories and 2 revenue streams.
   - **`Assumptions`**: Editable budget inputs in blue text. Change any number here, and all downstream charts update automatically!
   - **`Summary`**: Live formulas (`SUMIFS`, `INDEX/MATCH`) with zero formula errors.
   - **`Dashboard`**: High-level KPI cards and native variance charts.

---

## 📁 Pre-Generated Datasets (in `data/`)

If you want to build Power BI dashboards, Tableau stories, or custom machine learning models without running notebooks, pre-generated datasets are ready:
- `data/credit_risk_loans_data.csv`: 10,000 calibrated loan records with FICO scores, DTI, delinquency history, and default labels.
- `data/multi_asset_daily_returns.csv`: 3 years of daily log returns for US Equities, EM Equities, Bonds, Gold, and Bitcoin.

---

## ✏️ How a Beginner Can Update / Customize This Project

1. **Change Author Details:**
   - Search & replace `Anupam Sharia` and your LinkedIn handle in `README.md`, `index.html`, and `dashboard/executive_dashboard.html`.
2. **Swap With Real Data:**
   - In `flagship-credit-risk/Credit_Risk_Default_Analytics.ipynb`, replace the `generate_loan_portfolio()` function with:
     ```python
     df = pd.read_csv("your_real_loan_tape.csv")
     ```
   - The rest of the statistical tests and machine learning pipelines will work automatically!
3. **Commit & Push to GitHub:**
   ```bash
   git add .
   git commit -m "Update portfolio details"
   git push origin main
   ```
