## Financial Transaction Fraud Detection (AI CUP 2025)

This project builds an **account-level fraud detection system** using large-scale transaction data, 
with a focus on **behavioral feature engineering** and **risk-oriented visualization**.

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
   - Power BI risk dashboards

### Repository Structure
- `src/` : Production-style feature engineering & model training scripts
- `notebooks/` : Exploratory analysis and experiment tracking
- `powerbi/` : Risk dashboard design (pbix + screenshots)

### Visualization (Power BI)
The Power BI dashboard includes:
- Overall transaction risk overview
- High-risk account behavior comparison (Top30 vs population)
- Single-account behavioral drill-down

Due to data sensitivity and platform constraints, only static screenshots are provided.

### Notes
This project emphasizes **practical fraud modeling stability under highly imbalanced data**, 
and focuses on making model outputs interpretable and usable in real-world monitoring scenarios.

