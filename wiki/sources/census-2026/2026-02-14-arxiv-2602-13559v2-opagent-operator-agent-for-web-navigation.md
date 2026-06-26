---
type: source
source_type: arxiv
title: "OpAgent: Operator Agent for Web Navigation"
authors: Yuyu Guo, Wenjie Yang, Siyuan Yang, Ziyang Liu et al.
url: https://arxiv.org/abs/2602.13559v2
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [computer-use-agents, embodied-agents, agent-reliability, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# OpAgent: Operator Agent for Web Navigation

**arXiv:** [2602.13559v2](https://arxiv.org/abs/2602.13559v2) · 2026-02-14 · cs.AI
**Authors:** Yuyu Guo, Wenjie Yang, Siyuan Yang, Ziyang Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
To fulfill user instructions, autonomous web agents must contend with the inherent complexity and volatile nature of real-world websites. Conventional paradigms predominantly rely on Supervised Fine-Tuning (SFT) or Offline Reinforcement Learning (RL) using static datasets. However, these methods suffer from severe distributional shifts, as offline trajectories fail to capture the stochastic state transitions and real-time feedback of unconstrained wide web environments. In this paper, we propose a robust Online Reinforcement Learning WebAgent, designed to optimize its policy through direct, iterative interactions with unconstrained wide websites. Our approach comprises three core innovations: 1) Hierarchical Multi-Task Fine-tuning: We curate a comprehensive mixture of datasets categorized by functional primitives -- Planning, Acting, and Grounding -- establishing a Vision-Language Model (VLM) with strong instruction-following capabilities for Web GUI tasks. 2) Online Agentic RL in the Wild: We develop an online interaction environment and fine-tune the VLM using a specialized RL pipeline. We introduce a Hybrid Reward Mechanism that combines a ground-truth-agnostic WebJudge for holistic outcome assessment with a Rule-based Decision Tree (RDT) for progress reward. This system effectively mitigates the credit assignment challenge in long-horizon navigation. Notably, our RL-enhanced model achieves a 38.1\% success rate (pass@5) on WebArena, outperforming all existing monolithic baselines. 3) Operator Agent: We introduce a modular agentic framework, namely \textbf{OpAgent}, orchestrating a Planner, Grounder, Reflector, and Summarizer. This synergy enables robust error recovery and self-correction, elevating the agent's performance to a new State-of-the-Art (SOTA) success rate of \textbf{71.6\%}.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Entities:** [[webarena]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13559v2)
