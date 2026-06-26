---
type: source
source_type: arxiv
title: "Team of Thoughts: Efficient Test-time Scaling of Agentic Systems through Orchestrated Tool Calling"
authors: Jeffrey T. H. Wong, Zixi Zhang, Junyi Liu, Yiren Zhao
url: https://arxiv.org/abs/2602.16485v2
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.CL
tags: [coding-agents, agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Team of Thoughts: Efficient Test-time Scaling of Agentic Systems through Orchestrated Tool Calling

**arXiv:** [2602.16485v2](https://arxiv.org/abs/2602.16485v2) · 2026-02-18 · cs.CL
**Authors:** Jeffrey T. H. Wong, Zixi Zhang, Junyi Liu, Yiren Zhao

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing Multi-Agent Systems (MAS) typically rely on homogeneous model configurations, failing to exploit the diverse expertise inherent in different post-trained architectures. We propose Team-of-Thoughts, a heterogeneous MAS framework that treats diverse models as specialized tools within an orchestrator-driven paradigm. Team-of-Thoughts introduces two novel components: (1) Orchestrator Calibration, which identifies models with superior coordination and synthesis capabilities, and (2) Agent Self-Assessment, a protocol where tool agents profile their own domain-specific strengths to guide selection. At inference, the orchestrator dynamically activates the most compatible agents based on these profiles to maximize capability coverage. Across five mathematical reasoning and code generation benchmarks, Team-of-Thoughts consistently outperforms individual models and existing MAS baselines. Notably, on AIME24 and LiveCodeBench, Team-of-Thoughts achieves 96.00% and 77.91% accuracy, respectively, significantly improving over homogeneous role-play baselines (80.00% and 65.93%).

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[livecodebench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16485v2)
