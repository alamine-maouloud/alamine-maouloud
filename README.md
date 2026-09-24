<div align="center">

<!-- ANIMATED HEADER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=120&section=header&text=Al-Amine%20Maouloud&fontSize=42&fontColor=ffffff&fontAlignY=65&animation=fadeIn" />

</div>

<div align="center">

### `M2 Data & AI · ECE Paris` &nbsp;|&nbsp; `Quant Finance · UiO Oslo`

**Building at the intersection of Machine Learning, Quantitative Finance, and Systems Engineering**

[![Email](https://img.shields.io/badge/Email-maouloudalamines%40outlook.fr-0f0c29?style=flat-square&logo=microsoft-outlook&logoColor=white)](mailto:maouloudalamines@outlook.fr)
[![GitHub](https://img.shields.io/badge/GitHub-alamine--maouloud-302b63?style=flat-square&logo=github&logoColor=white)](https://github.com/alamine-maouloud)
[![Location](https://img.shields.io/badge/📍-Paris%20→%20Oslo-24243e?style=flat-square)](/)

</div>

---

## 👤 About Me

```python
profile = {
    "name"       : "Al-Amine Maouloud",
    "degree"     : "M2 Engineering – Data & AI @ ECE Paris (100% English)",
    "exchange"   : "Quantitative Finance @ University of Oslo (UiO) — Sept 2026",
    "target"     : ["Quant Finance", "ML Engineering", "Data Science"],
    "open_to"    : "6-month internship · Paris / Singapore / Hong Kong / London / Oslo / UAE",
    "languages"  : ["French (native)", "English (C1)", "Arabic (B2)"],
}
```

> I build end-to-end quantitative and ML systems, from **C++ pricing engines** and **Monte Carlo simulators**
> to **Federated Learning fraud detection** and **real-time orderbook engines**.
> I care about correctness, performance, and shipping things that work.

---

## 🔬 What I'm Working On

| Project | Stack | Status |
|---|---|---|
| mcrisk · Monte Carlo Risk Engine · Black-Scholes · Limit Order Book | Python, C++17, pybind11 | 🟢 Active |
| AI-Driven Quantum Gate Calibration | Deep RL, QuTiP, Stable-Baselines3 | 🟡 Running experiments |
| NICU Clinical Research Data Platform | Streamlit, SQLite, DuckDB, local LLM | ✅ Delivered |
| Federated Learning · Financial Fraud Detection | PyTorch, Flower, PySyft, XGBoost | 🟢 Active |
| Real Estate Investment Intelligence Platform | Python, Streamlit, Folium, DVF API | 🟡 Improving |
| Anomaly Detection · Banking Transactions | scikit-learn, IsolationForest, Pipeline | ✅ Complete |

---

## ⚙️ Technical Stack

**Quantitative Finance**
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Black-Scholes](https://img.shields.io/badge/Black--Scholes-pricing-302b63?style=flat-square)
![Monte Carlo](https://img.shields.io/badge/Monte%20Carlo-simulation-302b63?style=flat-square)
![pybind11](https://img.shields.io/badge/pybind11-C%2B%2B%20↔%20Python-302b63?style=flat-square)
![Time Series](https://img.shields.io/badge/Time%20Series-modeling-302b63?style=flat-square)

**Machine Learning & AI**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat-square)
![Federated Learning](https://img.shields.io/badge/Federated%20Learning-Flower%2FPySyft-24243e?style=flat-square)
![Reinforcement Learning](https://img.shields.io/badge/RL-Stable--Baselines3-24243e?style=flat-square)
![QuTiP](https://img.shields.io/badge/QuTiP-quantum%20control-302b63?style=flat-square)

**Data Engineering**
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![ETL](https://img.shields.io/badge/ETL%2FELT-pipelines-302b63?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)

**Infrastructure**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)

---

## 🚀 Featured Projects

### 🏦 mcrisk · Monte Carlo Risk Engine · Black-Scholes · Limit Order Book
> Credit, market, counterparty and market-microstructure risk in one engine, every model validated against closed-form results

- **Credit**: multi-factor Gaussian and Student-t copulas, VaR / ES 99.9%, Euler allocation, Basel IRB comparison; importance sampling cuts the variance of ES by ~750×
- **Market (FRTB IMA)**: filtered historical simulation (GARCH), 10-day ES 97.5%, Kupiec and Christoffersen backtests
- **Counterparty**: Hull-White exposures, CSA collateral, CVA / DVA with wrong-way risk
- **Pricing**: Black-Scholes pricer with full Greeks (C++ CLI), variance-reduced Monte Carlo, American options (Longstaff-Schwartz), Heston
- **Microstructure**: C++ price-time priority order book simulating 15M events/s, Hawkes order flow, Almgren-Chriss execution
- **Performance**: C++ kernels exposed through pybind11, up to ×5 faster than NumPy · 76 tests
- **Stack**: Python, C++17, pybind11, NumPy · [View project](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/finance-quant/monte-carlo-risk-engine)

---

### ⚛️ AI-Driven Quantum Gate Calibration
> AI-driven calibration of a two-qubit CZ gate: deep reinforcement learning agents adapt optimal-control pulses to each device's parameter drift

- **GRAPE** optimal control (QuTiP) computes the baseline pulses on the nominal Hamiltonian
- **AI (deep reinforcement learning)**: four agents (SAC, TD3, DDPG, PPO) learn to correct the pulses for each device in a 20-mode cosine basis
- AI-corrected pulses benchmarked against optimal control alone on an ensemble of 100 noisy devices
- **Stack**: Python, QuTiP, Gymnasium, Stable-Baselines3 · [View project](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/machine-learning/quantum-gate-calibration)

---

### 🏥 NICU Clinical Research Data Platform
> Clinical session logger and analytics platform for neonatal music-therapy research

- 71-field schema, SQLite (transactions) + DuckDB (analytics), 3-layer validation, de-identified exports, append-only audit trail
- Local LLM (Llama 3 via Ollama): text-to-SQL and RAG with guardrails, so no clinical data leaves the site
- Companion desktop app (**NeoRhythm**) delivering randomized auditory protocols during EEG sessions
- **Stack**: Python, Streamlit, SQLite, DuckDB, Ollama, ChromaDB · [View platform](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/data-engineering/nicu-research-data-platform) · [View NeoRhythm](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/data-engineering/nicu-auditory-stimulation-app)

---

### 🔐 Federated Learning · Fraud Detection *(Research internship)*
> Privacy-preserving ML applied to financial transaction fraud — trained on distributed data without centralization

- Implemented FL pipeline with **Flower** and **PySyft** across simulated distributed clients
- Models: **XGBoost** + **PyTorch** neural nets on financial time-series features
- Achieved comparable F1 to centralized baseline while preserving full data privacy
- Directly applicable to regulatory-compliant AI in banking (GDPR, MAS)

---

### 🏙️ Real Estate Investment Intelligence
> Full-stack data platform to identify high-yield real estate opportunities across France

- Ingested and cleaned **DVF** (notarial sales), **rent data**, **student density**, and **transport proximity** datasets
- Computed price/m², rental yield, volume trends per municipality and department
- Interactive map (Folium) + filters (Streamlit) for investment decision support
- **Stack**: Python, Pandas, NumPy, Seaborn, Streamlit, Folium, Jupyter

---

### 🚨 Anomaly Detection · Banking Transactions
> Unsupervised fraud detection pipeline for banking transaction monitoring

- End-to-end pipeline: preprocessing (impute → scale → encode) → **IsolationForest** → alert scoring
- Streamlit dashboard with threshold slider, Top-N suspicious transactions, CSV export
- Architecture: clean `core / domain / app` separation with synthetic data generator

---

## 🎓 Education & Certifications

| Institution | Program | Period |
|---|---|---|
| 🇳🇴 University of Oslo (UiO) | Quantitative Finance (Exchange) | Sept 2026 – Jan 2027 |
| 🇫🇷 ECE Paris | Engineering Degree · Data & AI (M2) | 2024 – 2026 |
| 🇫🇷 Saint-Joseph High School | Preparatory Classes · Physics-Chemistry-Engineering | 2022 – 2024 |

**Certifications**: Generative AI & LLMs (IBM) · Financial Markets (Yale) · Data Analysis L2 (DataScientist) · Cloud Fundamentals · Project Management (Centrale Lille)

---


<div align="center">

*Open to internship opportunities · Quant / AI / ML · January 2027*

**`maouloudalamines@outlook.fr`**

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=80&section=footer" />

</div>
