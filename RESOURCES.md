# AI Ethics & Social Justice Podcast — Resource Hub

A curated collection of open-source projects, research, and community discussions at the intersection of AI ethics, algorithmic fairness, and social justice.

## Open-Source Fairness & Bias Auditing Projects

### 1. [Fair-Code](https://github.com/yakew7/Fair-Code) — Algorithmic Bias Detection & Mitigation
- **Owner:** yakew7 · **Stars:** 46 · **Forks:** 31 · **License:** MIT
- **Language:** Python · **Last updated:** Sep 2026
- **What it does:** Seven real-world bias audits across criminal justice (COMPAS), hiring, lending, insurance denial, welfare eligibility, healthcare readmission, and tenant screening. Each audit follows a reproducible pipeline: train biased model → measure fairness gap → engineer fair model → measure again. Ships Jupyter notebooks, terminal scripts, and a reusable `faircode` Python package (Open Dataset Profiler, benchmark harness, MCP server).
- **Why it matters for this podcast:** Fair-Code doesn't just demonstrate bias — it demonstrates that removing protected attributes often isn't enough because proxy variables (custody status, employment tenure, BMI, payer code) carry the same signal. Its explainers (53+) on the impossibility theorem, proxy entanglement, sampling bias, and race correction in clinical algorithms are among the best publicly available pedagogical material on why fairness metrics conflict.

### 2. [ai-ethics-toolkit](https://github.com/Menth1996/ai-ethics-toolkit) — Bias Detection, Fairness Metrics & Explainability
- **Owner:** Menth1996 · **Language:** Python
- **What it does:** A Python toolkit for analyzing and mitigating bias, ensuring fairness, and promoting transparency in AI models. Provides bias detection, fairness metrics (demographic parity, equal opportunity, disparate impact), explainability (LIME, SHAP), and privacy-preserving AI (differential privacy, federated learning).
- **Why it matters for this podcast:** Bridges the gap between research fairness metrics and practitioner-friendly tooling. Its modular design (bias detector → explainer → privacy module) mirrors how real audit workflows need to move between detection, explanation, and remediation.

### 3. [ai-ethics-auditor](https://github.com/Eired1975/ai-ethics-auditor) — AI Bias Audit Tool (LLM Focus)
- **Owner:** Eired1975 · **Language:** TypeScript
- **What it does:** A focused toolkit for auditing AI models for bias, fairness, and transparency, with particular attention to large language models.
- **Why it matters for this podcast:** As LLMs move into high-stakes decision-making (hiring screening, content moderation, loan approval), the fairness challenges shift from tabular proxy-detection to prompt bias, training data contamination, and generation-time discrimination.

## Key Concepts Covered on This Podcast

| Concept | What It Means | Where to Start |
|---------|--------------|----------------|
| **Fairness Metric Conflicts** | The mathematically proven impossibility of satisfying Demographic Parity, Equalized Odds, and Predictive Parity simultaneously when base rates differ across groups | Fair-Code explainers/fairness-metric-conflicts.md |
| **Proxy Variables** | Why removing a protected attribute like race doesn't remove the bias — correlated features carry the same signal | Fair-Code explainers/proxy-variables.md |
| **The COMPAS Debate** | ProPublica and Northpointe were both right — using different fairness metrics | Fair-Code COMPAS audit |
| **Intersectional Bias** | Why auditing race and gender separately misses discrimination against people at their intersection | Fair-Code Explainers |
| **Demographic Parity vs. Equalized Odds** | Equal outcomes vs. equal error rates — you often can't have both | Fair-Code explainers |

## How to Contribute

This is a crowdsourced hub. If you know of an active project, a controversial issue thread, or a research paper that belongs here, open an issue or submit a PR.