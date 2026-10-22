<div align="center">

# Mohit Singh

### Applied AI/ML Engineer · Python Backend Developer · Generative AI & RAG

I build practical AI systems that connect machine learning models and local/cloud LLMs to authenticated APIs, deterministic fallbacks, and reproducible evaluation pipelines.

[![Email](https://img.shields.io/badge/Email-2335mohitsingh%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:2335mohitsingh@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-mohit--singh-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohit-singh-172548253/)
[![Portfolio](https://img.shields.io/badge/Portfolio-mohitsingh--2335.github.io-58A6FF?style=flat-square&logo=google-chrome&logoColor=white)](https://mohitsingh-2335.github.io/)
[![LeetCode](https://img.shields.io/badge/LeetCode-007NEMESIS-FFA116?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/u/007NEMESIS/)

</div>

---


I am a **B.Tech CSE (IoT & Blockchain)** graduate (2022–2026) from **Babu Banarasi Das University, Lucknow**. My engineering work focuses on bridging the gap between standalone notebooks and maintainable software services:

- **End-to-End Delivery:** Designing data ingestion, feature pipelines, and model inference alongside Flask/FastAPI microservices, SQLite/Parquet persistence, and Dockerized deployments.
- **Defensive Engineering:** Implementing HMAC-SHA256 request signing, replay protection, OAuth2 sync, and rule-based fallbacks when LLM or ML endpoints degrade.
- **Honest Evaluation:** Using chronological/walk-forward splits, benchmark replay diagnostics, and automated `pytest`/`unittest` suites rather than leaky random splits.

```python
mohit = {
    "location": "Lucknow, Uttar Pradesh, India",
    "focus": ["Applied AI/ML Microservices", "Python Backend Engineering", "RAG & Agentic Workflows"],
    "core_stack": ["Python", "PyTorch", "XGBoost/LightGBM", "Flask/FastAPI", "LangChain/watsonx", "Docker"],
    "open_to": ["AI/ML Engineer", "Python Backend Engineer", "Generative AI Engineer"],
}
```

## Systems at a Glance

| System | Domain | Core Stack | Key Engineering & Evaluation Proof |
| :--- | :--- | :--- | :--- |
| **[TaskPulse](https://github.com/MohitSingh-2335/Dynamic-Daily-Task-Engine)** | Local-First AI & Backend Automation | Python, Flask, SQLite, Supabase, Ollama, Google Calendar API | Voice/text task parser with local LLM + deterministic fallback, OAuth2 calendar sync, latency/token telemetry, and 5 test modules |
| **[Phishing Detection API](https://github.com/MohitSingh-2335/Phishing-detection-microservice)** ([Live Demo](https://url-tester.netlify.app/))| Threat ML & API Security | Python, Flask, XGBoost, scikit-learn, Render | 90%+ accuracy across 700K+ labeled URLs using 12 lexical/entropy features, redirect tracing, and HMAC-SHA256 replay protection |
| **[DePIN-Guard](https://github.com/MohitSingh-2335/DePIN-Guard)** ([Live Demo](https://depin-guard-frontend.vercel.app/)) | IIoT Anomaly Detection | PyTorch, LSTM Autoencoder, Flask, FastAPI, Docker, MQTT/TLS, Hyperledger Fabric | Unsupervised 30-step LSTM autoencoder microservice (`<60ms` inference latency) with fault-tolerant fallback and blockchain audit logging |
| **[Mudra](https://github.com/MohitSingh-2335/Mudra)** ([Live Demo](https://mudra-trading.streamlit.app/))| Quantitative ML Research | Python, LightGBM, XGBoost, CatBoost, Optuna, SHAP, Streamlit | Multi-timeframe CCXT/Binance pipeline, Parquet storage, walk-forward validation design, Fractional Kelly/VaR risk limits, and SHAP explainability |

## Featured Engineering Deep Dives

### 1. [TaskPulse — Local-First AI Task Automation](https://github.com/MohitSingh-2335/Dynamic-Daily-Task-Engine)
A Flask productivity service that converts unstructured voice and text inputs into structured tasks, priority tiers, subtasks, and time-blocked schedules.
- **Hybrid AI & Heuristic Parsing:** Connects to local LLMs via Ollama with automatic heuristic fallbacks so task intake works reliably offline.
- **Stateful Workflows & Sync:** Implements SQLite persistence (with optional Supabase support), two-way Google Calendar OAuth2 synchronization, automated task rollover, and evening review workflows.
- **Observability & Testing:** Tracks inference latency and token usage via custom telemetry and validates behavior across 5 dedicated test suites (`test_api`, `test_ai_parser`, `test_task_service`, `test_database`, `test_memory`).

### 2. [Phishing Detection Microservice](https://github.com/MohitSingh-2335/Phishing-detection-microservice) · [Live Demo](https://url-tester.netlify.app/)
A hardened Flask REST microservice that classifies suspicious URLs in real time using engineered lexical and structural signals.
- **Feature Engineering & Model Selection:** Extracted 12 URL features (including Shannon entropy, digit density, subdomain depth, and redirect chains) across **700,000+ labeled URLs**, benchmarking XGBoost against Random Forest and SVM via `RandomizedSearchCV` to reach **90%+ accuracy**.
- **API Hardening:** Protected inference endpoints with **HMAC-SHA256 request signing**, timestamp validation for replay-attack prevention, and constant-time signature comparisons (`hmac.compare_digest`) against timing attacks.

### 3. [DePIN-Guard — Industrial IoT Anomaly Detection](https://github.com/MohitSingh-2335/DePIN-Guard) · [Live Demo](https://depin-guard-frontend.vercel.app/)
A four-person capstone framework for monitoring industrial IoT sensor streams and recording tamper-evident security alerts.
- **AI Inference Layer (Team AI Lead):** Architected and containerized a **PyTorch 30-step LSTM Autoencoder** microservice served via Flask, flagging unsupervised sensor anomalies via reconstruction-error thresholds at **<60ms telemetry latency**.
- **Resilient Distributed Integration:** Connected the anomaly detector to a Dockerized FastAPI, React, WebSocket, MQTT/TLS, and Hyperledger Fabric stack with graceful fallback handling if the inference container is unreachable.

### 4. [Mudra — Quantitative ML Research Platform](https://github.com/MohitSingh-2335/Mudra) · [Live Demo](https://mudra-trading.streamlit.app/)
An experimental machine-learning pipeline for crypto market-data ingestion, technical feature engineering, strategy evaluation, and risk analysis.
- **Data & Modeling Pipeline:** Automated multi-timeframe OHLCV ingestion via CCXT/Binance into partitioned Parquet storage and compared LightGBM, XGBoost, and CatBoost models tuned with Optuna under chronological and walk-forward validation.
- **Risk Governance & Explainability:** Built event-driven backtesting accounting for fees, slippage, Fractional Kelly sizing, Value-at-Risk (VaR) limits, and drawdown circuit breakers, paired with SHAP signal attribution and a Streamlit research interface.

## Experience & Verified Credentials

### Work Experience
- **Machine Learning Intern — Edunet Foundation (AICTE & IBM SkillsBuild)** · *Remote · Jan 2025 – Feb 2025*  
  Built an end-to-end regression pipeline in Python (`scikit-learn`, `Pandas`, `NumPy`, `Matplotlib`) to forecast solar power generation from environmental telemetry, executing EDA, missing-value imputation, feature scaling, and evaluation across MAE, MSE, RMSE, and R² ([Solar_power_prediction](https://github.com/MohitSingh-2335/Solar_power_prediction)).

### Certifications
- **IBM RAG & Agentic AI Specialization Credentials** — IBM / Coursera (*Develop Generative AI Applications*, *Build RAG Applications*, *Vector Databases for RAG*, *Advanced RAG with Vector Databases and Retrievers*, *Build Multimodal Generative AI Applications*)
- **Artificial Intelligence Fundamentals** — IBM SkillsBuild (Credly)
- **Oracle Fusion AI Agent Studio Certified Foundations Associate** — Oracle University (Oct 2025)
- **Data Analysis with Python, Internet of Things & Blockchain Essentials** — IBM Developer Skills Network

## Technical Toolkit

| Layer | Technologies & Practices |
| :--- | :--- |
| **Languages & Data** | Python, SQL, Bash, Pandas, NumPy, Feature Engineering, Exploratory Data Analysis (EDA) |
| **Machine Learning** | PyTorch, scikit-learn, XGBoost, LightGBM, Optuna, SHAP, LSTM Autoencoders, Walk-Forward Validation |
| **Generative AI & RAG** | IBM watsonx, LangChain (LCEL), LlamaIndex, ChromaDB, FAISS, BM25 Hybrid Search, LangGraph, ReAct, Pydantic, MCP |
| **Backend** | Flask, FastAPI, REST APIs, SQLite, Supabase |
| **DevOps & Systems** | Docker, Docker Compose, GitHub Actions, Streamlit, Pytest / Unittest |

---

## GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=MohitSingh-2335&show_icons=true&theme=react&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF&count_private=true" height="160" alt="Mohit's GitHub stats"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=MohitSingh-2335&layout=compact&theme=react&hide_border=true&bg_color=0D1117&title_color=58A6FF&hide=jupyter%20notebook,html,css" height="160" alt="Most used languages"/>

</div>
