---
type: source
source_type: arxiv
title: "EntWorld: A Holistic Environment and Benchmark for Verifiable Enterprise GUI Agents"
authors: Ying Mo, Yu Bai, Dapeng Sun, Yuqian Shi et al.
url: https://arxiv.org/abs/2601.17722v1
date: 2026-01-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [computer-use-agents, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# EntWorld: A Holistic Environment and Benchmark for Verifiable Enterprise GUI Agents

**arXiv:** [2601.17722v1](https://arxiv.org/abs/2601.17722v1) · 2026-01-25 · cs.AI
**Authors:** Ying Mo, Yu Bai, Dapeng Sun, Yuqian Shi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Multimodal Large Language Models (MLLMs) have enabled agents to operate in open-ended web and operating system environments. However, existing benchmarks predominantly target consumer-oriented scenarios (e.g., e-commerce and travel booking), failing to capture the complexity and rigor of professional enterprise workflows. Enterprise systems pose distinct challenges, including high-density user interfaces, strict business logic constraints, and a strong reliance on precise, state-consistent information retrieval-settings in which current generalist agents often struggle. To address this gap, we introduce EntWorld, a large-scale benchmark consisting of 1,756 tasks across six representative enterprise domains, including customer relationship management (CRM), information technology infrastructure library (ITIL), and enterprise resource planning (ERP) systems. Unlike previous datasets that depend on fragile execution traces or extensive manual annotation, EntWorld adopts a schema-grounded task generation framework that directly reverse-engineers business logic from underlying database schemas, enabling the synthesis of realistic, long-horizon workflows. Moreover, we propose a SQL-based deterministic verification mechanism in building datasets that replaces ambiguous visual matching with rigorous state-transition validation. Experimental results demonstrate that state-of-the-art models (e.g., GPT-4.1) achieve 47.61% success rate on EntWorld, substantially lower than the human performance, highlighting a pronounced enterprise gap in current agentic capabilities and the necessity of developing domain-specific agents. We release EntWorld as a rigorous testbed to facilitate the development and evaluation of the next generation of enterprise-ready digital agents.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17722v1)
