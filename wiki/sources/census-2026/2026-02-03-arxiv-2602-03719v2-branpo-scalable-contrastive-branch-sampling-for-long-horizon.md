---
type: source
source_type: arxiv
title: "BranPO: Scalable Contrastive Branch Sampling for Long-Horizon Agentic Reinforcement Learning"
authors: Yubao Zhao, Weiquan Huang, Sudong Wang, Ruochen Zhao et al.
url: https://arxiv.org/abs/2602.03719v2
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agentic-rl, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# BranPO: Scalable Contrastive Branch Sampling for Long-Horizon Agentic Reinforcement Learning

**arXiv:** [2602.03719v2](https://arxiv.org/abs/2602.03719v2) · 2026-02-03 · cs.CL
**Authors:** Yubao Zhao, Weiquan Huang, Sudong Wang, Ruochen Zhao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic reinforcement learning enables large language models to perform multi-turn planning and tool use, but long-horizon training remains challenging under sparse trajectory-level rewards, where a single outcome is uniformly assigned to all decisions. Prior methods introduce finer-grained supervision via tree-based exploration or process-level evaluation, but often incur high cost or produce noisy credit signals. In agentic trajectories, early mistakes may still be corrected by later actions, while seemingly promising intermediate states can fail due to poor subsequent decisions. We call this property non-monotonic correctness, which makes outcome rewards or state values insufficient for guiding what actions should be taken from each state. To address this, we propose Branching Relative Policy Optimization (\textbf{BranPO}), a value-free method that constructs localized contrastive supervision without dense rewards. BranPO truncates trajectories at intermediate prefixes and resamples continuations to form contrastive branches that share the same prefix but diverge in final outcomes, thereby isolating decisions that drive success or failure. We further introduce difficulty-aware branch sampling and Redundant Step Masking to improve sampling efficiency and suppress redundant updates. Experiments show that BranPO consistently outperforms diverse baseline categories across multiple multi-hop QA benchmarks without additional training cost, and generalizes to broader long-horizon agentic tasks with consistent improvements. Our code is available at https://github.com/YubaoZhao/BranPO.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03719v2)
