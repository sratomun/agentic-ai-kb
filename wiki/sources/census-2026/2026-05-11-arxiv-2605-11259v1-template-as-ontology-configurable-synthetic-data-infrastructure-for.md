---
type: source
source_type: arxiv
title: "Template-as-Ontology: Configurable Synthetic Data Infrastructure for Cross-Domain Manufacturing AI Validation"
authors: Grama Chethan
url: https://arxiv.org/abs/2605.11259v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.AI
tags: [knowledge-graph, tool-use, arxiv, auto-ingested]
---

# Template-as-Ontology: Configurable Synthetic Data Infrastructure for Cross-Domain Manufacturing AI Validation

**arXiv:** [2605.11259v1](https://arxiv.org/abs/2605.11259v1) · 2026-05-11 · cs.AI
**Authors:** Grama Chethan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLarge language model (LLM)-based AI agents deployed in manufacturing environments require populated, schema-correct data for validation, yet production MES data is proprietary, privacy-encumbered, and vendor-specific. This paper introduces the Template-as-Ontology principle: a single Python configuration module (700-770 lines, 45 validated exports) serves simultaneously as the specification for a time-stepped manufacturing simulator and as the runtime domain schema for AI analytics tools, producing alignment by construction rather than integration. We formally define the domain template as a typed relational configuration schema and prove that structural alignment between simulation and tool layers is guaranteed by single-source consumption. A five-layer pipeline--simulation, PostgreSQL, CDC/Iceberg lakehouse, star schema, and 12 parameterized AI tools--generates causally coherent, MES-shaped data spanning 66 entity types across four operational domains mapped to ISA-95/IEC 62264. We validate the architecture with six industry templates (aerospace, pharma, automotive, electronics, beverages, warehousing) running on identical framework code. Calibration experiments (60 runs, 10 seeds per template) confirm parametric controllability: observed KPIs fall within configured ranges across all templates. A controlled hallucination experiment (72 tool invocations, Qwen3-32B) demonstrates that ontology-constrained parameters eliminate tool-parameter fabrication (0% constrained vs. 43% unconstrained hallucination rate for the evaluated model, Fisher's exact test p < 10^-12); the 0% constrained rate is an architectural guarantee that holds for any model. The framework provides a reusable data layer for discrete manufacturing AI validation.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.11259v1)
