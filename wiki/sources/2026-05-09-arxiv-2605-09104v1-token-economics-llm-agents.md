---
type: source
source_type: arxiv
kind: survey
depth: full-text
title: "Token Economics for LLM Agents: A Dual-View Study from Computing and Economics"
authors: Yuxi Chen, Junming Chen, Chenyu He et al. (Zhejiang University + Alibaba Cloud)
url: https://arxiv.org/abs/2605.09104
date: 2026-05-09
citationCount: 0
influentialCitationCount: 0
velocity: recent
ingested: 2026-06-26
tags: [arxiv, agent-finops, token-economics, survey, agentic-ai, 2026]
---

# Token Economics for LLM Agents: A Dual-View Study from Computing and Economics

**arXiv [2605.09104](https://arxiv.org/abs/2605.09104)** · 2026-05-09 · **recent (survey)** · Yuxi Chen, Junming Chen, Chenyu He et al.

**Significance.** The theory hub for [[agent-finops]] — the first survey to formalize tokens as an economic primitive and unify the computing and economics views of agent cost.

## Abstract
As LLM agents evolve, tokens have emerged as the core economic primitives of Agentic AI. However, their exponential consumption introduces severe computational, collaborative, and security bottlenecks. Current surveys remain fragmented across system optimization, architecture design, and trust, lacking a unified framework to evaluate the fundamental trade-off between output quality and economic cost. To bridge this gap, this survey presents the first comprehensive survey of Token Economics. By unifying computer science and economics, we conceptualize tokens as production factors, exchange mediums, and units of account. We synthesize existing literature across a four-dimensional taxonomy: (1) Micro-level (Single Agent): optimizing budget-constrained factor substitution via neoclassical firm theory; (2) Meso-level (Multi-Agent Systems): minimizing collaboration friction using transaction cost and principal-agent theories; (3) Macro-level (Agent Ecosystems): addressing congestion externalities and pricing via mechanism design; (4) Security: internalizing adversarial threats as endogenous economic constraints. Finally, we outline frontier directions, including differentiable token budgets and dynamic markets.

## From the paper (full-text)
**Contribution / method.** A survey and conceptual framework (no original experiments). Treats tokens as production factor / exchange medium / unit of account, and frames the central problem as a constrained optimization — minimize total token cost subject to a quality floor (min TC s.t. Y ≥ Z). Organizes the literature into a four-level taxonomy: micro (single-agent factor substitution, neoclassical firm theory), meso (multi-agent transaction-cost and principal-agent theory), macro (ecosystem congestion/pricing via mechanism design), and security (adversarial cost as endogenous constraint). Maps ~190 cited works onto this scaffold.
**Results.** Not applicable — no measured results. Names forward trends and opportunities including "Differentiable Token Budgeting" and "Real-Time Token Markets and Dynamic Pricing."
**Takeaway.** Use this as the citation hub and shared vocabulary for agent cost — treat tokens as an economic primitive and budget them with firm theory, transaction-cost economics, and mechanism design; it grounds the *why*, while the systems papers (CASTER/ZEBRA/Green SARC/EnumGRPO) supply the *how* and the numbers.

## Graph
- **Concepts:** [[agent-finops|Agent FinOps]] · [[agent-economies|Agent economies]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** census record `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.09104v1); full text read via alphaXiv (https://arxiv.org/abs/2605.09104). Raw fulltext capture pending backfill.
