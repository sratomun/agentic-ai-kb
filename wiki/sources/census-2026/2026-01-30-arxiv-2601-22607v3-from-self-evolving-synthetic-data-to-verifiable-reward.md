---
type: source
source_type: arxiv
title: "From Self-Evolving Synthetic Data to Verifiable-Reward RL: Post-Training Multi-turn Interactive Tool-Using Agents"
authors: Jiaxuan Gao, Jiaao Chen, Chuyi He, Shusheng Xu et al.
url: https://arxiv.org/abs/2601.22607v3
date: 2026-01-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agent-reliability, self-evolving-agents, agentic-rl, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# From Self-Evolving Synthetic Data to Verifiable-Reward RL: Post-Training Multi-turn Interactive Tool-Using Agents

**arXiv:** [2601.22607v3](https://arxiv.org/abs/2601.22607v3) · 2026-01-30 · cs.AI
**Authors:** Jiaxuan Gao, Jiaao Chen, Chuyi He, Shusheng Xu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Interactive tool-using agents must solve real-world tasks via multi-turn interaction with both humans and external environments, requiring dialogue state tracking, multi-step tool execution, while following complex instructions. Post-training such agents is challenging because synthesis for high-quality multi-turn tool-use data is difficult to scale, and reinforcement learning (RL) could face noisy signals caused by user simulation, leading to degraded training efficiency. We propose a unified framework that combines a self-evolving data agent with verifier-based RL. Our system, EigenData, is a hierarchical multi-agent engine that synthesizes tool-grounded dialogues together with executable per-instance checkers, and improves generation reliability via closed-loop self-evolving process that updates prompts and workflow. Building on the synthetic data, we develop an RL recipe that first fine-tunes the user model and then applies GRPO-style training with trajectory-level group-relative advantages and dynamic filtering, yielding consistent improvements beyond SFT. Evaluated on tau^2-bench, our best model reaches 73.0% pass^1 on Airline and 98.3% pass^1 on Telecom, matching or exceeding frontier models. Overall, our results suggest a scalable pathway for bootstrapping complex tool-using behaviors without expensive human annotation.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.22607v3)
