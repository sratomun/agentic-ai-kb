---
type: source
source_type: arxiv
title: "Toward Culturally Aligned LLMs through Ontology-Guided Multi-Agent Reasoning"
authors: Wonduk Seo, Wonseok Choi, Junseo Koh, Juhyeon Lee et al.
url: https://arxiv.org/abs/2601.21700v3
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.CL
tags: [knowledge-graph, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Toward Culturally Aligned LLMs through Ontology-Guided Multi-Agent Reasoning

**arXiv:** [2601.21700v3](https://arxiv.org/abs/2601.21700v3) · 2026-01-29 · cs.CL
**Authors:** Wonduk Seo, Wonseok Choi, Junseo Koh, Juhyeon Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) increasingly support culturally sensitive decision making, yet often exhibit misalignment due to skewed pretraining data and the absence of structured value representations. Existing methods can steer outputs, but often lack demographic grounding and treat values as independent, unstructured signals, reducing consistency and interpretability. We propose OG-MAR, an Ontology-Guided Multi-Agent Reasoning framework. OG-MAR summarizes respondent-specific values from the World Values Survey (WVS) and constructs a global cultural ontology by eliciting relations over a fixed taxonomy via competency questions. At inference time, it retrieves ontology-consistent relations and demographically similar profiles to instantiate multiple value-persona agents, whose outputs are synthesized by a judgment agent that enforces ontology consistency and demographic proximity. Experiments on regional social-survey benchmarks across four LLM backbones show that OG-MAR improves cultural alignment and robustness over competitive baselines, while producing more transparent reasoning traces.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21700v3)
