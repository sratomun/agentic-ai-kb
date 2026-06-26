---
type: entity
entity_type: model
tags: [agents, model, small-language-models]
created: 2026-06-23
updated: 2026-06-23
census_count: 26
---

# Nemotron

*NVIDIA's family of efficient open models — including the Nemotron-H hybrid Mamba-Transformer line and the Hymba hybrid-head SLMs — built to hit LLM-class accuracy at a fraction of the inference FLOPs.*

## What it is
NVIDIA Research's efficient-model program. Nemotron-H is a family of hybrid Mamba-Transformer models (2/4.8/9B) that trade some attention for state-space layers to cut inference cost; Hymba-1.5B is a related hybrid-head architecture. The bet is architectural: different model sizes want different architectures, not just fewer layers of the same one.

## Why it matters
Nemotron is the architectural half of the [[small-language-models]] argument — evidence that you beat the scaling law by changing the architecture, not only the size. Nemotron-H (2/4.8/9B) matches dense 30B models on instruction-following and code at an order-of-magnitude fewer inference FLOPs; Hymba-1.5B shows ~3.5× the throughput of comparable transformers and outperforms 13B models on instruction following. It also signals NVIDIA's own stake: the company is building the models *and* the edge/inference stack an SLM-first world runs on.

## Relationships
- exemplar of [[small-language-models]]; sibling families [[phi]], [[smollm]], [[gemma]], [[qwen]]
- hybrid architecture relates to [[mixture-of-experts]] (both are efficiency-by-design routes)
- deployed as the model tier in [[agentic-ai]]

## Cited by
<!-- Auto-maintained by kg-curator enrich. -->
- **277** · 21.9/mo · [[2025-06-02-arxiv-2506-02153v2-small-language-models-are-the-future-of-agentic|Small Language Models are the Future of Agentic AI]]
