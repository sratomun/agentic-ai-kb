---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Green SARC: Predictive Cost and Carbon Governance for Agentic AI Systems"
authors: Gaston Besanson (Universidad Torcuato Di Tella)
url: https://arxiv.org/abs/2606.15954
date: 2026-06-14
citationCount: 0
influentialCitationCount: 0
velocity: recent
ingested: 2026-06-26
tags: [arxiv, agent-finops, cost-governance, greenops, governance-gap, agentic-ai, 2026]
---

# Green SARC: Predictive Cost and Carbon Governance for Agentic AI Systems

**arXiv [2606.15954](https://arxiv.org/abs/2606.15954)** · 2026-06-14 · **recent (citations not yet accrued)** · Gaston Besanson

**Significance.** The cleanest statement of the thesis that **budget safety is an architectural property, not a reward-shaping hope** — and the node that ties [[agent-finops]] to [[governance-gap]] and GreenOps.

## Abstract
Agentic AI systems act through tools and sub-agents, yet the controls meant to bound their financial and environmental cost still sit on dashboards evaluated beside or after execution. Green SARC applies the SARC governance-by-architecture framework — four enforcement sites in the agent loop — to FinOps and GreenOps, contributing the theory of what to enforce and how to predict it. We report four policy-independent results. (i) The unconstrained "State Snowball" is Θ(n²) in loop depth; on 3,000 real multi-step plans (SWE-rebench) it holds on 100%, with median curvature ĉ₂ = 216 exceeding the linear-accretion prediction p/2 = 134. (ii) On real residuals the Normal-σ gate under-covers (92% at nominal 95%); split-conformal calibration holds (95.2%). (iii) A soft Lagrangian penalty tuned to the budget in expectation breaches it on 91.5% of seeds; the architectural gate breaches 0%. (iv) Under binding budgets the gate's over-budget incidence is 0% on synthetic and real (BurstGPT) arrivals. End-to-end token/USD/carbon savings (47–55%) are real but policy-dependent in magnitude — set by a scope-cap knob, not by gate rejections.

## From the paper (full-text)
**Contribution / method.** Applies the SARC "governance-by-architecture" framework — four enforcement sites compiled into the agent loop (Pre-Action Gate, Action-Time Monitor, Post-Action Auditor, Escalation Router) — to cost/carbon rather than correctness. The core construct is a **predictive pre-action gate**: an online per-(kind, model) OLS estimator forecasts a proposed action's token cost/carbon and admits it only if the forecast plus a safety margin fits the remaining budget at confidence 1−δ. The safety margin is upgraded from a Normal-σ bound to a distribution-free **split-conformal** margin (Theorem 2), with an anytime-valid trajectory over-spend bound via Ville's inequality (Theorem 3). Rule-based accounting is shown to be the "zero-information limit" of this gate.
**Results.** Architectural gate: **0% over-budget incidence** at every budget level (φ = 0.25×–2.0× baseline, δ=0.05, 20 seeds) vs **91.5% of seeds breached** by a soft Lagrangian penalty. Full-stack savings on the synthetic workload: **47.3% token / 67.6% USD / 67.3% carbon** (5.99M tokens/$100.68/897 gCO₂e → 3.16M/$32.57/294 gCO₂e); 55.7% token cut on real BurstGPT arrivals — flagged as partly a context-truncation-cap artifact. Calibration: split-conformal holds **95.2%** where Normal-σ under-covers at 92%. "State Snowball" confirmed: 100% of 3,000 SWE-rebench plans show positive quadratic curvature (median ĉ₂ = 216 > predicted 134). Gate overhead p50 1.7 μs / p99 3.7 μs.
**Takeaway.** A calibrated pre-action gate enforces hard budgets (0% overspend) where a "soft penalty" breaches ~92% of the time; the headline 47–55% savings are a tunable scope knob, so report mechanism and calibration, not just the percentage.

## Graph
- **Concepts:** [[agent-finops|Agent FinOps]] · [[governance-gap|Governance gap]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** census record `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.15954v1); full text read via alphaXiv (https://arxiv.org/abs/2606.15954). Raw fulltext capture pending backfill.
