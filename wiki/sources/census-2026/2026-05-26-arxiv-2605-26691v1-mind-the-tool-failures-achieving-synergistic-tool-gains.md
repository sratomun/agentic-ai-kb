---
type: source
source_type: arxiv
title: "Mind the Tool Failures: Achieving Synergistic Tool Gains for Medical Agents"
authors: Yunhui Gan, Tan Pan, Kaiyu Guo, Limei Han et al.
url: https://arxiv.org/abs/2605.26691v1
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 15
primary: cs.AI
tags: [recommendation-agents, clinical-agents, agent-reliability, agentic-rl, tool-use, arxiv, auto-ingested]
---

# Mind the Tool Failures: Achieving Synergistic Tool Gains for Medical Agents

**arXiv:** [2605.26691v1](https://arxiv.org/abs/2605.26691v1) · 2026-05-26 · cs.AI
**Authors:** Yunhui Gan, Tan Pan, Kaiyu Guo, Limei Han et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Medical AI agents increasingly use external tools for diagnosis, treatment recommendation, and evidence retrieval, yet most existing approaches assume that task-appropriate tools are reliable within their intended scope. This assumption is fragile in real clinical settings, where even relevant tools may fail on challenging instances and lead to unsafe downstream decisions. To address this issue, we study medical tool use under imperfect-tool settings to correct failure instances missed by individual tools. Instance-dependent failure patterns create a gap between the best fixed single tool and an ideal instance-wise selector, which we refer to as the Single-Oracle risk gap. The core challenge is that conventional task-level tool selection cannot realize this gap, as it is inherently bounded by the performance of the best single tool. Motivated by this observation, we therefore account for instance-level heterogeneity and formulate tool use as an instance-level selection problem. Particularly, we propose a GRPO-based reinforcement learning framework with rewards for probabilistic risk minimization and disagreement-aware synergy learning, which promotes instance-level correction of erroneous tool consensus. Furthermore, an entropy-guided sampling strategy is adopted to upweight high-disagreement instances, which provide stronger signals for learning instance-specific tool synergy. These two components complement each other in mitigating instance-level heterogeneity and improving tool synergy. Experiments on two tasks and seven medical benchmarks show that our method consistently achieves robust and stable improvements over a broad range of baselines, highlighting the importance of synergy-aware tool use for reliable medical agentic systems.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26691v1)
