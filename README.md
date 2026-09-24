<div align="center">

<img width="100%" src="assets/header.svg" alt="Al-Amine Maouloud · Data & AI Engineer · Quantitative Finance" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1400&color=8B7CF6&center=true&vCenter=true&width=680&lines=I+build+the+risk+models+banks+rely+on;Python+%2B+C%2B%2B%2C+every+result+checked+against+exact+formulas;I+apply+AI+to+hard+scientific+problems;Looking+for+an+internship+from+January+2027" alt="Typing SVG" />

[![Email](https://img.shields.io/badge/Email-maouloudalamines%40outlook.fr-0f0c29?style=for-the-badge&logo=microsoft-outlook&logoColor=white)](mailto:maouloudalamines@outlook.fr)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Al--Amine%20Maouloud-302b63?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/al-amine-maouloud-412a89249)
[![Projects](https://img.shields.io/badge/See%20all%20my%20projects-24243e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/alamine-maouloud/projects_finance-ai)

</div>

---

## 👋 My profile in 30 seconds

- 🎓 **Who I am:** final-year engineering student (M2 Data & AI) at **ECE Paris**, on exchange in **Quantitative Finance** at the **University of Oslo**.
- 🏦 **What I build:** the models banks use to measure risk and price financial products, plus AI systems and research software used by real teams.
- ⭐ **What makes me different:** I code in both **Python and C++**, and I check every model against a known exact answer before trusting it.
- 🎯 **What I'm looking for:** a **6-month internship from January 2027** in quantitative finance, risk, or AI (Paris, London, Singapore, Hong Kong, Oslo, UAE).

<div align="center">

| 🏦 **3 in 1** | ⚡ **×5** | 📈 **15M / s** | ✅ **76** | 🤖 **4** |
|:---:|:---:|:---:|:---:|:---:|
| bank risks covered<br>by one engine | faster thanks<br>to C++ | stock-market orders<br>simulated per second | automated tests<br>proving the results | AI agents compared<br>on quantum chips |

</div>

---

## 🚀 Featured Projects

### 🏦 mcrisk · A risk engine for banks
**Monte Carlo · Black-Scholes · Limit Order Book** &nbsp;|&nbsp; `Python` `C++`

> **The problem.** A bank must know how much it could lose if borrowers default, if markets crash, or if a trading partner goes bankrupt, and it must hold enough capital to survive it.
>
> **What I built.** One engine that simulates millions of possible futures and computes these losses with the methods regulators require (Basel, FRTB). It also prices options with **Black-Scholes** and simulates a **stock-exchange order book**.
>
> **Why it matters.** Every result is checked against an exact formula (76 automated tests), and the heavy computations run in C++, up to **5× faster**.

<details>
<summary><b>🔍 Technical details</b></summary>
<br>

| Module | What it computes | Techniques |
|---|---|---|
| **Credit risk** | Loss distribution, VaR / ES 99.9%, economic capital | Gaussian and Student-t copulas, Euler allocation, Basel IRB comparison, importance sampling (~750× variance reduction) |
| **Market risk (FRTB)** | 10-day VaR and Expected Shortfall | Filtered historical simulation (GARCH), Kupiec and Christoffersen backtests |
| **Counterparty risk** | Exposure profiles, CVA / DVA | Hull-White model, CSA collateral, wrong-way risk |
| **Pricing** | Option prices and Greeks | Black-Scholes (C++ CLI), variance-reduced Monte Carlo, Longstaff-Schwartz, Heston |
| **Microstructure** | Order book dynamics, execution cost | C++ price-time priority matching (15M events/s), Hawkes order flow, Almgren-Chriss |

</details>

[**→ View the project**](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/finance-quant/monte-carlo-risk-engine)

<br>

### ⚛️ AI that calibrates quantum computers
**Deep Reinforcement Learning · Quantum Control** &nbsp;|&nbsp; `Python`

> **The problem.** Quantum computers are fragile: every chip is slightly different, so control signals tuned for an ideal chip lose precision on a real one.
>
> **What I built.** AI agents that learn to adjust the control signals chip by chip, on top of a classical optimization method. I compared **4 AI algorithms** on **100 simulated chips**.
>
> **Why it matters.** It shows I can take AI beyond standard datasets and apply it to a hard scientific problem.

<details>
<summary><b>🔍 Technical details</b></summary>
<br>

- Target: two-qubit CZ gate on a transmon-like Hamiltonian, with drift on qubit frequencies and coupling
- Baseline: GRAPE optimal control (QuTiP)
- AI: residual deep RL (SAC, TD3, DDPG, PPO with Stable-Baselines3) correcting pulses in a 20-mode cosine basis
- Evaluation: average gate fidelity over an ensemble of 100 noisy devices, versus optimal control alone

</details>

[**→ View the project**](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/machine-learning/quantum-gate-calibration)

<br>

### 🏥 Private AI assistant for neonatal intensive care research
**Generative AI · Local LLM · Text-to-SQL · RAG** &nbsp;|&nbsp; `Python`

> **The problem.** Researchers in a neonatal intensive care study wanted to ask questions about their data in plain English. But medical data about premature babies can never be sent to ChatGPT or any other cloud AI.
>
> **What I built.** A **private AI assistant that runs 100% on-site** (Llama 3), with no internet connection. It:
> - turns a researcher's question into a database query and answers with the result (**text-to-SQL**)
> - searches clinicians' free-text notes by meaning, not by keywords (**RAG**)
> - summarises session notes into structured data and **flags missing or inconsistent entries**
>
> Safety is built in at three levels: medical-advice requests are refused, the AI can only read the data (never change it), and identifying fields are hidden from it. Every AI answer is logged for audit.
>
> **Why it matters.** Generative AI deployed where it is hardest: sensitive medical data, no cloud, every answer traceable. The assistant runs on a research data platform I also built, alongside a desktop app (**NeoRhythm**) that plays the sound protocols during EEG sessions.

<details>
<summary><b>🔍 Technical details</b></summary>
<br>

- **LLM:** Llama 3 (8B) served locally with Ollama, fully offline
- **Text-to-SQL:** generated SQL is screened for write operations, then executed through a read-only DuckDB connection
- **Semantic RAG:** free-text notes embedded with sentence-transformers (all-MiniLM-L6-v2) in ChromaDB, answers synthesised by the LLM
- **LLM workflows:** note summarisation into structured JSON, LLM-based data-quality checks
- **Guardrails:** system prompt, read-only driver and de-identified schema, plus an AI audit-trail table
- **Platform:** Streamlit, SQLite + DuckDB, 71-field schema, 3-layer validation, de-identified exports
- **NeoRhythm:** tkinter + pygame, randomized protocols, CSV / JSON session logs, macOS and Windows builds

</details>

[**→ Platform & AI assistant**](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/data-engineering/nicu-research-data-platform) &nbsp;·&nbsp; [**→ NeoRhythm**](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/data-engineering/nicu-auditory-stimulation-app)

---

## 📂 More Projects

| Project | In one sentence | Built with |
|---|---|---|
| 🔐 **Federated fraud detection** | Detecting fraud across several banks **without sharing their customers' data** | PyTorch · Flower · XGBoost |
| 🏙️ [**Buy-to-let risk & return in every French commune**](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/finance-quant/real-estate-investment-analysis) | Prices a flat in 2,376 communes from **1.8 million real sales** and simulates 15 years of after-tax returns: **where it pays, and how much you can lose** | Python · pandas · Monte Carlo |
| 🚨 [**Card & payment fraud detection**](https://github.com/alamine-maouloud/projects_finance-ai/tree/main/machine-learning/card-payment-fraud-detection) | Catches **85% of fraud cases** while analysts review only 0.2% of transactions, and **explains every alert** | scikit-learn · Streamlit |

---

## 🧰 Skills

| Area | What I use it for | Tools |
|---|---|---|
| 🏦 **Quantitative finance** | Risk measurement, option pricing, simulation | Monte Carlo · Black-Scholes · VaR / ES · CVA |
| 💻 **Programming** | Fast, tested, production-style code | Python · C++17 · SQL · Java · C |
| 🤖 **AI & Machine Learning** | Prediction, fraud detection, decision-making agents | PyTorch · scikit-learn · XGBoost · deep RL · LLMs |
| 🗄️ **Data engineering** | Pipelines, databases, dashboards | Pandas · DuckDB · SQLite · Streamlit |

<div align="center">
<br>
<img src="https://skillicons.dev/icons?i=cpp,python,c,java,pytorch,tensorflow,sklearn,sqlite,postgres,git,linux&theme=dark" />
</div>

---

## 🎓 Education

| | School | Program | Period |
|:---:|---|---|---|
| 🇳🇴 | **University of Oslo** | Quantitative Finance (Exchange) | Sept 2026 – Jan 2027 |
| 🇫🇷 | **ECE Paris** | Engineering Degree · Data & AI (M2) | 2024 – 2027 |
| 🇫🇷 | **Saint-Joseph High School** | Preparatory Classes · Physics, Chemistry, Engineering | 2022 – 2024 |

**Certifications:** Generative AI & LLMs (IBM) · Financial Markets (Yale) · Data Analysis L2 (DataScientist) · Cloud Fundamentals · Project Management (Centrale Lille)

**Languages:** French (native) · English (C1) · Arabic (B2)

---

<div align="center">

### 📫 Open to Quant / Risk / AI internships from January 2027

[![Email](https://img.shields.io/badge/-maouloudalamines%40outlook.fr-0f0c29?style=flat-square&logo=microsoft-outlook&logoColor=white)](mailto:maouloudalamines@outlook.fr)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-302b63?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/al-amine-maouloud-412a89249)

<img width="100%" src="assets/footer.svg" alt="" />

</div>
