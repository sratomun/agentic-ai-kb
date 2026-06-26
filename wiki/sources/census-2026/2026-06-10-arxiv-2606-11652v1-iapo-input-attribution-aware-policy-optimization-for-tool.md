---
type: source
source_type: arxiv
title: "IAPO: Input Attribution-Aware Policy Optimization for Tool Use in Small Multimodal Agents"
authors: Yifan Yang, Zhen Zhang, Jiayi Tian, Liyan Tan et al.
url: https://arxiv.org/abs/2606.11652v1
date: 2026-06-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.LG
tags: [agentic-rl, tool-use, arxiv, auto-ingested]
---

# IAPO: Input Attribution-Aware Policy Optimization for Tool Use in Small Multimodal Agents

**arXiv:** [2606.11652v1](https://arxiv.org/abs/2606.11652v1) · 2026-06-10 · cs.LG
**Authors:** Yifan Yang, Zhen Zhang, Jiayi Tian, Liyan Tan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper investigates reinforcement learning (RL) methods for improving tool-calling capabilities in multimodal small language model (SLM) agents. While existing works have explored various reward designs to improve agentic tool-calling ability, these approaches face inherent limitations for SLM training, especially under multimodal scenarios. First, many existing methods evaluate tool use correctness through exact matching against certain ground-truth or predefined formats. However, this assumption is often unsuitable for multimodal tasks, where multiple tool use paths may be valid and annotated tool trajectories are typically unavailable. Second, such sparse and brittle binary rewards provide little guidance on how to improve the underlying decision process, making them particularly difficult for multimodal SLM to learn from. To address these issues, we propose Input Attribution-Aware Policy Optimization (IAPO), an RL algorithm for improving tool use in multimodal SLM by aligning the model's attribution across input components with that of a stronger teacher. Experiments on Qwen2.5-VL-3B show that the proposed method improves visual question answering accuracy by an average of 3% across six test sets compared with existing visual tool use work, by helping the model attend to the most relevant input evidence.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.11652v1)
