---
type: source
source_type: arxiv
title: "Absorbing Complexity: An Interaction-Native Knowledge Harness for Financial LLM Agents"
authors: Ailiya Borjigin, Igor Stadnyk, Ben Bilski, Maksym Chikita et al.
url: https://arxiv.org/abs/2606.01886v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [finance-agents, knowledge-graph, agent-memory, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Absorbing Complexity: An Interaction-Native Knowledge Harness for Financial LLM Agents

**arXiv:** [2606.01886v1](https://arxiv.org/abs/2606.01886v1) · 2026-06-01 · cs.AI
**Authors:** Ailiya Borjigin, Igor Stadnyk, Ben Bilski, Maksym Chikita et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Financial AI agents often fail for a simple reason: they make users carry the complexity. A user must repeatedly restate goals, risk preferences, portfolio context, past judgments, and shifting market assumptions, while the agent answers, retrieves, acts, and forgets. In finance, this is not just inconvenient. In tasks such as market analysis, copy-trading review, and trade preparation, forgotten context and stale memory can create latency, repeated errors, weak auditability, and unsafe decisions. We propose the interaction-native knowledge harness (InKH), an architecture for financial LLM agents that absorbs complexity into the system. InKH converts user, market, portfolio, and tool events into structured operational knowledge. It uses passive knowledge injection to assemble a bounded working context buffer before the main model step, temporal graph memory for low-latency retrieval, a wiki audit surface for human-readable governance, and background extraction with maturity, decay, and write-time invalidation. We evaluate InKH on a reproducible controlled synthetic benchmark with 24 random seeds, 4 rounds, 80 episodes per round, and 6 baselines, producing 46,080 baseline-conditioned evaluations. InKH achieves mean task quality of 0.815 at 900 ms latency. Compared with agent-driven wiki-walk memory, it reduces latency by 82.95 percent, token cost by 82.29 percent, and stale-knowledge usage by 96.58 percent, while improving quality by 0.108 and traceability by 0.461. Compared with a temporal-graph system without invalidation, it improves quality by 0.050 and reduces stale-memory usage by 96.58 percent with comparable serving cost. The results support a design thesis for financial AI: adoption happens when complexity is absorbed by the system rather than transferred to the user. The benchmark validates architecture-level behavior, not live trading performance.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01886v1)
