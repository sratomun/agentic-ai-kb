---
type: entity
entity_type: model
tags: [agents, model, small-language-models]
created: 2026-06-23
updated: 2026-06-23
census_count: 25
---

# Phi

*Microsoft's family of small language models built on "textbook-quality" data curation — the canonical proof that data quality can substitute for parameter count.*

## What it is
A line of compact models from Microsoft Research (Phi-2 at 2.7B, the Phi-3 generation including Phi-3-small at 7B, marketed as "a highly capable language model locally on your phone"). The thesis is data-centric: heavily curated, synthetic-and-filtered training data lets a small model punch far above its size class.

## Why it matters
Phi is the most-cited existence proof in the [[small-language-models]] case: Phi-2 (2.7B) matches ~30B models on commonsense and code at ~15× faster inference, and Phi-3-small (7B) reaches 70B-class code generation. When someone argues a small model can't do the job, Phi is the counterexample — and it's why "curate better data" beats "add parameters" as the default SLM play.

## Relationships
- exemplar of [[small-language-models]]; sibling families [[gemma]], [[smollm]], [[nemotron]], [[qwen]]
- capability comes via [[post-training]] and data curation ([[synthetic-data]])
- deployed as the model tier in [[agentic-ai]]

## Cited by
<!-- Auto-maintained by kg-curator enrich. -->
- **277** · 21.9/mo · [[2025-06-02-arxiv-2506-02153v2-small-language-models-are-the-future-of-agentic|Small Language Models are the Future of Agentic AI]]
- **6** · 0.7/mo · [[2025-10-04-arxiv-2510-03847v1-small-language-models-for-agentic-systems-a-survey-of-architectures-ca|Small Language Models for Agentic Systems: A Survey of Architectur…]]
- **5** · 0.3/mo · [[2025-01-04-arxiv-2501-02342v1-optimizing-small-language-models-for-in-vehicle-function-calling|Optimizing Small Language Models for In-Vehicle Function-Calling]]
- **0** · [[2026-06-05-arxiv-2606-07810v1-slmjury-can-small-language-models-judge-as-well-as-large-ones|SLMJury: Can Small Language Models Judge as Well as Large Ones?]]
