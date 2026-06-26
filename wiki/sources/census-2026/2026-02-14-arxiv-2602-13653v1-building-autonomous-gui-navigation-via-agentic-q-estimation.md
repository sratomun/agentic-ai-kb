---
type: source
source_type: arxiv
title: "Building Autonomous GUI Navigation via Agentic-Q Estimation and Step-Wise Policy Optimization"
authors: Yibo Wang, Guangda Huzhang, Yuwei Hu, Yu Xia et al.
url: https://arxiv.org/abs/2602.13653v1
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [computer-use-agents, embodied-agents, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Building Autonomous GUI Navigation via Agentic-Q Estimation and Step-Wise Policy Optimization

**arXiv:** [2602.13653v1](https://arxiv.org/abs/2602.13653v1) · 2026-02-14 · cs.AI
**Authors:** Yibo Wang, Guangda Huzhang, Yuwei Hu, Yu Xia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Multimodal Large Language Models (MLLMs) have substantially driven the progress of autonomous agents for Graphical User Interface (GUI). Nevertheless, in real-world applications, GUI agents are often faced with non-stationary environments, leading to high computational costs for data curation and policy optimization. In this report, we introduce a novel MLLM-centered framework for GUI agents, which consists of two components: agentic-Q estimation and step-wise policy optimization. The former one aims to optimize a Q-model that can generate step-wise values to evaluate the contribution of a given action to task completion. The latter one takes step-wise samples from the state-action trajectory as inputs, and optimizes the policy via reinforcement learning with our agentic-Q model. It should be noticed that (i) all state-action trajectories are produced by the policy itself, so that the data collection costs are manageable; (ii) the policy update is decoupled from the environment, ensuring stable and efficient optimization. Empirical evaluations show that our framework endows Ovis2.5-9B with powerful GUI interaction capabilities, achieving remarkable performances on GUI navigation and grounding benchmarks and even surpassing contenders with larger scales.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13653v1)
