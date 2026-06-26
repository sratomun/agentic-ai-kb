---
type: source
source_type: arxiv
title: "AgentHallu: Benchmarking Automated Hallucination Attribution of LLM-based Agents"
authors: Xuannan Liu, Xiao Yang, Zekun Li, Peipei Li et al.
url: https://arxiv.org/abs/2601.06818v1
date: 2026-01-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [clinical-agents, agent-reliability, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# AgentHallu: Benchmarking Automated Hallucination Attribution of LLM-based Agents

**arXiv:** [2601.06818v1](https://arxiv.org/abs/2601.06818v1) · 2026-01-11 · cs.CL
**Authors:** Xuannan Liu, Xiao Yang, Zekun Li, Peipei Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As LLM-based agents operate over sequential multi-step reasoning, hallucinations arising at intermediate steps risk propagating along the trajectory, thus degrading overall reliability. Unlike hallucination detection in single-turn responses, diagnosing hallucinations in multi-step workflows requires identifying which step causes the initial divergence. To fill this gap, we propose a new research task, automated hallucination attribution of LLM-based agents, aiming to identify the step responsible for the hallucination and explain why. To support this task, we introduce AgentHallu, a comprehensive benchmark with: (1) 693 high-quality trajectories spanning 7 agent frameworks and 5 domains, (2) a hallucination taxonomy organized into 5 categories (Planning, Retrieval, Reasoning, Human-Interaction, and Tool-Use) and 14 sub-categories, and (3) multi-level annotations curated by humans, covering binary labels, hallucination-responsible steps, and causal explanations. We evaluate 13 leading models, and results show the task is challenging even for top-tier models (like GPT-5, Gemini-2.5-Pro). The best-performing model achieves only 41.1\% step localization accuracy, where tool-use hallucinations are the most challenging at just 11.6\%. We believe AgentHallu will catalyze future research into developing robust, transparent, and reliable agentic systems.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.06818v1)
