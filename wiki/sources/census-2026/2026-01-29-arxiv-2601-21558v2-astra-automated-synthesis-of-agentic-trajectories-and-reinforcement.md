---
type: source
source_type: arxiv
title: "ASTRA: Automated Synthesis of agentic Trajectories and Reinforcement Arenas"
authors: Xiaoyu Tian, Haotian Wang, Shuaiting Chen, Hao Zhou et al.
url: https://arxiv.org/abs/2601.21558v2
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [agentic-rl, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# ASTRA: Automated Synthesis of agentic Trajectories and Reinforcement Arenas

**arXiv:** [2601.21558v2](https://arxiv.org/abs/2601.21558v2) · 2026-01-29 · cs.CL
**Authors:** Xiaoyu Tian, Haotian Wang, Shuaiting Chen, Hao Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) are increasingly used as tool-augmented agents for multi-step decision making, yet training robust tool-using agents remains challenging. Existing methods still require manual intervention, depend on non-verifiable simulated environments, rely exclusively on either supervised fine-tuning (SFT) or reinforcement learning (RL), and struggle with stable long-horizon, multi-turn learning. To address these challenges, we introduce ASTRA, a fully automated end-to-end framework for training tool-augmented language model agents via scalable data synthesis and verifiable reinforcement learning. ASTRA integrates two complementary components. First, a pipeline that leverages the static topology of tool-call graphs synthesizes diverse, structurally grounded trajectories, instilling broad and transferable tool-use competence. Second, an environment synthesis framework that captures the rich, compositional topology of human semantic reasoning converts decomposed question-answer traces into independent, code-executable, and rule-verifiable environments, enabling deterministic multi-turn RL. Based on this method, we develop a unified training methodology that integrates SFT with online RL using trajectory-level rewards to balance task completion and interaction efficiency. Experiments on multiple agentic tool-use benchmarks demonstrate that ASTRA-trained models achieve state-of-the-art performance at comparable scales, approaching closed-source systems while preserving core reasoning ability. We release the full pipelines, environments, and trained models at https://github.com/LianjiaTech/astra.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21558v2)
