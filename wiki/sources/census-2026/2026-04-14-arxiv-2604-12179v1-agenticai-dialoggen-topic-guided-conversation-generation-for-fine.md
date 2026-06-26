---
type: source
source_type: arxiv
title: "AgenticAI-DialogGen: Topic-Guided Conversation Generation for Fine-Tuning and Evaluating Short- and Long-Term Memories of LLMs"
authors: Manoj Madushanka Perera, Adnan Mahmood, Kasun Eranda Wijethilake, Quan Z. Sheng
url: https://arxiv.org/abs/2604.12179v1
date: 2026-04-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.CL
tags: [knowledge-graph, agent-memory, arxiv, auto-ingested]
---

# AgenticAI-DialogGen: Topic-Guided Conversation Generation for Fine-Tuning and Evaluating Short- and Long-Term Memories of LLMs

**arXiv:** [2604.12179v1](https://arxiv.org/abs/2604.12179v1) · 2026-04-14 · cs.CL
**Authors:** Manoj Madushanka Perera, Adnan Mahmood, Kasun Eranda Wijethilake, Quan Z. Sheng

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advancements in Large Language Models (LLMs) have improved their ability to process extended conversational contexts, yet fine-tuning and evaluating short- and long-term memories remain difficult due to the absence of datasets that encode both short- and long-term conversational history. Existing conversational datasets lack memory grounding, overlook topic continuity, or rely on costly human annotation. To address these gaps, we introduce AgenticAI-DialogGen, a modular agent-based framework that generates persona-grounded and topic-guided conversations without human supervision. The framework uses LLM agents to extract knowledge graphs, identify topics, build speaker personas, and simulate topic-guided conversations from unstructured conversations. A QA module generates memory-grounded Question Answer (QA) pairs drawn from short- and long-term conversational histories. We also generated a new dataset entitled, TopicGuidedChat (TGC), where long-term memory is encoded as speaker-specific knowledge graphs and short-term memory as newly generated topic-guided conversations. Evaluations depict that AgenticAI-DialogGen yields higher conversational quality and LLMs fine-tuned on TGC dataset achieve improved performance on memory-grounded QA tasks.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.12179v1)
