---
type: source
source_type: arxiv
title: "Does RL Expand the Capability Boundary of LLM Agents? A PASS@(k,T) Analysis"
authors: Zhiyuan Zhai, Wenjing Yan, Xiaodan Shao, Xin Wang
url: https://arxiv.org/abs/2604.14877v1
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.LG
tags: [agent-reliability, agentic-rl, tool-use, arxiv, auto-ingested]
---

# Does RL Expand the Capability Boundary of LLM Agents? A PASS@(k,T) Analysis

**arXiv:** [2604.14877v1](https://arxiv.org/abs/2604.14877v1) · 2026-04-16 · cs.LG
**Authors:** Zhiyuan Zhai, Wenjing Yan, Xiaodan Shao, Xin Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Does reinforcement learning genuinely expand what LLM agents can do, or merely make them more reliable? For static reasoning, recent work answers the second: base and RL pass@k curves converge at large k. We ask whether this holds for agentic tool use, where T rounds of interaction enable compositional strategies that re-sampling cannot recover. We introduce PASS@(k,T), a two-dimensional metric that jointly varies sampling budget k and interaction depth T, separating capability expansion from efficiency improvement. Our main finding is that, contrary to the static-reasoning result, tool-use RL genuinely enlarges the capability boundary: the RL agent's pass-curve pulls above the base model's and the gap widens at large k rather than converging. The expansion is specific to compositional, sequential information gathering; on simpler tasks RL behaves as prior work predicts. Under matched training data, supervised fine-tuning regresses the boundary on the same compositional tasks, isolating self-directed exploration as the causal factor. Mechanism analysis shows RL reweights the base strategy distribution toward the subset whose downstream reasoning more often yields a correct answer, with the improvement concentrated on how the agent integrates retrieved information. These results reconcile optimistic and pessimistic readings of RL for LLMs: both are correct, on different task types.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14877v1)
