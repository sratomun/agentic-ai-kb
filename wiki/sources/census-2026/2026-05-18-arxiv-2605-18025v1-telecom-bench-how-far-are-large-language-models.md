---
type: source
source_type: arxiv
title: "TeleCom-Bench: How Far Are Large Language Models from Industrial Telecommunication Applications?"
authors: Jieting Xiao, Yun Lin, Huizhen Qiu, Rui Ma et al.
url: https://arxiv.org/abs/2605.18025v1
date: 2026-05-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-reliability, agent-skills, tool-use, arxiv, auto-ingested]
---

# TeleCom-Bench: How Far Are Large Language Models from Industrial Telecommunication Applications?

**arXiv:** [2605.18025v1](https://arxiv.org/abs/2605.18025v1) · 2026-05-18 · cs.AI
**Authors:** Jieting Xiao, Yun Lin, Huizhen Qiu, Rui Ma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While Large Language Models have achieved remarkable integration in various vertical scenarios, their deployment in the telecommunications domain remains exploratory due to the lack of a standardized evaluation framework. Current telecom benchmarks primarily focus on static, foundational knowledge and isolated atomic skills, neglecting the equipment-specific documentation and end-to-end industrial workflows essential for real-world production systems. To bridge this gap, we present TeleCom-Bench, a comprehensive benchmark comprising 12 evaluation sets with 22,678 curated samples, which evaluates LLMs across a synergistic hierarchy: (1) Multi-dimensional Knowledge Comprehension, which integrates telecommunication fundamentals, 3GPP protocols, and 5G network architecture with proprietary product knowledge across wired, core, and wireless networks via knowledge graph-driven synthesis; and (2)End-to-End Knowledge Application, which formalizes six core tasks on authentic trajectories from live network agent workflows, including intent recognition, entity extraction, event verification, tool invocation, root cause analysis, and solution generation-across network optimization and fault maintenance scenarios. Evaluations of eight state-of-the-art LLMs reveal a universal Execution Wall: while models achieve 90% accuracy in linguistic interface tasks such as intent recognition and entity extraction, performance collapses to approximately 30% in procedural execution tasks like solution generation. This capability gap demonstrates that current LLMs function competently as diagnosticians but fail as field engineers. TeleCom-Bench provides standardized diagnostics to precisely pinpoint this deficit, offering actionable guidance for domain-specific alignment toward production-ready telecom agents. The dataset and evaluation code have been released at https://github.com/ZTE-AICloud/TeleCom-Bench.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-skills|Agent skills]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.18025v1)
