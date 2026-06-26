---
type: source
source_type: arxiv
title: "SearchGym: Bootstrapping Real-World Search Agents via Cost-Effective and High-Fidelity Environment Simulation"
authors: Xichen Zhang, Ziyi He, Yinghao Zhu, Sitong Wu et al.
url: https://arxiv.org/abs/2601.14615v1
date: 2026-01-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [knowledge-graph, agentic-rl, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# SearchGym: Bootstrapping Real-World Search Agents via Cost-Effective and High-Fidelity Environment Simulation

**arXiv:** [2601.14615v1](https://arxiv.org/abs/2601.14615v1) · 2026-01-21 · cs.CL
**Authors:** Xichen Zhang, Ziyi He, Yinghao Zhu, Sitong Wu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Search agents have emerged as a pivotal paradigm for solving open-ended, knowledge-intensive reasoning tasks. However, training these agents via Reinforcement Learning (RL) faces a critical dilemma: interacting with live commercial Web APIs is prohibitively expensive, while relying on static data snapshots often introduces noise due to data misalignment. This misalignment generates corrupted reward signals that destabilize training by penalizing correct reasoning or rewarding hallucination. To address this, we propose SearchGym, a simulation environment designed to bootstrap robust search agents. SearchGym employs a rigorous generative pipeline to construct a verifiable knowledge graph and an aligned document corpus, ensuring that every reasoning task is factually grounded and strictly solvable. Building on this controllable environment, we introduce SearchGym-RL, a curriculum learning methodology that progressively optimizes agent policies through purified feedback, evolving from basic interactions to complex, long-horizon planning. Extensive experiments across the Llama and Qwen families demonstrate strong Sim-to-Real generalization. Notably, our Qwen2.5-7B-Base model trained within SearchGym surpasses the web-enhanced ASearcher baseline across nine diverse benchmarks by an average relative margin of 10.6%. Our results validate that high-fidelity simulation serves as a scalable and highly cost-effective methodology for developing capable search agents.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[llama]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.14615v1)
