<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0F2B5B&height=160&section=header&text=Ramesh%20Shrestha&fontSize=44&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Data%20Scientist%20%C2%B7%20ML%20Engineer%20%C2%B7%20Sydney%2C%20Australia&descAlignY=62&descSize=17" width="100%"/>
</div>

<div align="center">
  <a href="https://linkedin.com/in/rameshsta">
    <img src="https://img.shields.io/badge/LinkedIn-rameshsta-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;
  <a href="mailto:shrestha.ramesh000@gmail.com">
    <img src="https://img.shields.io/badge/Email-shrestha.ramesh000%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white"/>
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=RameshSTA&style=flat-square&color=0F2B5B&label=Profile+Views"/>
</div>

<br/>

Production-focused Applied Data Scientist with end-to-end ownership across the full ML lifecycle — feature engineering on large-scale datasets, model training and calibration, real-time API deployment, and monitoring in production. Work spans fraud intelligence, customer analytics, financial AI, and agentic LLM systems.

Full working rights in Australia &nbsp;·&nbsp; Open to Data Scientist and ML Engineer roles

---

## Projects

<br/>

### FraudSentinel — Proactive Payment Fraud Intelligence

**[View Repository](https://github.com/RameshSTA/fraudsentinel)** &nbsp;·&nbsp; **[Live Drift Dashboard](https://rameshsta.github.io/fraudsentinel/reports/drift_monitoring_report.html)**

Early-warning fraud scoring system built on 590,540 real IEEE-CIS payment transactions. The model ranks every entity by its probability of committing fraud within the next **72 hours** — scoring risk before the financial loss materialises.

<table>
  <tr>
    <td align="center"><strong>4.7×</strong></td>
    <td align="center"><strong>37.8%</strong></td>
    <td align="center"><strong>7×</strong></td>
    <td align="center"><strong>19.5%</strong></td>
    <td align="center"><strong>3.5×</strong></td>
    <td align="center"><strong>&lt; 20 ms</strong></td>
  </tr>
  <tr>
    <td align="center">Operational Lift</td>
    <td align="center">Fraud Captured<br/>(Top 8% reviewed)</td>
    <td align="center">High Band Lift<br/>(Top 3%)</td>
    <td align="center">High Band<br/>Precision</td>
    <td align="center">AUC-PR above<br/>no-skill baseline</td>
    <td align="center">API Inference<br/>Latency</td>
  </tr>
</table>

**Architecture** — PyTorch MLP · MD5-hashed entity embeddings (32-dim learned vectors) · Temperature-scaled calibration via LBFGS · 72-hour early-warning label · Entity velocity features · Fraud campaign propagation signals

**MLOps** — MLflow experiment tracking · SHAP LinearExplainer (262K-dim feature space) · Evidently AI drift monitoring · DVC reproducible pipeline · Docker · 50 pytest unit tests · `make pipeline` end-to-end

<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square"/>
<img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
<img src="https://img.shields.io/badge/Evidently_AI-6C47FF?style=flat-square"/>
<img src="https://img.shields.io/badge/DVC-945DD6?style=flat-square&logo=dvc&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>

---

### CLV Long-Term Optimisation — Customer Value Forecasting & Retention

**[View Repository](https://github.com/RameshSTA/clv-long-term-optimization)**

End-to-end CLV forecasting, churn risk modelling, and budget-constrained retention investment optimisation on a £12.1M revenue corpus of 4,933 customers.

<table>
  <tr>
    <td align="center"><strong>0.816</strong></td>
    <td align="center"><strong>ρ = 0.57</strong></td>
    <td align="center"><strong>6.3×</strong></td>
    <td align="center"><strong>44.5×</strong></td>
    <td align="center"><strong>62%</strong></td>
  </tr>
  <tr>
    <td align="center">Churn Model<br/>AUC-ROC</td>
    <td align="center">CLV Forecast<br/>Spearman Rank ρ</td>
    <td align="center">Top-Decile<br/>Revenue Lift</td>
    <td align="center">Net ROI<br/>(£200 budget frontier)</td>
    <td align="center">Revenue from<br/>Top 10% of Customers</td>
  </tr>
</table>

**Models** — BG/NBD + Gamma-Gamma probabilistic CLV engine · Random Forest champion (AUC-PR = 0.883) · XGBoost · LightGBM · 5-fold stratified CV · PuLP/CBC 0-1 Knapsack budget allocator

**Analysis** — 500-draw Monte Carlo simulation with P5–P95 ROI confidence bands · 8-segment RFM taxonomy · Gini coefficient = 0.73 · SHAP attribution (recency and frequency as dominant churn drivers) · 11-stage automated scoring pipeline · MLflow + GitHub Actions CI

<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
<img src="https://img.shields.io/badge/XGBoost-189BCE?style=flat-square"/>
<img src="https://img.shields.io/badge/LightGBM-02569B?style=flat-square"/>
<img src="https://img.shields.io/badge/PuLP%2FCBC-4A90D9?style=flat-square"/>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square"/>
<img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>

---

### ConnectIntelligence — Real-Time Predictive Retention Engine

**[View Repository](https://github.com/RameshSTA/ConnectIntelligence)** &nbsp;·&nbsp; **[Live Demo](https://connect-intelligence.vercel.app)**

Member churn prediction and real-time risk scoring for the Australian Superannuation sector. Deployed as a production API with explainable AI and behavioural persona segmentation.

<table>
  <tr>
    <td align="center"><strong>0.86</strong></td>
    <td align="center"><strong>&lt; 200 ms</strong></td>
    <td align="center"><strong>4</strong></td>
  </tr>
  <tr>
    <td align="center">Weighted<br/>Accuracy</td>
    <td align="center">End-to-End<br/>API Latency</td>
    <td align="center">Actionable Risk<br/>Personas (K-Means)</td>
  </tr>
</table>

**Architecture** — XGBoost with systematic feature selection and hyperparameter tuning · FastAPI + Docker production API · SHAP explainability for every high-risk prediction · K-Means behavioural segmentation into four distinct retention intervention groups

<img src="https://img.shields.io/badge/XGBoost-189BCE?style=flat-square"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>

---

### FinGraph-ASX — Neuro-Symbolic GraphRAG Intelligence Engine

**[View Repository](https://github.com/RameshSTA/FinGraph-ASX-GraphRAG-Engine)**

Agentic AI system for financial due diligence over ASX-listed company annual reports. Replaces vector-only search with a structured, graph-indexed knowledge base — grounding every LLM response in traceable, source-linked evidence.

<table>
  <tr>
    <td align="center"><strong>40%</strong></td>
    <td align="center"><strong>15%</strong></td>
    <td align="center"><strong>50+</strong></td>
  </tr>
  <tr>
    <td align="center">Retrieval Latency<br/>Reduction</td>
    <td align="center">LLM Answer<br/>Accuracy Improvement</td>
    <td align="center">Financial Entities<br/>Auto-Extracted</td>
  </tr>
</table>

**Architecture** — LlamaIndex retrieval pipeline · Neo4j graph database · Groq LLM inference · Custom NLP entity extraction · Citation-style answer verification layer · Streamlit interface

<img src="https://img.shields.io/badge/LlamaIndex-6B4FBB?style=flat-square"/>
<img src="https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white"/>
<img src="https://img.shields.io/badge/Groq-0F2B5B?style=flat-square"/>
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>

---

## Technical Skills

**Machine Learning & AI**

<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/XGBoost-189BCE?style=flat-square"/>
<img src="https://img.shields.io/badge/LightGBM-02569B?style=flat-square"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
<img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
<img src="https://img.shields.io/badge/Prophet-3776AB?style=flat-square"/>
<img src="https://img.shields.io/badge/LSTM-EE4C2C?style=flat-square"/>
<img src="https://img.shields.io/badge/NLP%20%2F%20GraphRAG-6B4FBB?style=flat-square"/>

**MLOps & Deployment**

<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square"/>
<img src="https://img.shields.io/badge/DVC-945DD6?style=flat-square&logo=dvc&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/>
<img src="https://img.shields.io/badge/Evidently_AI-6C47FF?style=flat-square"/>

**Data Engineering**

<img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white"/>
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white"/>
<img src="https://img.shields.io/badge/Azure_Data_Factory-0078D4?style=flat-square&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>

**Cloud & Databases**

<img src="https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white"/>
<img src="https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>

**Visualisation & BI**

<img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white"/>
<img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white"/>
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>

---

## Professional Experience

**Associate Consultant — ERP Data Developer** &nbsp;·&nbsp; PM-Partners &nbsp;·&nbsp; Sydney &nbsp;·&nbsp; Feb 2026 – Present

Automated daily ingestion pipelines in Azure Data Factory, reducing manual effort by 40%. Slashed data refresh latency by 75% and elevated reporting accuracy by 30% through automated SQL/PL-SQL validation scripts across high-volume ERP production datasets.

**Data Science & ML Intern** &nbsp;·&nbsp; Hightech Mastermind Pty Ltd &nbsp;·&nbsp; Sydney &nbsp;·&nbsp; Feb 2025 – Apr 2025

Boosted forecasting performance 15% over baseline using a champion-challenger workflow (XGBoost, scikit-learn). Containerised all workflows in Docker with GitHub Actions CI/CD. Delivered stakeholder-ready Power BI + SHAP reports, accelerating executive decisions by 25%.

---

## Education

**Bachelor of Software Engineering** — Data Science & Artificial Intelligence &nbsp;·&nbsp; Torrens University Australia &nbsp;·&nbsp; 2021–2024

**Professional Year Program** — Information Technology &nbsp;·&nbsp; QIBA &nbsp;·&nbsp; 2024–2025

---

## Certifications

Google Advanced Data Analytics Professional Certificate &nbsp;·&nbsp; 2025

Deep Learning Specialisation — DeepLearning.AI &nbsp;·&nbsp; 2025

Machine Learning Specialisation — Stanford University / DeepLearning.AI &nbsp;·&nbsp; 2024

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0F2B5B&height=80&section=footer" width="100%"/>
</div>
