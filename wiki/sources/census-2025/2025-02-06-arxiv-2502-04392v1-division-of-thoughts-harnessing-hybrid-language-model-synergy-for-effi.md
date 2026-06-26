---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Division-of-Thoughts: Harnessing Hybrid Language Model Synergy for Efficient On-Device Agents"
authors: Chenyang Shao et al.
url: https://arxiv.org/abs/2502.04392v1
date: 2025-02-06
score: 9
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, reasoning-models]
---

# Division-of-Thoughts: Harnessing Hybrid Language Model Synergy for Efficient On-Device Agents

**arXiv:** [2502.04392v1](https://arxiv.org/abs/2502.04392v1) · 2025-02-06 · cs.CL
**Authors:** Chenyang Shao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The rapid expansion of web content has made on-device AI assistants indispensable for helping users manage the increasing complexity of online tasks. The emergent reasoning ability in large language models offer a promising path for next-generation on-device AI agents. However, deploying full-scale Large Language Models (LLMs) on resource-limited local devices is challenging. In this paper, we propose Division-of-Thoughts (DoT), a collaborative reasoning framework leveraging the synergy between locally deployed Smaller-scale Language Models (SLMs) and cloud-based LLMs. DoT leverages a Task Decomposer to elicit the inherent planning abilities in language models to decompose user queries into smaller sub-tasks, which allows hybrid language models to fully exploit their respective strengths. Besides, DoT employs a Task Scheduler to analyze the pair-wise dependency of sub-tasks and create a dependency graph, facilitating parallel reasoning of sub-tasks and the identification of key steps. To allocate the appropriate model based on the difficulty of sub-tasks, DoT leverages a Plug-and-Play Adapter, which is an additional task head attached to the SLM that does not alter the SLM's parameters. To boost adapter's task allocation capability, we propose a self-reinforced training method that relies solely on task execution feedback. Extensive experiments on various benchmarks demonstrate that our DoT significantly reduces LLM costs while maintaining competitive reasoning accuracy. Specifically, DoT reduces the average reasoning time and API costs by 66.12% and 83.57%, while achieving comparable reasoning accuracy with the best baseline methods.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2502.04392v1)
