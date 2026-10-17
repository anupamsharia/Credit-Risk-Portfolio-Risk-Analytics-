# Multi-Asset Portfolio Risk & Volatility Forecasting

Part of the **Credit Risk & Portfolio Risk Analytics** portfolio by **Anupam Sharia**.

---

## 📌 Project Overview
A quantitative risk and allocation engine evaluating a 5-asset portfolio (US Equities, Emerging Market Equities, 10-Year Bonds, Gold, and Bitcoin) across 756 simulated trading days.

### Key Highlights:
- **Mean-Variance Optimization:** Diagnosed textbook Markowitz estimation error instability (unconstrained solve allocated 100% to Bitcoin) and introduced a practitioner-ready 35% position cap.
- **Value-at-Risk (VaR) & CVaR:** Evaluated 1-day and 10-day 95%/99% VaR using Historical, Parametric, and Monte Carlo (8,000 runs) methodologies.
- **Stress Testing:** Quantified risk under a correlation crisis scenario (VaR surges by ~14%).
- **Volatility Forecasting:** Implemented EWMA (RiskMetrics $\lambda = 0.94$).

---

## 📂 Folder Structure
- `Portfolio_Risk_Forecasting.ipynb`: Complete executable pipeline.
- `outputs/`: Exported chart PNGs:
  - `01_cumulative_growth.png`
  - `02_correlation_matrix.png`
  - `03_efficient_frontier.png`
  - `04_ewma_volatility.png`
  - `05_drawdown.png`
  - `06_stress_test.png`

---

## 🚀 How to Run for Beginners
```bash
pip install -r ../requirements.txt
jupyter notebook Portfolio_Risk_Forecasting.ipynb
```
Select **Kernel -> Restart & Run All** to reproduce all figures and VaR calculations.
