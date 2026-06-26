---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ZEBRA: Zero-shot Budgeted Resource Allocation for LLM Orchestration"
authors: May Hamri, Inbal Talgam-Cohen (Tel Aviv University)
url: https://arxiv.org/abs/2605.20485
date: 2026-05-19
citationCount: 0
influentialCitationCount: 0
velocity: recent
ingested: 2026-06-26
tags: [arxiv, agent-finops, budget-allocation, orchestration, agentic-ai, 2026]
---

# ZEBRA: Zero-shot Budgeted Resource Allocation for LLM Orchestration

**arXiv [2605.20485](https://arxiv.org/abs/2605.20485)** · 2026-05-19 · **recent** (SCALE @ ICML 2026 workshop) · May Hamri, Inbal Talgam-Cohen

**Significance.** Answers the question budget-aware methods skip — not *whether* the budget is respected but *how to split it across phases* of a multi-agent pipeline. The "allocate" layer of [[agent-finops]].

## Abstract
As autonomous agents increasingly execute end-to-end tasks under fixed monetary budgets, the pressing open question shifts from whether the budget is respected, to how to spend it effectively. Existing budget-aware methods typically control reasoning step-by-step within a single agent, or learn resource allocation policies via RL. None address how to split a budget across the composing phases of a multi-agent pipeline at inference time. We propose ZEBRA, a zero-shot framework that reduces multi-phase budget allocation to a continuous nonlinear knapsack problem: an LLM controller estimates per-phase utility curves, and a water-filling search on the Lagrange multiplier returns the per-phase split. Additive and multiplicative aggregations are unified under the same solver. On a 150-task APPS coding benchmark, both ZEBRA variants outperform LLM-direct on every aggregate metric. At a budget of α = 0.5 of the unconstrained spend, ZEBRA recovers 94.4% of unconstrained quality, versus 88.1% for LLM-direct. The advantage transfers beyond coding: on a 3-phase HotpotQA pipeline, ZEBRA beats LLM-direct by 14.3pp.

## From the paper (full-text)
**Contribution / method.** Adds an **allocation agent** above a Plan→Decompose→Implement→Refine LangGraph pipeline. Instead of letting an LLM output budget shares directly, it prompts the LLM to estimate each phase's **performance–budget utility curve** (saturating exponential f(x)=a(1−e^{−bx})), turning the split into a **continuous nonlinear knapsack** solved by water-filling / bisection on the Lagrange multiplier in O(n log 1/ε). Multiplicative objectives fold into the additive solver via a log transform. Fully zero-shot — no RL, fine-tuning, or training data.
**Results.** At tight budget **α=0.5, ZEBRA recovers 94.4% of unconstrained quality vs 88.1% for LLM-direct** at identical spend (~$0.011/task); at α=0.8, 98.1% vs 94.3%. Gains concentrate on hard tasks (+6.7 points / +10.0pp success on medium tasks at α=0.5, p_BH=3.7×10⁻⁴; easy tasks tie). Transfer to **HotpotQA (3-phase QA): +14.3pp retention (92.1% vs 77.8%, p≈10⁻⁴)**, with the allocation adapting (near-balanced split for QA vs refine-skewed for coding). Both variants beat LLM-direct at p<0.01 (paired Wilcoxon, n=150).
**Takeaway.** Don't let the model divide its own budget — elicit per-phase utility curves and hand the split to a knapsack solver; it recovers ~94% of full quality at half the spend, and the edge grows exactly when the budget binds.

## Graph
- **Concepts:** [[agent-finops|Agent FinOps]] · [[multi-agent-systems|Multi-agent systems]] · [[intent-routing|Intent routing]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[langgraph]]
- **Raw:** census record `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.20485v1); full text read via alphaXiv (https://arxiv.org/abs/2605.20485). Raw fulltext capture pending backfill.
