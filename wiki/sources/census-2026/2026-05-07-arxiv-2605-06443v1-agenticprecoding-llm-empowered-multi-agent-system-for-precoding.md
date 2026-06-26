---
type: source
source_type: arxiv
title: "AgenticPrecoding: LLM-Empowered Multi-Agent System for Precoding Optimization"
authors: Zijiu Yang, Zixiang Zhang, Shunpu Tang, Qianqian Yang et al.
url: https://arxiv.org/abs/2605.06443v1
date: 2026-05-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.MA
tags: [coding-agents, multi-agent-systems, arxiv, auto-ingested]
---

# AgenticPrecoding: LLM-Empowered Multi-Agent System for Precoding Optimization

**arXiv:** [2605.06443v1](https://arxiv.org/abs/2605.06443v1) · 2026-05-07 · cs.MA
**Authors:** Zijiu Yang, Zixiang Zhang, Shunpu Tang, Qianqian Yang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Precoding is a key technique for interference management and performance improvement in multi-antenna wireless systems. However, existing precoding methods are typically developed for specific system models, objectives, and constraint sets, which limits their adaptability to the heterogeneous and evolving scenarios expected in future 6G networks. To address this limitation, we propose AgenticPrecoding, a universal multi-agent framework that automates end-to-end precoding derivation directly from user-level communication requirements. Specifically, AgenticPrecoding decomposes the derivation process into four coordinated stages: problem formulation, solver selection, prompt upsampling, and code generation, assigning each stage to a specialized agent tailored to its specific reasoning demands. We employ two LoRA-adapted reasoning agents to inject precoding-specific domain knowledge for problem formulation and solver selection, while two general-purpose Large Language Models (LLMs) handle prompt refinement and executable code generation. Furthermore, a feedback-driven refinement mechanism is incorporated to enhance code executability, constraint feasibility, and solution quality. Extensive experiments across 10 representative precoding scenarios demonstrate that AgenticPrecoding achieves superior cross-scenario adaptability compared to conventional optimization-based and LLM-based baselines.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.06443v1)
