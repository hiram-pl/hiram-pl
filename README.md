<!--
**hiram-pl/hiram-pl** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

Hello, I'm Hiram! I'm currently focused on **data engineering, applied modeling, and causal inference.** I've previously built warehouse pipelines and forecasting systems at [ADEO](https://www.adeo.com/) (30B+ revenue; parent of Leroy Merlin; Europe’s #1, world’s #3 DIY retailer).

---

## Featured work

### [Financed Emissions Estimator](https://github.com/hiram-pl/financed_emissions) · [Live demo](https://hiram-pl.github.io/financed_emissions/)
Predicting vehicle gCO₂/km across a €120M car-loan book, and quantifying how badly the standard PCAF fallback distorts it.

- XGBoost on ~150K EEA records — R² 0.91, MAE ~5% of mean, selected over tree/RF by 5-fold CV
- Powertrain-aware routing: isolating combustion cases cut RMSE ~25% and removed CO₂-collinear leakage
- Moved a 6K-loan book from PCAF data-quality score 5.0 → 3.0, showing the loan-amount proxy **overstates emissions by ~2.2×**
- Deployed as an interactive Streamlit app serving the model live

`Python` `XGBoost` `scikit-learn` `Streamlit`

---

### [Meridian](https://doc-insight-score.lovable.app/) — Paris Fintech Hackathon 2026, 5th of 800+
An agentic regulatory operating system for EU banks. Ingests ACPR/EBA regulator feeds and auto-generates role-specific AML/KYC compliance training, compressing a 12-month rollout to under an hour.

Founded the team, conceived the product, built the frontend, and delivered the final pitch and live demo to a VC jury including a Bessemer Venture Partners partner.

`LLM agents` `Regulatory data` `Lovable`

---

## Work not public here

The largest systems I've built are internal to ADEO and can't be open-sourced. Shape of the work:

| System | What it does |
|---|---|
| **KPI pipeline (BigQuery)** | 8+ source systems; replaced full-refresh with incremental `MERGE`, cutting bytes scanned 99.6% (3.5 TB → 13 GB) and per-read cost from $22 to $0.08 |
| **Four-tier view architecture** | 25+ views with LAKE/SWAMP governance, decoupling business rules from source schemas so onboarding a new business unit needs no core code changes |
| **Discount & sales star schema** | 19 business units / 11 countries unified into a Power BI-facing star schema, with collision-proof keys and line-grain checks catching fan-out at every stage |
| **Workforce forecasting engine** | Prophet-based headcount projection 36 months out for 74,000 employees; validated at 2.21% error on a 6-month backtest |

Happy to walk through any of these in detail!

---

## Stack

**Languages** Python (pandas, scikit-learn, matplotlib) · SQL · R (tidyverse, ggplot2)
**Data platform** BigQuery · Google Cloud Platform · Terraform · Power BI
**Modeling** Dimensional modeling / ELT · Gradient boosting (XGBoost) · Cross-validation
