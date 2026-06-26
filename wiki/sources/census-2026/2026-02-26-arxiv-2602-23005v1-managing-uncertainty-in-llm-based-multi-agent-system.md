---
type: source
source_type: arxiv
title: "Managing Uncertainty in LLM-based Multi-Agent System Operation"
authors: Man Zhang, Tao Yue, Yihua He
url: https://arxiv.org/abs/2602.23005v1
date: 2026-02-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.SE
tags: [clinical-agents, coding-agents, knowledge-graph, human-agent-interaction, agent-reliability, arxiv, auto-ingested]
---

# Managing Uncertainty in LLM-based Multi-Agent System Operation

**arXiv:** [2602.23005v1](https://arxiv.org/abs/2602.23005v1) · 2026-02-26 · cs.SE
**Authors:** Man Zhang, Tao Yue, Yihua He

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Applying LLM-based multi-agent software systems in safety-critical domains such as lifespan echocardiography introduces system-level risks that cannot be addressed by improving model accuracy alone. During system operation, beyond individual LLM behavior, uncertainty propagates through agent coordination, data pipelines, human-in-the-loop interaction, and runtime control logic. Yet existing work largely treats uncertainty at the model level rather than as a first-class software engineering concern. This paper approaches uncertainty from both system-level and runtime perspectives. We first differentiate epistemological and ontological uncertainties in the context of LLM-based multi-agent software system operation. Building on this foundation, we propose a lifecycle-based uncertainty management framework comprising four mechanisms: representation, identification, evolution, and adaptation. The uncertainty lifecycle governs how uncertainties emerge, transform, and are mitigated across architectural layers and execution phases, enabling structured runtime governance and controlled adaptation. We demonstrate the feasibility of the framework using a real-world LLM-based multi-agent echocardiographic software system developed in clinical collaboration, showing improved reliability and diagnosability in diagnostic reasoning. The proposed approach generalizes to other safety-critical LLM-based multi-agent software systems, supporting principled operational control and runtime assurance beyond model-centric methods.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23005v1)
