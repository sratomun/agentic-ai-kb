---
type: source
source_type: arxiv
title: "WideSeek-R1: Exploring Width Scaling for Broad Information Seeking via Multi-Agent Reinforcement Learning"
authors: Zelai Xu, Zhexuan Xu, Ruize Zhang, Chunyang Zhu et al.
url: https://arxiv.org/abs/2602.04634v3
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [agentic-rl, agent-memory, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# WideSeek-R1: Exploring Width Scaling for Broad Information Seeking via Multi-Agent Reinforcement Learning

**arXiv:** [2602.04634v3](https://arxiv.org/abs/2602.04634v3) · 2026-02-04 · cs.AI
**Authors:** Zelai Xu, Zhexuan Xu, Ruize Zhang, Chunyang Zhu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advancements in Large Language Models (LLMs) have largely focused on depth scaling, where a single agent solves long-horizon problems with multi-turn reasoning and tool use. However, as tasks grow broader, the key bottleneck shifts from individual competence to organizational capability. In this work, we explore a complementary dimension of width scaling with multi-agent systems to address broad information seeking. Existing multi-agent systems often rely on hand-crafted workflows and turn-taking interactions that fail to parallelize work effectively. To bridge this gap, we propose WideSeek-R1, a lead-agent-subagent framework trained via multi-agent reinforcement learning (MARL) to synergize scalable orchestration and parallel execution. By utilizing a shared LLM with isolated contexts and specialized tools, WideSeek-R1 jointly optimizes the lead agent and parallel subagents on a curated dataset of 20k broad information-seeking tasks. Extensive experiments show that WideSeek-R1-4B achieves an item F1 score of 40.0% on the WideSearch benchmark, which is comparable to the performance of single-agent DeepSeek-R1-671B. Furthermore, WideSeek-R1-4B exhibits consistent performance gains as the number of parallel subagents increases, highlighting the effectiveness of width scaling.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.04634v3)
