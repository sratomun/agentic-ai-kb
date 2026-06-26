---
type: source
source_type: arxiv
title: "FinCom: A Financial Multi-Agent Demo with Disagree-or-Commit Deliberation"
authors: Chao Peter Yang, Zixiao Tan, Kaisen Yao, Ziyu Zhou et al.
url: https://arxiv.org/abs/2606.00939v1
date: 2026-05-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.MA
tags: [recommendation-agents, finance-agents, agent-reliability, agent-security, agent-protocols, arxiv, auto-ingested]
---

# FinCom: A Financial Multi-Agent Demo with Disagree-or-Commit Deliberation

**arXiv:** [2606.00939v1](https://arxiv.org/abs/2606.00939v1) · 2026-05-31 · cs.MA
**Authors:** Chao Peter Yang, Zixiao Tan, Kaisen Yao, Ziyu Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent systems powered by large language models (LLMs) are increasingly used for financial analysis and decision support. However, existing coordination schemes, especially those emphasizing consensus or debate, are vulnerable to sycophancy: agents conform to peer reasoning instead of evidence, leading to premature agreement and degraded outcomes. We introduce FinCom (Financial Committee), a governed multi-agent framework and interactive system that operationalizes the Disagree-or-Commit (DoC) protocol to embed structured dissent into financial AI committees. A central Supervisor orchestrates three ReAct-enabled specialist agents: Research, Quantitative, and Risk. Each agent is equipped with role-specific tools for retrieval, computation, and stress testing. During deliberation, agents must either explicitly critique or commit to their peers' reasoning before converging on a unified recommendation. This demonstration showcases how FinCom supports committee-style financial analysis through coordinated multi-agent interaction, including structured report generation and interactive decision support. Evaluated across the most recent financial agent benchmark, in addition to 90 internal handcrafted financial tasks using an LLM-as-a-Judge protocol, DoC improves reasoning accuracy and risk awareness significantly over a consensus-seeking baseline on both an in-house and external evaluation set. By reframing disagreement as a governance primitive rather than noise, FinCom offers a lightweight, prompt-only recipe for improving accountability, transparency, and epistemic robustness in agentic financial systems.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.00939v1)
