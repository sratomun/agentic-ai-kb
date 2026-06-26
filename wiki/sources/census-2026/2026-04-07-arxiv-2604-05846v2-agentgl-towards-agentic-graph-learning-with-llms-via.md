---
type: source
source_type: arxiv
title: "AgentGL: Towards Agentic Graph Learning with LLMs via Reinforcement Learning"
authors: Yuanfu Sun, Kang Li, Dongzhe Fan, Jiajin Liu et al.
url: https://arxiv.org/abs/2604.05846v2
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [embodied-agents, knowledge-graph, agentic-rl, agent-memory, tool-use, arxiv, auto-ingested]
---

# AgentGL: Towards Agentic Graph Learning with LLMs via Reinforcement Learning

**arXiv:** [2604.05846v2](https://arxiv.org/abs/2604.05846v2) · 2026-04-07 · cs.CL
**Authors:** Yuanfu Sun, Kang Li, Dongzhe Fan, Jiajin Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) increasingly rely on agentic capabilities-iterative retrieval, tool use, and decision-making-to overcome the limits of static, parametric knowledge. Yet existing agentic frameworks treat external information as unstructured text and fail to leverage the topological dependencies inherent in real-world data. To bridge this gap, we introduce Agentic Graph Learning (AGL), a paradigm that reframes graph learning as an interleaved process of topology-aware navigation and LLM-based inference. Specifically, we propose AgentGL, the first reinforcement learning (RL)-driven framework for AGL. AgentGL equips an LLM agent with graph-native tools for multi-scale exploration, regulates tool usage via search-constrained thinking to balance accuracy and efficiency, and employs a graph-conditioned curriculum RL strategy to stabilize long-horizon policy learning without step-wise supervision. Across diverse Text-Attributed Graph (TAG) benchmarks and multiple LLM backbones, AgentGL substantially outperforms strong GraphLLMs and GraphRAG baselines, achieving absolute improvements of up to 17.5% in node classification and 28.4% in link prediction. These results demonstrate that AGL is a promising frontier for enabling LLMs to autonomously navigate and reason over complex relational environments. The code is publicly available at https://github.com/sunyuanfu/AgentGL.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05846v2)
