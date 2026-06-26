---
type: source
source_type: arxiv
title: "W&D:Scaling Parallel Tool Calling for Efficient Deep Research Agents"
authors: Xiaoqiang Lin, Jun Hao Liew, Silvio Savarese, Junnan Li
url: https://arxiv.org/abs/2602.07359v1
date: 2026-02-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [science-agents, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# W&D:Scaling Parallel Tool Calling for Efficient Deep Research Agents

**arXiv:** [2602.07359v1](https://arxiv.org/abs/2602.07359v1) · 2026-02-07 · cs.AI
**Authors:** Xiaoqiang Lin, Jun Hao Liew, Silvio Savarese, Junnan Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Deep research agents have emerged as powerful tools for automating complex intellectual tasks through multi-step reasoning and web-based information seeking. While recent efforts have successfully enhanced these agents by scaling depth through increasing the number of sequential thinking and tool calls, the potential of scaling width via parallel tool calling remains largely unexplored. In this work, we propose the Wide and Deep research agent, a framework designed to investigate the behavior and performance of agents when scaling not only depth but also width via parallel tool calling. Unlike existing approaches that rely on complex multi-agent orchestration to parallelize workloads, our method leverages intrinsic parallel tool calling to facilitate effective coordination within a single reasoning step. We demonstrate that scaling width significantly improves performance on deep research benchmarks while reducing the number of turns required to obtain correct answers. Furthermore, we analyze the factors driving these improvements through case studies and explore various tool call schedulers to optimize parallel tool calling strategy. Our findings suggest that optimizing the trade-off between width and depth is a critical pathway toward high-efficiency deep research agents. Notably, without context management or other tricks, we obtain 62.2% accuracy with GPT-5-Medium on BrowseComp, surpassing the original 54.9% reported by GPT-5-High.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.07359v1)
