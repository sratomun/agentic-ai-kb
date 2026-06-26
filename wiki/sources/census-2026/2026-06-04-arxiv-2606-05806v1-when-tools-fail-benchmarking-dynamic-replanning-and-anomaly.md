---
type: source
source_type: arxiv
title: "When Tools Fail: Benchmarking Dynamic Replanning and Anomaly Recovery in LLM Agents"
authors: Dongsheng Zhu, Xuchen Ma, Yucheng Shen, Xiang Li et al.
url: https://arxiv.org/abs/2606.05806v1
date: 2026-06-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# When Tools Fail: Benchmarking Dynamic Replanning and Anomaly Recovery in LLM Agents

**arXiv:** [2606.05806v1](https://arxiv.org/abs/2606.05806v1) · 2026-06-04 · cs.AI
**Authors:** Dongsheng Zhu, Xuchen Ma, Yucheng Shen, Xiang Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing benchmarks evaluate Tool-Integrated Reasoning (TIR) in LLMs on idealized ''happy paths'', largely overlooking real-world tool failures. We introduce ToolMaze, a benchmark for dynamic path discovery and error recovery in TIR agents. To separate systematic replanning from blind trial-and-error, ToolMaze adopts a two-dimensional design: DAG-based topological complexity and a $2 \times 2$ taxonomy of tool perturbations (explicit/implicit, transient/permanent). Evaluations show that perturbations degrade performance across nearly all models, with the sharpest drops under implicit semantic failures. Driven by systemic over-trust in corrupted outputs, Perturbation Recovery Rate (PRR) plummets by around 37\% in these scenarios, while complex topologies trap agents in futile trial-and-error loops. Crucially, agentic fault-tolerance improves with model scale $3.66\times$ slower than basic task execution, highlighting dynamic replanning as a distinct bottleneck unaddressed by model scaling or prompting. Data and code are available at https://github.com/Zhudongsheng75/ToolMaze.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.05806v1)
