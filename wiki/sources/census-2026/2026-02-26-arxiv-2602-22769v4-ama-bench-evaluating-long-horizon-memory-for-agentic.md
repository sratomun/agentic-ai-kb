---
type: source
source_type: arxiv
title: "AMA-Bench: Evaluating Long-Horizon Memory for Agentic Applications"
authors: Yujie Zhao, Boqin Yuan, Junbo Huang, Haocheng Yuan et al.
url: https://arxiv.org/abs/2602.22769v4
date: 2026-02-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# AMA-Bench: Evaluating Long-Horizon Memory for Agentic Applications

**arXiv:** [2602.22769v4](https://arxiv.org/abs/2602.22769v4) · 2026-02-26 · cs.AI
**Authors:** Yujie Zhao, Boqin Yuan, Junbo Huang, Haocheng Yuan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) are increasingly used as autonomous agents in complex, long-horizon applications, where effective memory is critical for sustained performance. Yet existing memory benchmarks are largely dialogue-centric, while real agent memory consists of continuous agent-environment interaction trajectories composed of states, actions, observations, and tool outputs. To address this gap, we introduce **AMA-Bench** (**A**gent **M**emory with **A**ny length), a benchmark for evaluating long-horizon memory in realistic agentic settings. AMA-Bench combines real-world agent trajectories from representative applications with expert-curated QA, as well as synthetic trajectories that scale to arbitrary horizons with rule-based QA. Our study shows that existing memory systems underperform because they fail to capture causal and objective information and rely heavily on lossy similarity-based retrieval. We further propose **AMA-Agent**, a memory system based on causality-graph construction and tool-augmented retrieval. AMA-Agent achieves **57.22%** accuracy on AMA-Bench, outperforming the strongest baseline by **11.16%**. Resources are available at: [https://ama-bench.github.io/](https://ama-bench.github.io/).

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.22769v4)
