<div align="center">

# Ramesh Shrestha

**Data Scientist — Sydney, Australia**

Building production-grade ML systems that ship to real environments and drive measurable decisions.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-rameshsta-0077b5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rameshsta/)
[![Email](https://img.shields.io/badge/Email-shrestha.ramesh000@gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:shrestha.ramesh000@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/RameshSTA?style=flat-square&logo=github&label=Follow)](https://github.com/RameshSTA)

</div>

---

I own the full ML lifecycle — feature engineering on large-scale datasets, training and calibrating models, deploying real-time APIs, and monitoring them in production. I work across fraud intelligence, customer analytics, financial risk, and healthcare AI. Currently working as an Associate Consultant at PM-Partners in Sydney while building production ML projects independently.

**Core stack:** Python · PyTorch · XGBoost · scikit-learn · FastAPI · Docker · MLflow · SHAP · Databricks · Azure · SQL

---

## Projects

### FraudSentinel — Proactive Payment Fraud Intelligence

Early-warning fraud detection system built on 590,540 real IEEE-CIS payment transactions. Ranks every transaction by the probability that the originating entity will commit fraud within the next 72 hours — capturing **37.6% of all fraud** by reviewing only the top 8% of traffic (**4.7× operational lift** over random review).

The core design shift: instead of detecting fraud after it happens, the system predicts it before the loss materialises. A 72-hour early-warning label, entity velocity features, behavioural baseline deviation, and fraud campaign propagation signals power a Torch MLP with hashed entity embeddings and temperature-scaled probability calibration.

**Stack:** PyTorch · entity embeddings · temperature scaling · FastAPI · MLflow · SHAP · Evidently AI · DVC · Docker · 50 pytest unit tests

| Metric | Value |
|--------|-------|
| Operational lift at top 8% | 4.7× |
| Fraud captured in top 8% reviewed | 37.6% |
| Precision in High risk band (top 1–3%) | 19.1% |
| AUC-PR improvement over no-skill baseline | 3.5× |
| API inference latency | <20ms |

[![GitHub](https://img.shields.io/badge/GitHub-fraudsentinel-181717?style=flat-square&logo=github)](https://github.com/RameshSTA/fraudsentinel)
[![Live Drift Report](https://img.shields.io/badge/Live_Report-Interactive_Drift_Dashboard-orange?style=flat-square&logo=plotly)](https://rameshsta.github.io/fraudsentinel/reports/drift_monitoring_report.html)

---

### ConnectIntelligence — Real-Time Predictive Retention Engine

XGBoost-powered member churn prediction for the Australian Superannuation sector, achieving 0.86 weighted accuracy. Deployed as a production real-time API (FastAPI + Docker, <200ms end-to-end) with SHAP explainability and K-Means behavioural segmentation into four high-risk personas.

[![GitHub](https://img.shields.io/badge/GitHub-ConnectIntelligence-181717?style=flat-square&logo=github)](https://github.com/RameshSTA/ConnectIntelligence)

---

### OptiHealth — Clinical Decision Support System

XAI-powered 30-day hospital readmission risk platform. XGBoost risk prediction + SHAP attributions + Prophet 7–30 day census forecasting. Full-stack deployment (Vercel / Render / NeonTech) with sub-100ms inference and TGA-compliant audit governance. Projected 15–20% reduction in preventable readmissions.

[![GitHub](https://img.shields.io/badge/GitHub-OptiHealth--Platform-181717?style=flat-square&logo=github)](https://github.com/RameshSTA/OptiHealth-Platform)
[![Live Demo](https://img.shields.io/badge/Live-optihealth--platform.vercel.app-00c7b7?style=flat-square)](https://optihealth-platform.vercel.app/)

---

### Customer Lifetime Value Forecasting & Optimisation

Cohort-based CLV prediction system achieving 20% improvement in forecasting precision over baseline. Segments customers into five actionable groups for long-horizon retention strategy and investment prioritisation.

[![GitHub](https://img.shields.io/badge/GitHub-clv--long--term--optimization-181717?style=flat-square&logo=github)](https://github.com/RameshSTA/clv-long-term-optimization)

---

### FinGraph-ASX — Neuro-Symbolic GraphRAG Intelligence Engine

Agentic GraphRAG system over ASX financial reports using LlamaIndex, Neo4j, and Groq. Cuts financial due diligence review time by 40%, reduces retrieval latency by 40%, and grounds every LLM response in source-linked evidence from annual reports to minimise hallucinations.

[![GitHub](https://img.shields.io/badge/GitHub-FinGraph--ASX--GraphRAG--Engine-181717?style=flat-square&logo=github)](https://github.com/RameshSTA/FinGraph-ASX-GraphRAG-Engine)

---

## Technical Skills

| Category | Tools |
|---|---|
| Machine Learning | PyTorch · XGBoost · LightGBM · scikit-learn · SHAP · Prophet · LSTM |
| MLOps | MLflow · DVC · Docker · GitHub Actions · Evidently AI · FastAPI |
| Data Engineering | Databricks · PySpark · Azure Data Factory · pandas · SQL · ETL |
| Cloud & Databases | Azure · AWS · Google Cloud · Snowflake · Neo4j · PostgreSQL |
| Visualisation | Power BI · Tableau · Plotly · Streamlit |
| Languages | Python · SQL · PL-SQL · Bash |

---

## Experience

**Associate Consultant — ERP Data Developer** · PM-Partners · Sydney · Feb 2026 – Present

**Data Science & ML Intern** · Hightech Mastermind Pty Ltd · Sydney · Feb 2025 – Apr 2025

---

## Education

**Bachelor of Software Engineering (Data Science & AI)** · Torrens University Australia · 2021–2024

**Professional Year Program (IT)** · QIBA · 2024–2025

---

## Certifications

Google Advanced Data Analytics Professional Certificate · 2025

Deep Learning Specialisation — DeepLearning.AI · 2025

Machine Learning Specialisation — Stanford University / DeepLearning.AI · 2024

---

<div align="center">

Full working rights in Australia · Open to Data Scientist and ML Engineer roles

</div>
