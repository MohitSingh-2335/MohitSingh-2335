&lt;div align=&quot;center&quot;&gt;

# Mohit Singh

### Applied AI/ML Engineer · Python Backend Developer · Generative AI & RAG

I build practical AI systems that connect machine learning models and local/cloud LLMs to authenticated APIs, deterministic fallbacks, and reproducible evaluation pipelines.

[](mailto:2335mohitsingh@gmail.com)
[](https://www.linkedin.com/in/mohit-singh-172548253/)
[Portfolio](https://www.google.com/search?q=https://mohitsingh-2335.github.io/)
[](https://leetcode.com/u/007NEMESIS/)

&lt;/div&gt;

## About Me

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
| **[Phishing Detection API](https://github.com/MohitSingh-2335/Phishing-detection-microservice)** | Threat ML & API Security | Python, Flask, XGBoost, scikit-learn, Render | 90%+ accuracy across 700K+ labeled URLs using 12 lexical/entropy features, redirect tracing, and HMAC-SHA256 replay protection |
| **[DePIN-Guard](https://github.com/MohitSingh-2335/DePIN-Guard)** ([Live Demo](https://www.google.com/search?q=https://depin-guard-frontend.vercel.app/)) | IIoT Anomaly Detection | PyTorch, LSTM Autoencoder, Flask, FastAPI, Docker, MQTT/TLS, Hyperledger Fabric | Unsupervised 30-step LSTM autoencoder microservice (`<60ms` inference latency) with fault-tolerant fallback and blockchain audit logging |
| **[Mudra](https://www.google.com/search?q=https://github.com/MohitSingh-2335/Mudra)** | Quantitative ML Research | Python, LightGBM, XGBoost, CatBoost, Optuna, SHAP, Streamlit | Multi-timeframe CCXT/Binance pipeline, Parquet storage, walk-forward validation design, Fractional Kelly/VaR risk limits, and SHAP explainability |
| **[Kaggriculture Agent](https://www.google.com/search?q=https://github.com/MohitSingh-2335/kaggriculture)** | Autonomous Simulation & Planning | Python, Market Modeling, Spatial Scheduling, Replay Diagnostics | Turn-based decision engine with typed state parsing, opponent tracking, Manhattan movement optimization, V1–V11 replay audits, and 55 passing unit tests |
| **[IBM RAG \& Agentic AI](https://www.google.com/search?q=https://github.com/MohitSingh-2335/ibm-rag-agentic-ai-architect)** | Generative AI & Retrieval | Python, IBM watsonx, LangChain/LCEL, LlamaIndex, ChromaDB, FAISS, BM25, Pydantic | Modular implementations covering hybrid dense/sparse retrieval, MMR, ReAct/LangGraph agents, MCP tool servers, and schema-validated JSON generation |

## Featured Engineering Deep Dives

### 1. [TaskPulse — Local-First AI Task Automation](https://github.com/MohitSingh-2335/Dynamic-Daily-Task-Engine)
A Flask productivity service that converts unstructured voice and text inputs into structured tasks, priority tiers, subtasks, and time-blocked schedules.
- **Hybrid AI & Heuristic Parsing:** Connects to local LLMs via Ollama with automatic heuristic fallbacks so task intake works reliably offline.
- **Stateful Workflows & Sync:** Implements SQLite persistence (with optional Supabase support), two-way Google Calendar OAuth2 synchronization, automated task rollover, and evening review workflows.
- **Observability & Testing:** Tracks inference latency and token usage via custom telemetry and validates behavior across 5 dedicated test suites (`test_api`, `test_ai_parser`, `test_task_service`, `test_database`, `test_memory`).

### 2. [Phishing Detection Microservice](https://github.com/MohitSingh-2335/Phishing-detection-microservice)
A hardened Flask REST microservice that classifies suspicious URLs in real time using engineered lexical and structural signals.
- **Feature Engineering & Model Selection:** Extracted 12 URL features (including Shannon entropy, digit density, subdomain depth, and redirect chains) across **700,000+ labeled URLs**, benchmarking XGBoost against Random Forest and SVM via `RandomizedSearchCV` to reach **90%+ accuracy**.
- **API Hardening:** Protected inference endpoints with **HMAC-SHA256 request signing**, timestamp validation for replay-attack prevention, and constant-time signature comparisons (`hmac.compare_digest`) against timing attacks.

### 3. [DePIN-Guard — Industrial IoT Anomaly Detection](https://github.com/MohitSingh-2335/DePIN-Guard) · [Live Demo](https://www.google.com/search?q=https://depin-guard-frontend.vercel.app/)
A four-person capstone framework for monitoring industrial IoT sensor streams and recording tamper-evident security alerts.
- **AI Inference Layer (Team AI Lead):** Architected and containerized a **PyTorch 30-step LSTM Autoencoder** microservice served via Flask, flagging unsupervised sensor anomalies via reconstruction-error thresholds at **<60ms telemetry latency**.
- **Resilient Distributed Integration:** Connected the anomaly detector to a Dockerized FastAPI, React, WebSocket, MQTT/TLS, and Hyperledger Fabric stack with graceful fallback handling if the inference container is unreachable.

### 4. [Mudra — Quantitative ML Research Platform](https://www.google.com/search?q=https://github.com/MohitSingh-2335/Mudra)
An experimental machine-learning pipeline for crypto market-data ingestion, technical feature engineering, strategy evaluation, and risk analysis.
- **Data & Modeling Pipeline:** Automated multi-timeframe OHLCV ingestion via CCXT/Binance into partitioned Parquet storage and compared LightGBM, XGBoost, and CatBoost models tuned with Optuna under chronological and walk-forward validation.
- **Risk Governance & Explainability:** Built event-driven backtesting accounting for fees, slippage, Fractional Kelly sizing, Value-at-Risk (VaR) limits, and drawdown circuit breakers, paired with SHAP signal attribution and a Streamlit research interface.

### 5. [Kaggriculture — Autonomous Market \& Scheduling Agent](https://www.google.com/search?q=https://github.com/MohitSingh-2335/kaggriculture)
An autonomous decision-making agent and benchmark suite for multi-step agricultural market simulation.
- **Algorithmic Planning:** Engineered typed game-state parsing, dynamic price and opponent modeling, value-density resource scheduling, and Manhattan-distance movement optimization.
- **Diagnostic Verification:** Built 20+ replay-analysis and economic-audit scripts across 11 strategy iterations (V1–V11), backed by **55 passing unit tests** covering state transitions, starvation guards, and scheduler invariants.

## Experience & Verified Credentials

### Work Experience
- **Machine Learning Intern — Edunet Foundation (AICTE & IBM SkillsBuild)** · *Remote · Jan 2025 – Feb 2025*  
  Built an end-to-end regression pipeline in Python (`scikit-learn`, `Pandas`, `NumPy`, `Matplotlib`) to forecast solar power generation from environmental telemetry, executing EDA, missing-value imputation, feature scaling, and evaluation across MAE, MSE, RMSE, and $R^2$ ([Solar\_power\_prediction](https://www.google.com/search?q=https://github.com/MohitSingh-2335/Solar_power_prediction)).

### Certifications
- **Oracle Fusion AI Agent Studio Certified Foundations Associate** — Oracle University (Oct 2025)
- **IBM RAG & Agentic AI Specialization Credentials** — IBM / Coursera (*Develop Generative AI Applications*, *Build RAG Applications*, *Vector Databases for RAG*, *Advanced RAG with Vector Databases and Retrievers*, *Build Multimodal Generative AI Applications*)
- **Artificial Intelligence Fundamentals** — IBM SkillsBuild (Credly)
- **Data Analysis with Python, Internet of Things & Blockchain Essentials** — IBM Developer Skills Network

## Technical Toolkit

| Layer | Technologies & Practices |
| :--- | :--- |
| **Languages & Data** | Python, SQL, Bash, Pandas, NumPy, Parquet, Feature Engineering, Exploratory Data Analysis (EDA) |
| **Machine Learning** | PyTorch, scikit-learn, XGBoost, LightGBM, CatBoost, Optuna, SHAP, LSTM Autoencoders, Walk-Forward Validation |
| **Generative AI & RAG** | IBM watsonx, LangChain (LCEL), LlamaIndex, ChromaDB, FAISS, BM25 Hybrid Search, LangGraph, ReAct, Ollama, Pydantic, MCP |
| **Backend & Security** | Flask, FastAPI, REST APIs, WebSockets, SQLite, Supabase, OAuth2, HMAC-SHA256, Replay Protection, JWT |
| **DevOps & Systems** | Docker, Docker Compose, GitHub Actions, Streamlit, MQTT/TLS, Hyperledger Fabric, Pytest / Unittest |

## GitHub Activity

&lt;div align=&quot;center&quot;&gt;

&lt;img src=&quot;https://github-readme-stats.vercel.app/api?username=MohitSingh-2335&amp;show_icons=true&amp;theme=react&amp;hide_border=true&amp;bg_color=0D1117&amp;title_color=58A6FF&amp;icon_color=58A6FF&amp;count_private=true&quot; height=&quot;160&quot; alt=&quot;Mohit&#39;s GitHub stats&quot;/&gt;
&lt;img src=&quot;https://github-readme-stats.vercel.app/api/top-langs/?username=MohitSingh-2335&amp;layout=compact&amp;theme=react&amp;hide_border=true&amp;bg_color=0D1117&amp;title_color=58A6FF&amp;hide=jupyter%20notebook,html,css&quot; height=&quot;160&quot; alt=&quot;Most used languages&quot;/&gt;

&lt;/div&gt;
