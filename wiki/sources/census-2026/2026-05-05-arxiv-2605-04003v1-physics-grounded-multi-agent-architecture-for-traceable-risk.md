---
type: source
source_type: arxiv
title: "Physics-Grounded Multi-Agent Architecture for Traceable, Risk-Aware Human-AI Decision Support in Manufacturing"
authors: Danny Hoang, Ryan Matthiessen, Christopher Miller, Nasir Mannan et al.
url: https://arxiv.org/abs/2605.04003v1
date: 2026-05-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.MA
tags: [recommendation-agents, knowledge-graph, human-agent-interaction, agent-reliability, agent-security, arxiv, auto-ingested]
---

# Physics-Grounded Multi-Agent Architecture for Traceable, Risk-Aware Human-AI Decision Support in Manufacturing

**arXiv:** [2605.04003v1](https://arxiv.org/abs/2605.04003v1) · 2026-05-05 · cs.MA
**Authors:** Danny Hoang, Ryan Matthiessen, Christopher Miller, Nasir Mannan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
High-precision CNC machining of free-form aerospace components requires bounded compensations informed by inspection, simulation, and process knowledge. Off-the-shelf large language model (LLM) assistants can generate text, but they do not reliably execute risk-constrained multi-step numerical workflows or provide auditable provenance for high-stakes decisions. We present multi-agent knowledge analysis (MAKA), a human-in-the-loop decision-support architecture that separates intent routing, tools-only quantitative analysis, knowledge graph retrieval, and critic-based verification that enforces physical plausibility, safety bounds, and provenance completeness before recommendations are surfaced for human approval. MAKA is instantiated on a Ti-6Al-4V rotor blade machining testbed by fusing virtual-machining path-tracking error fields, cutting-force and deflection simulations, and scan-based 3D inspection deviation maps from 16 blades. The analysis decomposes deviation into an evidence-linked pathing component, a drift-based wear proxy capturing systematic evolution across parts, a residual systematic compliance term, and a variability proxy for instability-aware escalation. In a three-level tool-orchestration benchmark (single-step through $\geq$3-step stateful sequences), MAKA improves successful tool execution by up to 87.5 percentage points relative to an unstructured single-model interaction pattern with identical tool access. Digital twin what-if studies show MAKA can coordinate traceable compensation candidates that reduce predicted surface deviation from order $10^{-2}$in to approximately $\pm 10^{-3}$in over most of the blade within the simulation environment, providing a pre-deployment verification signal for risk-aware human decision-making.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[knowledge-graph|Knowledge graphs]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.04003v1)
