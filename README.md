<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0F2B5B&height=180&section=header&text=Ramesh%20Shrestha&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Data%20Scientist%20%C2%B7%20ML%20Engineer%20%C2%B7%20Sydney%2C%20Australia&descAlignY=62&descSize=18" width="100%"/>
</div>

<div align="center">

  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/rameshsta)
  [![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shrestha.ramesh000@gmail.com)
  [![GitHub](https://img.shields.io/badge/GitHub-RameshSTA-0F2B5B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RameshSTA)
  ![Profile Views](https://komarev.com/ghpvc/?username=RameshSTA&style=for-the-badge&color=0F2B5B&label=PROFILE+VIEWS)

</div>

<br/>

---

## About Me

I am a **Data Scientist** based in Sydney, Australia, with professional experience building and deploying **production-grade ML systems** across fraud intelligence, customer lifecycle analytics, financial AI, and healthcare. I currently work as an **Associate Consultant — ERP Data Developer at PM-Partners**, where I design and maintain automated Azure Data Factory ingestion pipelines and SQL/PL-SQL validation workflows that directly power executive reporting for HR and Payroll units.

My approach to ML is end-to-end — I own the full lifecycle from raw data ingestion, feature engineering, and model training through to real-time API deployment with FastAPI and Docker, and long-term drift monitoring in production. Every system I ship includes SHAP explainability for stakeholder trust, Evidently AI monitoring for reliability, and reproducible DVC pipelines for engineering rigour. I am fluent with **PyTorch, XGBoost, scikit-learn, MLflow, and Azure**, and comfortable working across both research-oriented and production-focused environments.

I hold a **Bachelor of Software Engineering (Data Science & Artificial Intelligence)** from Torrens University Australia, complemented by the Deep Learning Specialisation (DeepLearning.AI) and Machine Learning Specialisation (Stanford University / DeepLearning.AI). I have full working rights in Australia and am actively open to **Data Scientist and ML Engineer** opportunities where models ship to production and decisions are data-driven.

---

## Featured Projects

<br/>

### FraudSentinel — Proactive Payment Fraud Intelligence System

<div>

[![View on GitHub](https://img.shields.io/badge/View_on_GitHub-0F2B5B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RameshSTA/fraudsentinel)
[![Live Drift Dashboard](https://img.shields.io/badge/Live_Drift_Dashboard-1A56DB?style=for-the-badge&logo=googleanalytics&logoColor=white)](https://rameshsta.github.io/fraudsentinel/reports/drift_monitoring_report.html)

</div>

Most fraud detection systems react after a transaction is already flagged. **FraudSentinel detects risk 72 hours earlier** — before the financial loss materialises. Built on 590,540 real IEEE-CIS payment transactions, the system engineers a forward-looking early-warning label that asks: *will this entity commit fraud within the next three days?* Every transaction is then ranked by risk score, allowing operations teams to intervene proactively at a fraction of the cost of traditional reactive review.

<br/>

<table align="center">
  <tr>
    <td align="center" width="160"><h3>4.7×</h3>Operational Lift<br/>over random review</td>
    <td align="center" width="160"><h3>37.8%</h3>Fraud Captured<br/>reviewing only top 8%</td>
    <td align="center" width="160"><h3>7×</h3>High Band Lift<br/>in top 3% of traffic</td>
    <td align="center" width="160"><h3>19.5%</h3>Precision<br/>in High Risk Band</td>
    <td align="center" width="160"><h3>3.5×</h3>AUC-PR above<br/>no-skill baseline</td>
    <td align="center" width="160"><h3>&lt;20 ms</h3>Real-Time API<br/>Inference Latency</td>
  </tr>
</table>

<br/>

**Model Architecture** — A PyTorch MLP with MD5-hashed entity embeddings (32-dimensional learned vectors) captures behavioural identity across the transaction graph. Entity velocity features and fraud campaign propagation signals encode temporal risk dynamics. Predicted probabilities are calibrated via temperature scaling (LBFGS optimisation, T = 1.033), improving Brier score from 0.163 to 0.154 and ensuring the model's confidence is reliable for downstream risk banding.

**Risk Bands** — Scored transactions are bucketed into three operational tiers (High / Medium / Low) based on review capacity, not arbitrary thresholds. The High band (top 3% of traffic) delivers 19.5% precision and 7× lift — meaning every investigator hour is seven times more productive than an unguided review queue at identical operational cost.

**Production MLOps** — MLflow tracks every experiment. SHAP LinearExplainer generates feature attributions across a 262,000-dimensional feature space for each scored transaction. Evidently AI produces an interactive drift monitoring dashboard (live link above) comparing training and production distributions. DVC ensures the 11-stage pipeline is fully reproducible via a single `make pipeline` command. 50 pytest unit tests validate the full system.

<br/>

<table>
  <tr>
    <td><strong>Core&nbsp;ML</strong></td>
    <td>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
      <img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td><strong>MLOps</strong></td>
    <td>
      <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square"/>
      <img src="https://img.shields.io/badge/DVC-945DD6?style=flat-square&logo=dvc&logoColor=white"/>
      <img src="https://img.shields.io/badge/Evidently_AI-6C47FF?style=flat-square"/>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><strong>Language</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
      <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/>
    </td>
  </tr>
</table>

---

### CLV Long-Term Optimisation — Customer Value Forecasting & Retention

<div>

[![View on GitHub](https://img.shields.io/badge/View_on_GitHub-0F2B5B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RameshSTA/clv-long-term-optimization)

</div>

Most retention programmes treat all at-risk customers equally. This system answers a more precise question: *which customers are worth retaining, by how much, and what is the optimal budget allocation to maximise return?* Built on 4,933 customers representing a £12.1M revenue corpus, it combines **probabilistic CLV forecasting, machine learning churn classification, and integer-programming budget optimisation** into a single automated decision pipeline.

<br/>

<table align="center">
  <tr>
    <td align="center" width="160"><h3>0.816</h3>Churn Model<br/>AUC-ROC</td>
    <td align="center" width="160"><h3>ρ = 0.57</h3>CLV Forecast<br/>Spearman Rank</td>
    <td align="center" width="160"><h3>6.3×</h3>Revenue Lift<br/>Top-Decile Customers</td>
    <td align="center" width="160"><h3>44.5×</h3>Net ROI<br/>(£200 budget frontier)</td>
    <td align="center" width="160"><h3>62%</h3>Revenue from<br/>Top 10% of Customers</td>
  </tr>
</table>

<br/>

**CLV Forecasting** — A BG/NBD + Gamma-Gamma probabilistic engine predicts each customer's expected revenue over a 180-day holdout. Spearman rank correlation of 0.57 confirms strong ranking fidelity between predicted CLV and realised revenue. Top-decile customers deliver a 6.3× revenue lift over the portfolio mean, validating the model as a reliable capital allocation guide.

**Churn Classification** — Four classifiers (Random Forest, XGBoost, LightGBM, Logistic Regression) are benchmarked via 5-fold stratified cross-validation. The champion Random Forest achieves AUC-ROC = 0.816 and AUC-PR = 0.883. SHAP attribution identifies recency and transaction frequency as the dominant churn drivers — insight that was adopted directly into retention targeting rules.

**Budget Optimisation** — A PuLP/CBC 0-1 Knapsack allocator returns the optimal customer set to target under any spend constraint. At the £200 efficiency frontier, net ROI reaches 44.5×. A 500-draw Monte Carlo simulation stress-tests assumptions and delivers a full P5–P95 confidence band for every budget scenario, removing guesswork from retention investment decisions.

**Pipeline** — Fully automated 11-step scoring pipeline (ingest → clean → features → CLV → churn → optimise → evaluate → segment → cohort → insights → sensitivity). MLflow experiment tracking and GitHub Actions CI across Python 3.9 and 3.11. An 8-segment RFM taxonomy reveals a Gini coefficient of 0.73 — the top 10% of customers drive 62% of total revenue.

<br/>

<table>
  <tr>
    <td><strong>Core&nbsp;ML</strong></td>
    <td>
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
      <img src="https://img.shields.io/badge/XGBoost-189BCE?style=flat-square"/>
      <img src="https://img.shields.io/badge/LightGBM-02569B?style=flat-square"/>
      <img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td><strong>Optimisation</strong></td>
    <td>
      <img src="https://img.shields.io/badge/PuLP%2FCBC-4A90D9?style=flat-square"/>
      <img src="https://img.shields.io/badge/Monte_Carlo-0F2B5B?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td><strong>MLOps</strong></td>
    <td>
      <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square"/>
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><strong>Language</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
    </td>
  </tr>
</table>

---

### ConnectIntelligence — Real-Time Predictive Retention Engine

<div>

[![View on GitHub](https://img.shields.io/badge/View_on_GitHub-0F2B5B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RameshSTA/ConnectIntelligence)
[![Live Demo](https://img.shields.io/badge/Live_Demo-009688?style=for-the-badge&logo=vercel&logoColor=white)](https://connect-intelligence.vercel.app)

</div>

Member churn is a critical operational risk for Australian Superannuation funds. **ConnectIntelligence** predicts which members are at risk of disengaging — and explains *why* — so that engagement teams can intervene with targeted strategies rather than blanket campaigns. The system is deployed as a production-grade real-time API, returning a churn probability and behavioural persona classification for any member within 200 milliseconds.

<br/>

<table align="center">
  <tr>
    <td align="center" width="200"><h3>0.86</h3>Weighted Accuracy<br/>on held-out test data</td>
    <td align="center" width="200"><h3>&lt;200 ms</h3>End-to-End<br/>API Inference Latency</td>
    <td align="center" width="200"><h3>4</h3>Behavioural Risk Personas<br/>via K-Means Clustering</td>
  </tr>
</table>

<br/>

**Model** — XGBoost classifier with systematic feature selection, hyperparameter tuning via cross-validation, and class-imbalance handling. Achieves 0.86 weighted accuracy on the held-out test set. SHAP values are computed for every high-risk prediction, providing each engagement team member with a traceable, plain-language explanation of which factors drove the risk score — building trust and enabling targeted action.

**Segmentation** — K-Means clustering identifies four distinct behavioural risk personas from the member population. Each persona maps to a tailored intervention playbook, improving engagement team effectiveness by focusing effort on the right strategy for the right member type rather than applying one-size-fits-all outreach.

**Deployment** — The full system is containerised with Docker and served via FastAPI. End-to-end inference — from raw member input to scored output — completes in under 200 milliseconds, enabling real-time integration with operational dashboards and CRM systems. A live interactive demo is available via the link above.

<br/>

<table>
  <tr>
    <td><strong>Core&nbsp;ML</strong></td>
    <td>
      <img src="https://img.shields.io/badge/XGBoost-189BCE?style=flat-square"/>
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
      <img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td><strong>Deployment</strong></td>
    <td>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
      <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><strong>Language</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
    </td>
  </tr>
</table>

---

### FinGraph-ASX — Neuro-Symbolic GraphRAG Intelligence Engine

<div>

[![View on GitHub](https://img.shields.io/badge/View_on_GitHub-0F2B5B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RameshSTA/FinGraph-ASX-GraphRAG-Engine)

</div>

Financial due diligence on ASX-listed companies is time-consuming and error-prone when done manually across dense annual reports. **FinGraph** replaces keyword search and manual reading with an **agentic GraphRAG pipeline** — combining a structured knowledge graph of extracted financial entities with LLM-powered reasoning — so analysts can ask complex questions in plain language and receive answers grounded in traceable, source-linked evidence from the original documents.

<br/>

<table align="center">
  <tr>
    <td align="center" width="200"><h3>40%</h3>Retrieval Latency<br/>Reduction</td>
    <td align="center" width="200"><h3>15%</h3>LLM Answer Accuracy<br/>Improvement</td>
    <td align="center" width="200"><h3>50+</h3>Financial Entities<br/>Auto-Extracted per Report</td>
  </tr>
</table>

<br/>

**Architecture** — A custom NLP extraction pipeline parses ASX annual reports and maps 50+ financial entities (companies, executives, subsidiaries, financial metrics, risk factors) into a **Neo4j graph database**. At query time, LlamaIndex traverses the graph rather than performing vector-only semantic search, dramatically improving precision on multi-hop financial questions. Groq handles LLM inference for speed.

**Accuracy and Trust** — A citation-style verification layer attaches the source sentence, page, and document to every LLM response. This grounds answers in the original filings and eliminates hallucinations — a critical requirement for financial analysis where accuracy directly affects investment decisions. Analysts can trace every claim back to its exact source with a single click.

**Interface** — A Streamlit application allows analysts to interrogate any ASX-listed company's filings in plain English. The system returns structured, evidence-backed answers alongside a visual knowledge graph of entity relationships.

<br/>

<table>
  <tr>
    <td><strong>AI&nbsp;/&nbsp;LLM</strong></td>
    <td>
      <img src="https://img.shields.io/badge/LlamaIndex-6B4FBB?style=flat-square"/>
      <img src="https://img.shields.io/badge/Groq-0F2B5B?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td><strong>Graph DB</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><strong>Interface</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><strong>Language</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
    </td>
  </tr>
</table>

---

## Technical Skills

<table>
  <tr>
    <td nowrap><strong>Machine Learning & AI</strong></td>
    <td>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
      <img src="https://img.shields.io/badge/XGBoost-189BCE?style=flat-square"/>
      <img src="https://img.shields.io/badge/LightGBM-02569B?style=flat-square"/>
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
      <img src="https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square"/>
      <img src="https://img.shields.io/badge/Prophet-3776AB?style=flat-square"/>
      <img src="https://img.shields.io/badge/LSTM-EE4C2C?style=flat-square"/>
      <img src="https://img.shields.io/badge/NLP%20%2F%20GraphRAG-6B4FBB?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td nowrap><strong>MLOps & Deployment</strong></td>
    <td>
      <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square"/>
      <img src="https://img.shields.io/badge/DVC-945DD6?style=flat-square&logo=dvc&logoColor=white"/>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/>
      <img src="https://img.shields.io/badge/Evidently_AI-6C47FF?style=flat-square"/>
    </td>
  </tr>
  <tr>
    <td nowrap><strong>Data Engineering</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white"/>
      <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white"/>
      <img src="https://img.shields.io/badge/Azure_Data_Factory-0078D4?style=flat-square&logo=microsoftazure&logoColor=white"/>
      <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
      <img src="https://img.shields.io/badge/SQL%20%2F%20PL--SQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td nowrap><strong>Cloud & Databases</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white"/>
      <img src="https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white"/>
      <img src="https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white"/>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td nowrap><strong>Visualisation & BI</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black"/>
      <img src="https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white"/>
      <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white"/>
      <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td nowrap><strong>Languages</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square"/>
      <img src="https://img.shields.io/badge/PL--SQL-0F2B5B?style=flat-square"/>
      <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white"/>
    </td>
  </tr>
</table>

---

## Professional Experience

**Associate Consultant — ERP Data Developer** &nbsp;&nbsp; PM-Partners · Sydney, NSW · Feb 2026 – Present

Designing and maintaining automated daily ingestion pipelines in Azure Data Factory for HR and Payroll units, replacing error-prone manual exports with validated end-to-end refreshes. Reduced manual effort by 40%, cut data refresh latency from hours to under 30 minutes (75% reduction), and elevated reporting accuracy by 30% through automated SQL/PL-SQL referential integrity validation across high-volume ERP production datasets.

**Data Science & ML Intern** &nbsp;&nbsp; Hightech Mastermind Pty Ltd · Sydney, NSW · Feb 2025 – Apr 2025

Implemented a champion–challenger model selection workflow (scikit-learn, XGBoost) that boosted forecasting performance 15% over baseline. Containerised all ML workflows with Docker and automated deployment through GitHub Actions CI/CD. Delivered stakeholder Power BI dashboards paired with SHAP interpretability reports, accelerating executive decision cycles by 25%.

---

## Education

**Bachelor of Software Engineering — Data Science & Artificial Intelligence** &nbsp;·&nbsp; Torrens University Australia &nbsp;·&nbsp; 2021 – 2024

**Professional Year Program — Information Technology** &nbsp;·&nbsp; QIBA, Sydney &nbsp;·&nbsp; 2024 – 2025

---

## Certifications

Google Advanced Data Analytics Professional Certificate &nbsp;·&nbsp; Google &nbsp;·&nbsp; 2025

Deep Learning Specialisation &nbsp;·&nbsp; DeepLearning.AI &nbsp;·&nbsp; 2025

Machine Learning Specialisation &nbsp;·&nbsp; Stanford University / DeepLearning.AI &nbsp;·&nbsp; 2024

---

<div align="center">
  <sub>Full working rights in Australia &nbsp;·&nbsp; References available upon request</sub>
  <br/><br/>
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0F2B5B&height=80&section=footer" width="100%"/>
</div>
