# John Oluwaseun Fashola

**Machine Learning Engineer**

I build end-to-end ML systems and data infrastructure for fintech, DeFi, and agricultural intelligence. Based in Abuja, Nigeria. Available for remote international contracts.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/john-fashola-67a149228/)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/John_TheAnalyst)
[![Portfolio](https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=vercel&logoColor=white)](https://john-fash.netlify.app/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:fashjohn04@gmail.com)
![Available](https://img.shields.io/badge/Status-Available%20for%20contracts-00B896?style=flat-square)

---

## Production Systems

These are live, deployed systems currently running in production or publicly accessible.

| Project | Domain | Status | Live |
|---|---|---|---|
| Agrolinking Commodity Intelligence Platform | Agricultural ML | ![Live](https://img.shields.io/badge/-Live-00B896?style=flat-square) | [API](https://agrolinking-intelligence-api.onrender.com/docs) · [Dashboard](https://agrolinking-intelligence-f8qq4uhupaax2qny8rpcpx.streamlit.app) |
| FRIDAY: Liquidity Intelligence Platform | Fintech ML | ![Deployed](https://img.shields.io/badge/-Deployed-00B896?style=flat-square) | [Live Demo](https://friday-beige-beta.vercel.app) |
| Solana AI Agent Wallet | DeFi / Autonomous Agent | ![Deployed](https://img.shields.io/badge/-Deployed-00B896?style=flat-square) | [Live Demo](https://solana-ai-agent-wallet.vercel.app/) |
| ERNIE: Retention Intelligence Engine | Product Analytics | ![Deployed](https://img.shields.io/badge/-Deployed-00B896?style=flat-square) | [GitHub](https://github.com/John-04/ERNIE) |
| Mobile Ad Fraud Detection | Fraud Detection / Anomaly Detection | ![In Development](https://img.shields.io/badge/-In%20Development-F59E0B?style=flat-square) | [GitHub](https://github.com/04-John/mobile-adfraud-clustering) |
| Crime Analytics Platform | Public Safety ML | ![In Development](https://img.shields.io/badge/-In%20Development-F59E0B?style=flat-square) | Coming soon |

---

## Agrolinking Commodity Intelligence Platform

**Lead ML Engineer · Agrolinking Solutions · Live in production**

Nigeria's most accurate agricultural price intelligence system. A 5-model ensemble forecasting 17 commodities across 6 geopolitical zones at 6 forecast horizons, running fully automated in daily production.

```
Stack: Python · XGBoost · LightGBM · Prophet · ARIMA · Holt-Winters · FastAPI · Streamlit · SHAP · pandas · scikit-learn
```

| Metric | Result |
|---|---|
| Average forecast error post-validation | 1.7% |
| Raw ensemble error before validation | 13.8% |
| Commodities tracked | 17 |
| Models per commodity | 5 |
| Forecast horizons | 6 (daily to 6-month) |
| Features engineered per commodity | 79 |
| States covered | 12 across 6 geopolitical zones |
| API endpoints | 8 |

**How the ensemble works**

Five models run in parallel per commodity. Weights are assigned inversely proportional to each model's holdout MAPE so the best performing model dominates but all five contribute. A scaling correction framework then cross-validates every forecast against Agricome Africa, WFP Nigeria, and NGX market sources before publishing.

**Key sourcing intelligence**

| Commodity | Best State | Saving vs Lagos |
|---|---|---|
| Ginger | Kaduna | 67% cheaper |
| Maize (white) | Kano | 62% cheaper |
| Sorghum | Kano | 54% cheaper |
| Soybeans | Plateau | 47% cheaper |
| Beans (white) | Kano | 47% cheaper |
| Rice | Plateau | 31% cheaper |

[![API Docs](https://img.shields.io/badge/Live%20API-agrolinking--intelligence--api.onrender.com-00B896?style=flat-square)](https://agrolinking-intelligence-api.onrender.com/docs)
[![Dashboard](https://img.shields.io/badge/Dashboard-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://agrolinking-intelligence-f8qq4uhupaax2qny8rpcpx.streamlit.app)

---

## FRIDAY: Liquidity Intelligence Platform

**ML Engineer · Paycrest case study**

Predicts payment corridor failures in African fintech before they happen. Built as a case study for Paycrest, deployed and publicly accessible.

```
Stack: Random Forest · XGBoost · LightGBM · SHAP · FastAPI · APScheduler · React · TypeScript · pytest
```

| Metric | Result |
|---|---|
| Ensemble models | 3 (RF, XGBoost, LightGBM) |
| Precision improvement over best single model | ~8% on critical failure class |
| API endpoints | 11 |
| Test suite | 39 tests (unit, integration, API) |
| Explainability | SHAP ranked contributing factors |

The SHAP explainability layer surfaces ranked contributing factors in plain language so clients understand why a corridor is flagged, not just a probability score. This is essential for trust in financial systems where a black box answer is not acceptable.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-friday--beige--beta.vercel.app-00B896?style=flat-square)](https://friday-beige-beta.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-John--04%2FFRIDAY-181717?style=flat-square&logo=github)](https://github.com/John-04/FRIDAY)

---

## Solana AI Agent Wallet

**DeFi Developer · Superteam Nigeria Challenge**

An autonomous DeFi agent that controls its own private keys and makes BUY, SELL, and HOLD decisions on-chain every 20 seconds with no human in the loop.

```
Stack: Solana · TypeScript · LangChain · ElizaOS · AutoGen · npm SDK · REST API · Render
```

| Metric | Result |
|---|---|
| Decision cycle | Every 20 seconds |
| Decision logic | Moving Average crossover signals |
| On-chain audit trail | Solana Memo Program (immutable) |
| Published SDK | AgentWalletSDK on npm |
| Framework compatibility | LangChain · AutoGen · ElizaOS |

Every decision is recorded immutably on-chain via the Solana Memo Program, creating a verifiable reasoning trail. The published npm SDK means any AI framework can import and control the agent.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-solana--ai--agent--wallet.vercel.app-00B896?style=flat-square)](https://solana-ai-agent-wallet.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-John--04%2FSolana--AI--Agent--Wallet-181717?style=flat-square&logo=github)](https://github.com/John-04/Solana-AI-Agent-Wallet)

---

## ERNIE: Engagement and Retention Network Intelligence Engine

**ML Engineer · Blockradar case study**

ML-powered user engagement and retention analytics built as a case study for Blockradar. Surfaces churn signals, engagement scoring, and cohort patterns from blockchain product user behaviour.

```
Stack: Python · scikit-learn · SQL · Streamlit · Plotly · pandas
```

[![GitHub](https://img.shields.io/badge/GitHub-John--04%2FERNIE-181717?style=flat-square&logo=github)](https://github.com/John-04/ERNIE)

---

## Technical Stack

**Machine Learning and AI**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Prophet](https://img.shields.io/badge/Prophet-003087?style=flat-square)
![SHAP](https://img.shields.io/badge/SHAP-111111?style=flat-square)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)

**Engineering and Deployment**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

**Data and Business Intelligence**

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)

**Blockchain**

![Solana](https://img.shields.io/badge/Solana-9945FF?style=flat-square&logo=solana&logoColor=white)

---

## Mobile Ad Fraud Detection via Clustering

**ML Engineer · Anomaly Detection · In development**

Unsupervised anomaly detection system for mobile ad click fraud using the TalkingData dataset (184 million click records). Identifies device farms and bot networks by clustering behavioural patterns across IP, device, OS, app, and channel dimensions.

```
Stack: Python · HDBSCAN · DBSCAN · scikit-learn · SHAP · FastAPI · pandas · NumPy · pytest
```

| Component | Detail |
|---|---|
| Feature engineering | Rolling-window behavioural features per IP, device, and OS |
| Clustering | HDBSCAN (primary) · DBSCAN (noise isolation) · K-Means (baseline) |
| Cross-population comparison | Chi-square tests and KL divergence for distribution shift |
| Explainability | SHAP values per flagged cluster |
| Serving | FastAPI /score endpoint for near real-time scoring |

[![GitHub](https://img.shields.io/badge/GitHub-04--John%2Fmobile--adfraud--clustering-181717?style=flat-square&logo=github)](https://github.com/04-John/mobile-adfraud-clustering)

---

## Work Experience

| Role | Organisation | Period |
|---|---|---|
| Lead Data Analyst and ML Engineer | Agrolinking Solutions | May 2024 to Present |
| Data Engineering Lead | StarkLytics | Sep 2025 to Dec 2025 |
| Analytics Facilitator | TenderDexta | Apr 2025 to Aug 2025 |
| Research Analyst | DataRactive | Aug 2024 to Sep 2024 |

---

## Awards and Recognition

| Award | Organisation | Year |
|---|---|---|
| Hackathon Winner: Best Infrastructure Tool | StarkLytics, StarkNet Ecosystem | Sep 2025 |
| Award for Leadership and Contribution to Data Education | TenderDexta Analytics Bootcamp | 2025 |
| DataCamp Scholarship Recipient | Data Community Africa | 2026 |

---

## Education and Certifications

**B.Sc. Criminology** · Federal University Oye-Ekiti (FUOYE) · Final Year · Oct 2022 to Jul 2026

| Certification | Issuer | Year |
|---|---|---|
| Data Engineering and ML Track | DataCamp, Data Community Africa Scholarship | 2026 |
| IBM Data Science Professional Certificate | IBM and Coursera | Apr 2023 |
| Google Data Analytics Certificate | Google and Coursera | Sep 2021 |
| Data Analytics Nanodegree | Udacity | Jan 2021 |

---

## GitHub Stats

<div align="center">

![John's GitHub Stats](https://github-readme-stats.vercel.app/api?username=John-04&show_icons=true&theme=default&count_private=true&hide_border=true&title_color=000000&icon_color=00B896&text_color=333333&bg_color=ffffff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=John-04&layout=compact&hide_border=true&title_color=000000&text_color=333333&bg_color=ffffff&langs_count=6)

</div>

---

<div align="center">

**Rate: $35 to $55/hr · Available immediately for remote contracts**

[![Portfolio](https://img.shields.io/badge/View%20Portfolio-john--fash.netlify.app-111111?style=flat-square)](https://john-fash.netlify.app/)
[![Email](https://img.shields.io/badge/Contact-fashjohn04%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:fashjohn04@gmail.com)

</div>
