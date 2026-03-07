# Ramesh Shrestha

**Data Scientist — Sydney, Australia**

I build production-grade machine learning systems end-to-end: feature engineering on large-scale datasets, model training and calibration, real-time API deployment, and monitoring in production. My work spans fraud intelligence, healthcare AI, financial risk, and customer analytics.

[LinkedIn](https://www.linkedin.com/in/rameshsta/) · [Email](mailto:shrestha.ramesh000@gmail.com)

---

## Featured Work

### FraudSentinel — Proactive Payment Fraud Intelligence

Early-warning fraud detection system built on 590,540 real IEEE-CIS payment transactions. The system ranks every transaction by the probability that the originating entity will commit fraud within the next 72 hours — before the loss materialises.

| Metric | Value |
|--------|-------|
| Fraud captured in top 8% reviewed | 37.8% |
| Operational lift at top 8% | 4.7× |
| Lift in top 3% (High risk band) | 7× |
| Precision in High risk band | 19.5% |
| AUC-PR improvement over no-skill baseline | 3.5× |
| API inference latency | < 20 ms |

**Architecture:** PyTorch MLP with hashed entity embeddings · temperature-scaled calibration · entity velocity features · fraud campaign propagation signals · 72-hour early-warning label

**MLOps:** MLflow experiment tracking · SHAP LinearExplainer · Evidently AI drift monitoring · DVC pipeline · Docker · 50 pytest unit tests · FastAPI scoring API

[GitHub](https://github.com/RameshSTA/fraudsentinel) · [Live Drift Dashboard](https://rameshsta.github.io/fraudsentinel/reports/drift_monitoring_report.html)

---

### OptiHealth — Clinical Decision Support System

30-day hospital readmission risk platform with XAI. XGBoost risk prediction with SHAP patient-level attributions and Prophet 7–30 day census forecasting. Full-stack deployment on Vercel / Render / NeonTech with sub-100ms inference and TGA-compliant audit governance. Projected 15–20% reduction in preventable readmissions.

[GitHub](https://github.com/RameshSTA/OptiHealth-Platform) · [Live Demo](https://optihealth-platform.vercel.app/)

---

### ConnectIntelligence — Real-Time Predictive Retention Engine

Member churn prediction for the Australian Superannuation sector. XGBoost achieving 0.86 weighted accuracy, deployed as a real-time FastAPI + Docker API (< 200 ms end-to-end) with SHAP explainability and K-Means behavioural segmentation into four actionable risk personas.

[GitHub](https://github.com/RameshSTA/ConnectIntelligence)

---

### Customer Lifetime Value Forecasting

Cohort-based CLV prediction system. Random Forest AUC = 0.831, Spearman ρ = 0.57. Monte Carlo simulation projects 10×–26× ROI (90% CI). Customers segmented into five actionable groups for long-horizon retention strategy and investment prioritisation. Built with SHAP, MLflow, and PuLP/CBC optimisation.

[GitHub](https://github.com/RameshSTA/clv-long-term-optimization)

---

### FinGraph-ASX — Neuro-Symbolic GraphRAG Intelligence Engine

Agentic GraphRAG system over ASX financial reports. Built with LlamaIndex, Neo4j, and Groq. Reduces financial due diligence review time by 40%, cuts retrieval latency by 40%, and grounds every LLM response in source-linked evidence from annual reports to minimise hallucinations.

[GitHub](https://github.com/RameshSTA/FinGraph-ASX-GraphRAG-Engine)

---

## Technical Skills

| Category | Tools |
|----------|-------|
| Machine Learning | PyTorch · XGBoost · LightGBM · scikit-learn · SHAP · Prophet · LSTM |
| MLOps | MLflow · DVC · Docker · GitHub Actions · Evidently AI · FastAPI |
| Data Engineering | Databricks · PySpark · Azure Data Factory · pandas · SQL · ETL |
| Cloud and Databases | Azure · AWS · Google Cloud · Snowflake · Neo4j · PostgreSQL |
| Visualisation | Power BI · Tableau · Plotly · Streamlit |
| Languages | Python · SQL · PL-SQL · Bash |

---

## Experience

**Associate Consultant — ERP Data Developer** · PM-Partners · Sydney · Feb 2026 – Present

**Data Science and ML Intern** · Hightech Mastermind Pty Ltd · Sydney · Feb 2025 – Apr 2025

---

## Education and Certifications

**Bachelor of Software Engineering (Data Science and AI)** · Torrens University Australia · 2021–2024

**Professional Year Program (IT)** · QIBA · 2024–2025

Google Advanced Data Analytics Professional Certificate · 2025

Deep Learning Specialisation — DeepLearning.AI · 2025

Machine Learning Specialisation — Stanford University / DeepLearning.AI · 2024

---

Full working rights in Australia. Open to Data Scientist and ML Engineer roles.
