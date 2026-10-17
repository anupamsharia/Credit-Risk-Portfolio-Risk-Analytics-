# Credit Risk & Loan Default Analytics

Part of the **Credit Risk & Portfolio Risk Analytics** portfolio by **Anupam Sharia**.

---

## 📌 Project Overview
Evaluates whether a calibrated machine learning scoring model can replace a retail bank's legacy underwriting rule (*"decline loan if credit score ≤ 620"*), and quantifies the expected portfolio profit impact.

### Key Questions Answered:
1. Which borrower attributes statistically predict default vs. merely correlate?
2. Does Gradient Boosting outperform Random Forest and Logistic Regression on ROC-AUC and PR-AUC?
3. What is the optimal probability cutoff threshold to balance commercial approval volume against loan charge-offs?
4. What is the net dollar value of implementing model-driven decisioning?

---

## 📂 Folder Structure
- `Credit_Risk_Default_Analytics.ipynb`: The end-to-end Jupyter Notebook pipeline (Data calibration, EDA, Welch's t-test, Chi-square, modeling, threshold optimization, and financial impact).
- `outputs/`: High-resolution exported charts:
  - `01_class_balance.png`
  - `02_risk_driver_distributions.png`
  - `03_correlation_heatmap.png`
  - `04_roc_comparison.png`
  - `05_feature_importance.png`
  - `06_profit_curve.png`

---

## 🚀 How to Run for Beginners
```bash
pip install -r ../requirements.txt
jupyter notebook Credit_Risk_Default_Analytics.ipynb
```
Select **Kernel -> Restart & Run All** to execute all statistical tests and generate all figures.
