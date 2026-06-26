---
type: source
source_type: arxiv
title: "LLM4Cov: Execution-Aware Agentic Learning for High-coverage Testbench Generation"
authors: Hejia Zhang, Zhongming Yu, Chia-Tung Ho, Haoxing Ren et al.
url: https://arxiv.org/abs/2602.16953v3
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# LLM4Cov: Execution-Aware Agentic Learning for High-coverage Testbench Generation

**arXiv:** [2602.16953v3](https://arxiv.org/abs/2602.16953v3) · 2026-02-18 · cs.AI
**Authors:** Hejia Zhang, Zhongming Yu, Chia-Tung Ho, Haoxing Ren et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Execution-aware LLM agents offer a promising paradigm for learning from tool feedback, but such feedback can be expensive and slow to obtain, making online reinforcement learning (RL) less practical in certain scenarios. High-coverage hardware verification exemplifies this challenge due to its reliance on industrial simulators and non-differentiable execution signals. We propose LLM4Cov, an offline agent-learning framework that models verification as single-step state transitions guided by deterministic evaluators. Building on this formulation, we introduce execution-validated data curation, policy-aware agentic data synthesis, and worst-state-prioritized sampling to enable scalable learning under execution constraints. We further curate a reality-aligned benchmark adapted from an existing verification suite through a revised evaluation protocol. Using the proposed pipeline, a compact 4B-parameter model achieves 69.2% pass rate and 90.4% average coverage in CVDP-ECov under agentic evaluation, outperforming its teacher by 5.3% and 10.5%, demonstrating competitive performance against models an order of magnitude larger.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16953v3)
