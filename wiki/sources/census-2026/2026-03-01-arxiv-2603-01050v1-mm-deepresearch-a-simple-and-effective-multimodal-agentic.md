---
type: source
source_type: arxiv
title: "MM-DeepResearch: A Simple and Effective Multimodal Agentic Search Baseline"
authors: Huanjin Yao, Qixiang Yin, Min Yang, Ziwang Zhao et al.
url: https://arxiv.org/abs/2603.01050v1
date: 2026-03-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CV
tags: [science-agents, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# MM-DeepResearch: A Simple and Effective Multimodal Agentic Search Baseline

**arXiv:** [2603.01050v1](https://arxiv.org/abs/2603.01050v1) · 2026-03-01 · cs.CV
**Authors:** Huanjin Yao, Qixiang Yin, Min Yang, Ziwang Zhao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We aim to develop a multimodal research agent capable of explicit reasoning and planning, multi-tool invocation, and cross-modal information synthesis, enabling it to conduct deep research tasks. However, we observe three main challenges in developing such agents: (1) scarcity of search-intensive multimodal QA data, (2) lack of effective search trajectories, and (3) prohibitive cost of training with online search APIs. To tackle them, we first propose Hyper-Search, a hypergraph-based QA generation method that models and connects visual and textual nodes within and across modalities, enabling to generate search-intensive multimodal QA pairs that require invoking various search tools to solve. Second, we introduce DR-TTS, which first decomposes search-involved tasks into several categories according to search tool types, and respectively optimize specialized search tool experts for each tool. It then recomposes tool experts to jointly explore search trajectories via tree search, producing trajectories that successfully solve complex tasks using various search tools. Third, we build an offline search engine supporting multiple search tools, enabling agentic reinforcement learning without using costly online search APIs. With the three designs, we develop MM-DeepResearch, a powerful multimodal deep research agent, and extensive results shows its superiority across benchmarks. Code is available at https://github.com/HJYao00/MM-DeepResearch

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01050v1)
