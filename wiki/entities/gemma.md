---
type: entity
entity_type: model
tags: [agents, model, small-language-models, open-models]
created: 2026-06-23
updated: 2026-06-23
census_count: 98
---

# Gemma

*Google's open-weight small-model family, derived from the Gemini research line — one of the two most-used SLM bases across the agent literature (with Qwen).*

## What it is
Google DeepMind's family of open-weight models (Gemma and successors), built from the same research as the proprietary Gemini models but released for local and on-device use across a range of small sizes.

## Why it matters
Gemma is one of the workhorse bases the research corpus actually fine-tunes on — it appears in ~98 papers across our census, second only to Qwen among small open models. For the exec that makes it a practical default when picking an SLM to specialize: broadly available, broadly supported, and backed by a frontier lab's pretraining. It's a primary instance of the [[open-models]] ↔ [[small-language-models]] overlap.

## Relationships
- exemplar of [[small-language-models]] and [[open-models]]; sibling families [[phi]], [[nemotron]], [[smollm]], [[qwen]]
- common base for [[post-training]] / [[distillation]] of agent specialists
- deployed as the model tier in [[agentic-ai]]

## Cited by
<!-- Auto-maintained by kg-curator enrich. -->
- **6** · 0.7/mo · [[2025-10-04-arxiv-2510-03847v1-small-language-models-for-agentic-systems-a-survey-of-architectures-ca|Small Language Models for Agentic Systems: A Survey of Architectur…]]
- **2** · 0.3/mo · [[2025-12-10-arxiv-2512-09543v2-swenergy-an-empirical-study-on-energy-efficiency-in-agentic-issue-reso|SWEnergy: An Empirical Study on Energy Efficiency in Agentic Issue…]]
- **0** · [[2025-12-09-arxiv-2512-08211v2-mobilefinetuner-a-mobile-native-framework-for-on-device-llm-fine-tunin|MobileFineTuner: A Mobile-Native Framework for On-Device LLM Fine-…]]
- **0** · [[2026-05-18-arxiv-2605-17774v2-internalizing-tool-knowledge-in-small-language-models-via-qlora-fine-t|Internalizing Tool Knowledge in Small Language Models via QLoRA Fi…]]
- **0** · [[2026-06-03-arxiv-2606-05250v1-towards-persistent-case-based-memory-for-autonomous-data-science-a-cbr|Towards Persistent Case-Based Memory for Autonomous Data Science: …]]
