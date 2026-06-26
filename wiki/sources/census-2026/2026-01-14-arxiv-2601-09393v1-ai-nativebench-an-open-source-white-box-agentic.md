---
type: source
source_type: arxiv
title: "AI-NativeBench: An Open-Source White-Box Agentic Benchmark Suite for AI-Native Systems"
authors: Zirui Wang, Guangba Yu, Michael R. Lyu
url: https://arxiv.org/abs/2601.09393v1
date: 2026-01-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [coding-agents, agent-reliability, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# AI-NativeBench: An Open-Source White-Box Agentic Benchmark Suite for AI-Native Systems

**arXiv:** [2601.09393v1](https://arxiv.org/abs/2601.09393v1) · 2026-01-14 · cs.SE
**Authors:** Zirui Wang, Guangba Yu, Michael R. Lyu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The transition from Cloud-Native to AI-Native architectures is fundamentally reshaping software engineering, replacing deterministic microservices with probabilistic agentic services. However, this shift renders traditional black-box evaluation paradigms insufficient: existing benchmarks measure raw model capabilities while remaining blind to system-level execution dynamics. To bridge this gap, we introduce AI-NativeBench, the first application-centric and white-box AI-Native benchmark suite grounded in Model Context Protocol (MCP) and Agent-to-Agent (A2A) standards. By treating agentic spans as first-class citizens within distributed traces, our methodology enables granular analysis of engineering characteristics beyond simple capabilities. Leveraging this benchmark across 21 system variants, we uncover critical engineering realities invisible to traditional metrics: a parameter paradox where lightweight models often surpass flagships in protocol adherence, a pervasive inference dominance that renders protocol overhead secondary, and an expensive failure pattern where self-healing mechanisms paradoxically act as cost multipliers on unviable workflows. This work provides the first systematic evidence to guide the transition from measuring model capability to engineering reliable AI-Native systems. To facilitate reproducibility and further research, we have open-sourced the benchmark and dataset.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[a2a-protocol]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.09393v1)
