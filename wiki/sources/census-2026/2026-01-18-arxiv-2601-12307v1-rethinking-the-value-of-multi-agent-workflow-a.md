---
type: source
source_type: arxiv
title: "Rethinking the Value of Multi-Agent Workflow: A Strong Single Agent Baseline"
authors: Jiawei Xu, Arief Koesdwiady, Sisong Bei, Yan Han et al.
url: https://arxiv.org/abs/2601.12307v1
date: 2026-01-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.MA
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Rethinking the Value of Multi-Agent Workflow: A Strong Single Agent Baseline

**arXiv:** [2601.12307v1](https://arxiv.org/abs/2601.12307v1) · 2026-01-18 · cs.MA
**Authors:** Jiawei Xu, Arief Koesdwiady, Sisong Bei, Yan Han et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in LLM-based multi-agent systems (MAS) show that workflows composed of multiple LLM agents with distinct roles, tools, and communication patterns can outperform single-LLM baselines on complex tasks. However, most frameworks are homogeneous, where all agents share the same base LLM and differ only in prompts, tools, and positions in the workflow. This raises the question of whether such workflows can be simulated by a single agent through multi-turn conversations. We investigate this across seven benchmarks spanning coding, mathematics, general question answering, domain-specific reasoning, and real-world planning and tool use. Our results show that a single agent can reach the performance of homogeneous workflows with an efficiency advantage from KV cache reuse, and can even match the performance of an automatically optimized heterogeneous workflow. Building on this finding, we propose \textbf{OneFlow}, an algorithm that automatically tailors workflows for single-agent execution, reducing inference costs compared to existing automatic multi-agent design frameworks without trading off accuracy. These results position the single-LLM implementation of multi-agent workflows as a strong baseline for MAS research. We also note that single-LLM methods cannot capture heterogeneous workflows due to the lack of KV cache sharing across different LLMs, highlighting future opportunities in developing \textit{truly} heterogeneous multi-agent systems.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.12307v1)
