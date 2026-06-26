---
type: source
source_type: arxiv
title: "Multi-Agentic Approach for History Matching of Oil Reservoirs"
authors: Linar Samigullin, Sergei Shumilin, Evgeny Burnaev
url: https://arxiv.org/abs/2605.15028v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 26
primary: cs.MA
tags: [clinical-agents, human-agent-interaction, agent-reliability, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# Multi-Agentic Approach for History Matching of Oil Reservoirs

**arXiv:** [2605.15028v1](https://arxiv.org/abs/2605.15028v1) · 2026-05-14 · cs.MA
**Authors:** Linar Samigullin, Sergei Shumilin, Evgeny Burnaev

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
History matching is a central inverse problem in reservoir engineering, where uncertain reservoir parameters must be calibrated against observations. Although automated history matching can reduce manual effort, practical deployment remains difficult because engineers must still configure heterogeneous workflows involving parameter selection, physically admissible bounds, optimizer choice, hyperparameter tuning, simulator execution, and diagnostic reporting. We propose PetroGraph, a multi-agent framework for intelligent reservoir history matching that decomposes this workflow into specialized agents for model review, experimental planning, parameterization, optimization, simulation, and summarization. The system combines large language model agents with domain-specific tools, retrieval-augmented access to simulator documentation, validation of modified ECLIPSE input decks, human-in-the-loop checkpoints, and an OPM Flow-based simulation backend. This design enables users to initiate and steer history matching through natural language while preserving explicit control over selected parameters and optimization settings. We evaluate PetroGraph on three reservoir models of increasing complexity: the synthetic SPE1 model, the faulted SPE9 benchmark, and the real-field Norne model. Using weighted normalized root mean square error as the objective, PetroGraph reduces the mismatch by 95% on SPE1, 69% on SPE9, and 13% on Norne. These results demonstrate that multi-agent orchestration can automate key decisions in history matching, lower the expertise barrier for operating complex simulation workflows, and provide a flexible foundation for extensible, domain-aware reservoir model adaptation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15028v1)
