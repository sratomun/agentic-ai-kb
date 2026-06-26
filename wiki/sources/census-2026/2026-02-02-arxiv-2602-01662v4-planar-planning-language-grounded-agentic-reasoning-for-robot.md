---
type: source
source_type: arxiv
title: "PLanAR: Planning-Language-Grounded Agentic Reasoning for Robot Manipulation"
authors: Pengyuan Guo, Zhonghao Mai, Zhengtong Xu, Kaidi Zhang et al.
url: https://arxiv.org/abs/2602.01662v4
date: 2026-02-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.RO
tags: [embodied-agents, agent-skills, agent-memory, arxiv, auto-ingested]
---

# PLanAR: Planning-Language-Grounded Agentic Reasoning for Robot Manipulation

**arXiv:** [2602.01662v4](https://arxiv.org/abs/2602.01662v4) · 2026-02-02 · cs.RO
**Authors:** Pengyuan Guo, Zhonghao Mai, Zhengtong Xu, Kaidi Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in vision-language models (VLMs) have enabled increasing progress in real-world robot manipulation. However, long-horizon manipulation in unstructured environments requires VLMs to reason about changing scene states, action constraints, and execution outcomes, which remains difficult with natural language reasoning alone. We present PLanAR, a planning-language-grounded robot agent framework for open-vocabulary, long-horizon manipulation. PLanAR uses a planning-language interface to define the VLM reasoning space: object predicates represent scene states, action schemas specify robot skills with preconditions and effects, and symbolic plans provide executable intermediate representations. This interface enables stepwise verification: after each action, PLanAR uses onboard observations to check whether the expected symbolic effects have been achieved, allowing the VLM-based agent to update task states, detect failures, and replan when execution deviates from expectation. Across robot embodiments, VLM backends, and tasks including stacking, crossword solving, and long-horizon kitchen workflows, PLanAR demonstrates strong real-world capability while revealing key limitations of current VLMs in embodied reasoning.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.01662v4)
