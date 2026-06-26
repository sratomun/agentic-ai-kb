---
type: source
source_type: arxiv
title: "Tool-Aware Optimization with Entropy Guidance for Efficient Agentic Reinforcement Learning"
authors: Hongye Cao, Nuo Yan, Haoyuan Deng, Ziwei Wang et al.
url: https://arxiv.org/abs/2606.03762v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.LG
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Tool-Aware Optimization with Entropy Guidance for Efficient Agentic Reinforcement Learning

**arXiv:** [2606.03762v1](https://arxiv.org/abs/2606.03762v1) · 2026-06-02 · cs.LG
**Authors:** Hongye Cao, Nuo Yan, Haoyuan Deng, Ziwei Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic reinforcement learning (RL) equips large language models (LLMs) with tool-use capabilities that substantially improve reasoning on complex tasks. However, integrating external tools often destabilizes training: over-reliance on tools can induce input distribution shift, while overly conservative tool use limits effective exploration. To address this issue, we propose a unified framework TAO-RL that couples tool-aware trajectory filtering with entropy-guided exploration for efficient policy optimization. Specifically, at the data level, TAO-RL filters rollout trajectories along two criteria: discarding those where all tool invocations fail to execute, and removing those where all rollouts are either correct or incorrect, as both cases yield degenerate advantage estimates that contribute no discriminative learning signal. This joint filtering retains data that are both tool-capable and informative, establishing a high-quality training distribution. At the algorithmic level, we introduce a tool-aware entropy-guided bonus that reshapes the advantage function at post-tool-call tokens, encouraging the policy to explore more diverse reasoning paths at critical decision points. These two components are mutually reinforcing: trajectory filtering establishes a clean and informative training foundation, while entropy-guided exploration drives stronger reasoning behaviors at critical tool-interaction junctures. Extensive experiments on 7 challenging reasoning benchmarks across 3 model scales demonstrate the superiority of TAO-RL over existing methods.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03762v1)
