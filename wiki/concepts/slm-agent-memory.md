---
type: concept
tags: [agents, small-language-models, agent-memory]
created: 2026-06-23
updated: 2026-06-23
kind: crosscutting
census_count: 9
---

# SLM Agent Memory

*External, structured memory for small-model agents — the layer that compensates for what a small context window and a small model can't hold on their own.*

## What it is
Memory architectures designed specifically for [[small-language-models]] agents: orchestrating what gets recalled, organizing it (clustering, case-based stores, modular per-persona memory), and keeping it cheap enough to run on-device. It's a specialization of [[agent-memory]] under a hard constraint — when the model is small and often runs locally, you can't lean on a huge context window or a frontier model's implicit recall, so memory has to be *externalized and engineered*.

## Why it matters
For small-model agents, memory is the binding constraint, not an add-on. A 1–8B model with a modest context window forgets fast, so long-horizon coherence has to come from an external store — which means the quality of the *memory system* often matters more than the marginal quality of the model. For the exec the implication is architectural: the leverage in an SLM-first agent is in retrieval, organization, and forgetting policy, and getting that right is what lets a cheap local model behave like a much larger one over a long task.

## What the evidence shows
The 2026 corpus shows memory being built *for* small models rather than inherited from LLM setups: intent-driven memory orchestration for SLM agents (→ [[2026-05-05-arxiv-2605-03312v1-memflow-intent-driven-memory-orchestration-for-small-language-model-ag|MemFlow]]), agent-driven clustering to organize memory adaptively (→ [[2026-03-16-arxiv-2603-15421v2-clag-adaptive-memory-organization-via-agent-driven-clustering-for-smal|CLAG]]), and explicitly lightweight agent memory using small models (→ [[2026-04-09-arxiv-2604-07798v3-lightweight-llm-agent-memory-with-small-language-models|Lightweight LLM Agent Memory with SLMs]]). A distinct **on-device** thread keeps memory local and personalized — bio-inspired on-device personalized memory (→ [[2026-05-05-arxiv-2605-03804v2-scrapmem-a-bio-inspired-framework-for-on-device-personalized-agent-mem|ScrapMem]]), preference-aligned memory for on-device RAG (→ [[2026-05-18-arxiv-2605-18271v2-from-volume-to-value-preference-aligned-memory-construction-for-on-dev|From Volume to Value]]), and persistent case-based memory with a locally-deployable small model (→ [[2026-06-03-arxiv-2606-05250v1-towards-persistent-case-based-memory-for-autonomous-data-science-a-cbr|persistent case-based memory]]). *(Evidence is abstract-tier — directional, not figure-grounded.)*

## Relationships
- specialization of [[agent-memory]] for [[small-language-models]]
- frequently built as external retrieval → overlaps [[agentic-rag]] and structured stores in [[knowledge-graph]]
- a core reliability lever for [[on-device-agents]] (local, personalized memory)

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. -->
- **1** · 0.1/mo · [[2025-10-17-arxiv-2510-15620v2-on-device-semantic-selection-made-low-latency-and-memory-efficient-wit|On-device Semantic Selection Made Low Latency and Memory Efficient…]]
- **0** · [[2025-09-24-arxiv-2511-03728v1-efficient-on-device-agents-via-adaptive-context-management|Efficient On-Device Agents via Adaptive Context Management]]
- **0** · [[2025-11-13-arxiv-2511-10277v1-fixed-persona-slms-with-modular-memory-scalable-npc-dialogue-on-consum|Fixed-Persona SLMs with Modular Memory: Scalable NPC Dialogue on C…]]
- **0** · [[2026-05-05-arxiv-2605-03312v1-memflow-intent-driven-memory-orchestration-for-small-language-model-ag|MemFlow: Intent-Driven Memory Orchestration for Small Language Mod…]]
- **0** · [[2026-06-03-arxiv-2606-05250v1-towards-persistent-case-based-memory-for-autonomous-data-science-a-cbr|Towards Persistent Case-Based Memory for Autonomous Data Science: …]]
- **0** · [[2026-05-05-arxiv-2605-03804v2-scrapmem-a-bio-inspired-framework-for-on-device-personalized-agent-mem|ScrapMem: A Bio-inspired Framework for On-device Personalized Agen…]]
