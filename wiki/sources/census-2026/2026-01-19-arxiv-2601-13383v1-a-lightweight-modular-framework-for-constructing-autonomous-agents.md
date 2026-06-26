---
type: source
source_type: arxiv
title: "A Lightweight Modular Framework for Constructing Autonomous Agents Driven by Large Language Models: Design, Implementation, and Applications in AgentForge"
authors: Akbar Anbar Jafari, Cagri Ozcinar, Gholamreza Anbarjafari
url: https://arxiv.org/abs/2601.13383v1
date: 2026-01-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [agent-skills, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# A Lightweight Modular Framework for Constructing Autonomous Agents Driven by Large Language Models: Design, Implementation, and Applications in AgentForge

**arXiv:** [2601.13383v1](https://arxiv.org/abs/2601.13383v1) · 2026-01-19 · cs.AI
**Authors:** Akbar Anbar Jafari, Cagri Ozcinar, Gholamreza Anbarjafari

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The emergence of LLMs has catalyzed a paradigm shift in autonomous agent development, enabling systems capable of reasoning, planning, and executing complex multi-step tasks. However, existing agent frameworks often suffer from architectural rigidity, vendor lock-in, and prohibitive complexity that impedes rapid prototyping and deployment. This paper presents AgentForge, a lightweight, open-source Python framework designed to democratize the construction of LLM-driven autonomous agents through a principled modular architecture. AgentForge introduces three key innovations: (1) a composable skill abstraction that enables fine-grained task decomposition with formally defined input-output contracts, (2) a unified LLM backend interface supporting seamless switching between cloud-based APIs and local inference engines, and (3) a declarative YAML-based configuration system that separates agent logic from implementation details. We formalize the skill composition mechanism as a directed acyclic graph (DAG) and prove its expressiveness for representing arbitrary sequential and parallel task workflows. Comprehensive experimental evaluation across four benchmark scenarios demonstrates that AgentForge achieves competitive task completion rates while reducing development time by 62% compared to LangChain and 78% compared to direct API integration. Latency measurements confirm sub-100ms orchestration overhead, rendering the framework suitable for real-time applications. The modular design facilitates extension: we demonstrate the integration of six built-in skills and provide comprehensive documentation for custom skill development. AgentForge addresses a critical gap in the LLM agent ecosystem by providing researchers and practitioners with a production-ready foundation for constructing, evaluating, and deploying autonomous agents without sacrificing flexibility or performance.

## Graph
- **Concepts:** [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.13383v1)
