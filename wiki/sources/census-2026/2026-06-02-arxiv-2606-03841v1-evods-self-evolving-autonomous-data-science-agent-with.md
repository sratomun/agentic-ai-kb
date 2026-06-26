---
type: source
source_type: arxiv
title: "EvoDS: Self-Evolving Autonomous Data Science Agent with Skill Learning and Context Management"
authors: Zherui Yang, Fan Liu, Yansong Ning, Hao Liu
url: https://arxiv.org/abs/2606.03841v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agent-reliability, self-evolving-agents, agentic-rl, agent-skills, agent-memory, arxiv, auto-ingested]
---

# EvoDS: Self-Evolving Autonomous Data Science Agent with Skill Learning and Context Management

**arXiv:** [2606.03841v1](https://arxiv.org/abs/2606.03841v1) · 2026-06-02 · cs.AI
**Authors:** Zherui Yang, Fan Liu, Yansong Ning, Hao Liu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent progress in Large Language Model (LLM) agents has enabled promising advances in automated data science. However, existing approaches remain fundamentally limited by their static action sets and lack of principled long-horizon context management, hindering their ability to accumulate reusable experience across tasks and operate reliably in multi-stage, iterative data science pipelines. To address these challenges, we introduce EvoDS, a self-evolving autonomous data science agent that learns to expand its skills and adaptively managing long-term context through agentic reinforcement learning. Specifically, EvoDS introduces two key strategies: (1) Autonomous Skill Acquisition (ASA) mechanism, which enables agents to synthesize, validate, and reuse executable skills; and (2) Adaptive Context Compression (ACC) strategy, which treats context management as a learned control problem rather than passive truncation. These strategies are orchestrated within a two-stage multi-agent training scheme, enabling EvoDS to autonomously improve over time. Theoretically, we prove that EvoDS's hierarchical design reduces tool-selection error, and its optimization objective aligns with an information bottleneck principle, ensuring efficient context use. Empirically, EvoDS outperforms state-of-the-art open-source data science agents by an average of 28.9% across four diverse benchmarks while eliminating out-of-token failures. Our code and data are available at https://github.com/usail-hkust/EvoDS.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03841v1)
