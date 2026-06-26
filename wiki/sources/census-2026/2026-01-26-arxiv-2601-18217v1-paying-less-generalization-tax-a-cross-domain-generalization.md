---
type: source
source_type: arxiv
title: "Paying Less Generalization Tax: A Cross-Domain Generalization Study of RL Training for LLM Agents"
authors: Zhihan Liu, Lin Guan, Yixin Nie, Kai Zhang et al.
url: https://arxiv.org/abs/2601.18217v1
date: 2026-01-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [agent-reliability, agentic-rl, arxiv, auto-ingested]
---

# Paying Less Generalization Tax: A Cross-Domain Generalization Study of RL Training for LLM Agents

**arXiv:** [2601.18217v1](https://arxiv.org/abs/2601.18217v1) · 2026-01-26 · cs.AI
**Authors:** Zhihan Liu, Lin Guan, Yixin Nie, Kai Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generalist LLM agents are often post-trained on a narrow set of environments but deployed across far broader, unseen domains. In this work, we investigate the challenge of agentic post-training when the eventual test domains are unknown. Specifically, we analyze which properties of reinforcement learning (RL) environments and modeling choices have the greatest influence on out-of-domain performance. First, we identify two environment axes that strongly correlate with cross-domain generalization: (i) state information richness, i.e., the amount of information for the agent to process from the state, and (ii) planning complexity, estimated via goal reachability and trajectory length under a base policy. Notably, domain realism and text-level similarity are not the primary factors; for instance, the simple grid-world domain Sokoban leads to even stronger generalization in SciWorld than the more realistic ALFWorld. Motivated by these findings, we further show that increasing state information richness alone can already effectively improve cross-domain robustness. We propose a randomization technique, which is low-overhead and broadly applicable: add small amounts of distractive goal-irrelevant features to the state to make it richer without altering the task. Beyond environment-side properties, we also examine several modeling choices: (a) SFT warmup or mid-training helps prevent catastrophic forgetting during RL but undermines generalization to domains that are not included in the mid-training datamix; and (b) turning on step-by-step thinking during RL, while not always improving in-domain performance, plays a crucial role in preserving generalization.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]]
- **Entities:** [[alfworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.18217v1)
