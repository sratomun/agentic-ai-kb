---
type: source
source_type: arxiv
title: "CM2: Reinforcement Learning with Checklist Rewards for Multi-Turn and Multi-Step Agentic Tool Use"
authors: Zhen Zhang, Kaiqiang Song, Xun Wang, Yebowen Hu et al.
url: https://arxiv.org/abs/2602.12268v2
date: 2026-02-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agentic-rl, tool-use, arxiv, auto-ingested]
---

# CM2: Reinforcement Learning with Checklist Rewards for Multi-Turn and Multi-Step Agentic Tool Use

**arXiv:** [2602.12268v2](https://arxiv.org/abs/2602.12268v2) · 2026-02-12 · cs.AI
**Authors:** Zhen Zhang, Kaiqiang Song, Xun Wang, Yebowen Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
AI agents are increasingly used to solve real-world tasks by reasoning over multi-turn user interactions and invoking external tools. However, applying reinforcement learning to such settings remains difficult: realistic objectives often lack verifiable rewards and instead emphasize open-ended behaviors; moreover, RL for multi-turn, multi-step agentic tool use is still underexplored; and building and maintaining executable tool environments is costly, limiting scale and coverage. We propose CM2, an RL framework that replaces verifiable outcome rewards with checklist rewards. CM2 decomposes each turn's intended behavior into fine-grained binary criteria with explicit evidence grounding and structured metadata, turning open-ended judging into more stable classification-style decisions. To balance stability and informativeness, our method adopts a strategy of sparse reward assignment but dense evaluation criteria. Training is performed in a scalable LLM-simulated tool environment, avoiding heavy engineering for large tool sets. Experiments show that CM2 consistently improves over supervised fine-tuning. Starting from an 8B Base model and training on an 8k-example RL dataset, CM2 improves over the SFT counterpart by 8 points on tau^-Bench, by 10 points on BFCL-V4, and by 12 points on ToolSandbox. The results match or even outperform similarly sized open-source baselines, including the judging model. CM2 thus provides a scalable recipe for optimizing multi-turn, multi-step tool-using agents without relying on verifiable rewards. Code provided by the open-source community: https://github.com/namezhenzhang/CM2-RLCR-Tool-Agent.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.12268v2)
