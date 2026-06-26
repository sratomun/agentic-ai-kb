---
type: source
source_type: arxiv
title: "LOGIGEN: Logic-Driven Generation of Verifiable Agentic Tasks"
authors: Yucheng Zeng, Weipeng Lu, Linyun Liu, Shupeng Li et al.
url: https://arxiv.org/abs/2603.00540v1
date: 2026-02-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agent-protocols, agent-memory, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# LOGIGEN: Logic-Driven Generation of Verifiable Agentic Tasks

**arXiv:** [2603.00540v1](https://arxiv.org/abs/2603.00540v1) · 2026-02-28 · cs.AI
**Authors:** Yucheng Zeng, Weipeng Lu, Linyun Liu, Shupeng Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The evolution of Large Language Models (LLMs) from static instruction-followers to autonomous agents necessitates operating within complex, stateful environments to achieve precise state-transition objectives. However, this paradigm is bottlenecked by data scarcity, as existing tool-centric reverse-synthesis pipelines fail to capture the rigorous logic of real-world applications. We introduce \textbf{LOGIGEN}, a logic-driven framework that synthesizes verifiable training data based on three core pillars: \textbf{Hard-Compiled Policy Grounding}, \textbf{Logic-Driven Forward Synthesis}, and \textbf{Deterministic State Verification}. Specifically, a Triple-Agent Orchestration is employed: the \textbf{Architect} compiles natural-language policy into database constraints to enforce hard rules; the \textbf{Set Designer} initializes boundary-adjacent states to trigger critical policy conflicts; and the \textbf{Explorer} searches this environment to discover causal solution paths. This framework yields a dataset of 20,000 complex tasks across 8 domains, where validity is strictly guaranteed by checking exact state equivalence. Furthermore, we propose a verification-based training protocol where Supervised Fine-Tuning (SFT) on verifiable trajectories establishes compliance with hard-compiled policy, while Reinforcement Learning (RL) guided by dense state-rewards refines long-horizon goal achievement. On $τ^2$-Bench, LOGIGEN-32B(RL) achieves a \textbf{79.5\% success rate}, substantially outperforming the base model (40.7\%). These results demonstrate that logic-driven synthesis combined with verification-based training effectively constructs the causally valid trajectories needed for next-generation agents.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00540v1)
