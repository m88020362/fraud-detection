## Financial Transaction Fraud Detection (AI CUP 2025)

This project builds an **account-level fraud detection system** using large-scale transaction data, 
with a focus on **behavioral feature engineering** and **risk-oriented visualization**.

Due to competition constraints and data sensitivity, this repository shares analysis logic, modeling approach, and visualization results, rather than full production data or dashboards.
### Pipeline Overview
1. Raw transaction cleaning & normalization (multi-currency → TWD)
2. Account-level behavioral feature engineering
   - Temporal patterns (night activity, entropy)
   - Amount dynamics (repeat amount ratio, drift)
   - Counterparty concentration & network features
3. Imbalanced classification with LightGBM
   - Optuna hyperparameter tuning
   - Threshold optimization based on F1
4. Risk output & visualization
   - Account risk scores
   - Top-N high-risk concentration analysis
   - Power BI–based risk dashboards (screenshots only)

### Visualization (Power BI)
The Power BI dashboard includes:
- Overall transaction risk overview
- High-risk account behavior comparison (Top30 vs population)
- Single-account behavioral drill-down

Due to pbix file size limitations and data sensitivity, the Power BI source file is not included.
Only static dashboard screenshots are provided for demonstration and discussion purposes.

### Data Availability
- The original transaction data is provided by AI CUP 2025 and is not publicly shareable
- No raw transaction or label data is included in this repository
- All analysis results shown are derived from competition-provided datasets under usage restrictions



