##✅ 1. Architecture Diagram Description
#AI‑Powered Telecom Churn Prediction Architecture
#1. Data Sources
CRM system (customer profiles, tenure, demographics)
Billing system (payment history, monthly charges)
Network usage logs (data usage, call drops)
Support ticketing system (complaints, issue frequency)

#2. Ingestion Layer
Batch ETL jobs (daily customer data refresh)
API connectors (billing + CRM sync)
Data validation scripts

#3. Storage Layer
Data Lake (Raw Zone)
    Raw usage logs
    Billing records
    Support tickets
Feature Store (Processed Zone)
    Cleaned, engineered features
    Normalized numeric fields
Model Registry
    Versioned FFNN models
    Metadata + evaluation metrics

4. AI / Processing Layer
Feature engineering pipeline
Feed-forward neural network (FFNN) training
Model evaluation (AUC, recall, F1)
Batch prediction service (daily churn scoring)

5. Consumption Layer
Retention dashboard (high-risk customers)
Alerts to CRM (flag customers with churn probability > threshold)
Marketing campaign engine (personalized offers)
Human review workflow (retention agents validate predictions)

6. Monitoring & Responsible AI
Drift detection
Fairness checks
Weekly performance reports
Human-in-the-loop overrides


