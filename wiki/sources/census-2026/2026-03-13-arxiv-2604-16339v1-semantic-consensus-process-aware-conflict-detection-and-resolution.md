---
type: source
source_type: arxiv
title: "Semantic Consensus: Process-Aware Conflict Detection and Resolution for Enterprise Multi-Agent LLM Systems"
authors: Vivek Acharya
url: https://arxiv.org/abs/2604.16339v1
date: 2026-03-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agent-protocols, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# Semantic Consensus: Process-Aware Conflict Detection and Resolution for Enterprise Multi-Agent LLM Systems

**arXiv:** [2604.16339v1](https://arxiv.org/abs/2604.16339v1) · 2026-03-13 · cs.AI
**Authors:** Vivek Acharya

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent large language model (LLM) systems are rapidly emerging as the dominant architecture for enterprise AI automation, yet production deployments exhibit failure rates between 41% and 86.7%, with nearly 79% of failures originating from specification and coordination issues rather than model capability limitations. This paper identifies Semantic Intent Divergence--the phenomenon whereby cooperating LLM agents develop inconsistent interpretations of shared objectives due to siloed context and absent process models--as a primary yet formally unaddressed root cause of multi-agent failure in enterprise settings. We propose the Semantic Consensus Framework (SCF), a process-aware middleware comprising six components: a Process Context Layer for shared operational semantics, a Semantic Intent Graph for formal intent representation, a Conflict Detection Engine for real-time identification of contradictory, contention-based, and causally invalid intent combinations, a Consensus Resolution Protocol using a policy--authority--temporal hierarchy, a Drift Monitor for detecting gradual semantic divergence, and a Process-Aware Governance Integration layer for organizational policy enforcement. Evaluation across 600 runs spanning three multi-agent frameworks (AutoGen, CrewAI, LangGraph) and four enterprise scenarios demonstrates that SCF is the only approach to achieve 100% workflow completion--compared to 25.1% for the next-best baseline--while detecting 65.2% of semantic conflicts with 27.9% precision and providing complete governance audit trails. The framework is protocol-agnostic and compatible with MCP and A2A communication standards.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Entities:** [[mcp]] · [[a2a-protocol]] · [[langgraph]] · [[autogen]] · [[crewai]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.16339v1)
