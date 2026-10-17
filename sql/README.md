# Advanced Financial & Risk Analytics (SQL)

Part of the **Credit Risk & Portfolio Risk Analytics** portfolio by **Anupam Sharia**.

---

## 📌 Project Overview
Demonstrates six advanced SQL query patterns on a realistic 3-table banking schema (`customers`, `accounts`, `transactions`) addressing institutional analytics and risk challenges.

### Queries Included:
1. **Running-Balance Overdraft Detection:** Windowed `SUM() OVER(PARTITION BY ... ORDER BY ...)` catches intra-month overdraft dips that month-end balances conceal.
2. **Monthly Cohort Retention:** Triangular growth retention report computed on months-since-signup.
3. **RFM Customer Segmentation:** `NTILE()`-based Recency, Frequency, and Monetary scoring tiers.
4. **Fraud / Anomaly Detection:** Account-level rolling z-scores paired with a `LATERAL` join transaction velocity check.
5. **Month-over-Month Net Revenue:** Windowed moving averages and `LAG()` functions for board reporting.
6. **Customer Lifetime Value (CLV) & Channel ROI:** 12-month proxy CLV using `FILTER` and `PERCENTILE_CONT(0.50)` (median) to prevent whale skew.

---

## 🚀 How to Run for Beginners
- Compatible with **PostgreSQL 14+**, **Snowflake**, **BigQuery**, or any SQL client (DBeaver, pgAdmin, DataGrip).
- Dialect porting notes are provided inline for MySQL and SQL Server.
- Simply run `Advanced_Financial_Analytics.sql` sequentially to create tables, populate mock data, and test each query pattern.
