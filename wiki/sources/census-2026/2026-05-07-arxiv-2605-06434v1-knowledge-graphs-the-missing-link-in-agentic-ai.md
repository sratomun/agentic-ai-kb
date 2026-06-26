---
type: source
source_type: arxiv
title: "Knowledge Graphs, the Missing Link in Agentic AI-based Formal Verification"
authors: Vaisakh Naduvodi Viswambharan, Keerthan Kopparam Radhakrishna, Deepak Narayan Gadde, Aman Kumar
url: https://arxiv.org/abs/2605.06434v1
date: 2026-05-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, knowledge-graph, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Knowledge Graphs, the Missing Link in Agentic AI-based Formal Verification

**arXiv:** [2605.06434v1](https://arxiv.org/abs/2605.06434v1) · 2026-05-07 · cs.AI
**Authors:** Vaisakh Naduvodi Viswambharan, Keerthan Kopparam Radhakrishna, Deepak Narayan Gadde, Aman Kumar

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Large Language Models (LLMs) have enabled workflows that generate SystemVerilog Assertions (SVAs) from natural-language specifications, with the potential to accelerate Formal Verification (FV). However, high-quality assertion synthesis remains challenging because specifications are often ambiguous or incomplete and critical micro-architectural details reside in the Register Transfer Level (RTL). Many existing approaches treat the specification and RTL as loosely structured text, which weakens specification-to-RTL grounding and leads to semantic mismatches and frequent syntax failures during formal parsing and elaboration. This work addresses these limitations with a verification-centric Knowledge Graph (KG) constructed from structured Intermediate Representations (IRs) extracted from the specification, RTL, and formal-tool feedback, including syntax diagnostics, Counterexamples (CEXs), and coverage reports. The KG links requirements, design hierarchy, signals, assumptions, and properties to provide traceable, design-grounded context for generation. A multi-agent workflow queries and updates this KG to generate SVAs and to drive three refinement loops: syntax repair guided by tool diagnostics, CEX-guided correction using trace links, and coverage-directed property augmentation. Evaluation across seven benchmark designs indicates that KG-based context retrieval improves specification-to-RTL grounding and consistently produces compilable SVAs with low syntax-repair overhead. The approach achieves formal coverage ranging from 78.5% to 99.4%, though convergence exhibits design dependence with complex temporal and arithmetic reasoning remaining challenging for current LLM capabilities.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.06434v1)
