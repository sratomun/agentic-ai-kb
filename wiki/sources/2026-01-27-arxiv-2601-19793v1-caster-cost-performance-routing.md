---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "CASTER: Breaking the Cost-Performance Barrier in Multi-Agent Orchestration via Context-Aware Strategy for Task Efficient Routing"
authors: Shanyv Liu, Xuyang Yuan, Tao Chen et al. (China University of Petroleum; Univ. of Houston)
url: https://arxiv.org/abs/2601.19793
date: 2026-01-27
citationCount: 0
influentialCitationCount: 0
velocity: recent
ingested: 2026-06-26
tags: [arxiv, agent-finops, routing, multi-agent-systems, intent-routing, agentic-ai, 2026]
---

# CASTER: Breaking the Cost-Performance Barrier in Multi-Agent Orchestration via Context-Aware Strategy for Task Efficient Routing

**arXiv [2601.19793](https://arxiv.org/abs/2601.19793)** · 2026-01-27 · **recent** · Shanyv Liu, Xuyang Yuan, Tao Chen et al.

**Significance.** The "route" layer of [[agent-finops]] — predicting difficulty *upfront* beats reactive FrugalGPT-style cascades on both cost and quality.

## Abstract
Graph-based Multi-Agent Systems (MAS) enable complex cyclic workflows but suffer from inefficient static model allocation, where deploying strong models uniformly wastes computation on trivial sub-tasks. We propose CASTER (Context-Aware Strategy for Task Efficient Routing), a lightweight router for dynamic model selection in graph-based MAS. CASTER employs a Dual-Signal Router that combines semantic embeddings with structural meta-features to estimate task difficulty. During training, the router self-optimizes through a Cold Start to Iterative Evolution paradigm, learning from its own routing failures via on-policy negative feedback. Experiments using LLM-as-a-Judge evaluation across Software Engineering, Data Analysis, Scientific Discovery, and Cybersecurity demonstrate that CASTER reduces inference cost by up to 72.4% compared to strong-model baselines while matching their success rates, and consistently outperforms both heuristic routing and FrugalGPT across all domains.

## From the paper (full-text)
**Contribution / method.** A lightweight neural router that intercepts each agent node in a LangGraph MAS and picks the backend (strong vs weak model) before execution. It is a **Dual-Branch Feature Fusion Network**: a semantic branch (1536-dim text-embedding-3-small → 128-dim) fused with a 6-dim structural meta-feature branch (→16-dim) into a classifier emitting p(Strong|x) at a 0.5 threshold. Trained via **Cold Start → Iterative Evolution** using **on-policy negative feedback** — deliberately learning from its own boundary failures (the paper shows random exploration pollutes the training data).
**Results.** **Up to 72.4% cost reduction** vs strong-model baseline; per-domain unit-cost cuts 23.4–54.3% (e.g., Software $0.0392→$0.0179). Matches or beats strong-model quality while cheaper — Science 95.3 vs 95.2 and Security 86.2 vs 85.5 both **beat** the strong model by mitigating "over-thinking" on simple sub-tasks. **Pareto-dominates FrugalGPT**: 20.7–48.0% lower total cost AND higher quality across all four domains (Software $0.58 vs $1.11 at 80.8 vs 79.8), by avoiding the cascade's fail-then-retry double-billing. Also shields against weak-model "logic collapse" (Web Security 48.0→86.0).
**Takeaway.** A tiny embeddings-plus-metadata router that predicts difficulty before spending delivers ~72% cost cuts at strong-model quality and beats FrugalGPT on the frontier — predicting need beats cascading and retrying.

## Graph
- **Concepts:** [[agent-finops|Agent FinOps]] · [[intent-routing|Intent routing]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[langgraph]] · [[llm-as-judge]]
- **Raw:** census record `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.19793v1); full text read via alphaXiv (https://arxiv.org/abs/2601.19793). Raw fulltext capture pending backfill.
