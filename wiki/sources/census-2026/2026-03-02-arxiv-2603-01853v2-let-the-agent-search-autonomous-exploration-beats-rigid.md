---
type: source
source_type: arxiv
title: "Let the Agent Search: Autonomous Exploration Beats Rigid Workflows in Temporal Question Answering"
authors: Xufei Lv, Jiahui Yang, Haoyuan Sun, Xialin Su et al.
url: https://arxiv.org/abs/2603.01853v2
date: 2026-03-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.CL
tags: [knowledge-graph, agent-reliability, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Let the Agent Search: Autonomous Exploration Beats Rigid Workflows in Temporal Question Answering

**arXiv:** [2603.01853v2](https://arxiv.org/abs/2603.01853v2) · 2026-03-02 · cs.CL
**Authors:** Xufei Lv, Jiahui Yang, Haoyuan Sun, Xialin Su et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Temporal Knowledge Graph Question Answering (TKGQA) is challenging because it requires multi-hop reasoning under complex temporal constraints. Recent LLM-based approaches have improved semantic modeling for this task, but many still rely on fixed reasoning workflows or costly post-training, which can limit adaptability and make error recovery difficult. We show that enabling an off-the-shelf Large Language Model (LLM) to determine its next action is already effective in a zero-shot setting. Based on this insight, we propose AT2QA, an Autonomous and Training-free Agent for TKG Question Answering. AT2QA empowers the LLM to iteratively interact with the TKG via a generic search tool, inherently enabling autonomous exploration and dynamic self-correction during reasoning. To further elicit the LLM's potential for complex temporal reasoning, we introduce a training-free experience mining mechanism that distills a compact few-shot demonstration library from successful self-generated trajectories. AT2QA also yields a transparent audit trail for every prediction. Experiments on three challenging benchmarks -- MultiTQ, Timeline-CronQuestion, and Timeline-ICEWS-Actor -- show that AT2QA achieves new state-of-the-art performance, surpassing the strongest baselines by 10.7, 4.9, and 11.2 absolute points, respectively. Our code is available at https://github.com/AT2QA-Official-Code/AT2QA-Official-Code

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01853v2)
