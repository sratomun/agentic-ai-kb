---
type: source
source_type: arxiv
title: "Making OpenAPI Documentation Agent-Ready: Detecting Documentation and REST Smells with a Multi-Agent LLM System"
authors: Rayfran Rocha Lima, Davi G. Assunção Pinheiro, Thiago Medeiros de Menezes
url: https://arxiv.org/abs/2605.14312v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.SE
tags: [clinical-agents, agent-protocols, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# Making OpenAPI Documentation Agent-Ready: Detecting Documentation and REST Smells with a Multi-Agent LLM System

**arXiv:** [2605.14312v1](https://arxiv.org/abs/2605.14312v1) · 2026-05-14 · cs.SE
**Authors:** Rayfran Rocha Lima, Davi G. Assunção Pinheiro, Thiago Medeiros de Menezes

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The growing adoption of AI agents and the Model Context Protocol (MCP) has motivated organizations to expose existing REST APIs as agent-consumable tools. In our industrial context, this initiative targeted an ecosystem of 16 production APIs comprising approximately 600 endpoints. Although these APIs were stable and widely used within a microservice architecture, early proof-of-concept experiments revealed systematic failures in task planning, tool selection, and payload construction when accessed through MCP-based agents. Rather than attributing these failures to model limitations alone, we conducted an ecosystem-scale empirical assessment of the underlying OpenAPI documentation. We developed Hermes, a multi-agent LLM-based system that detects documentation and REST-related smells at the endpoint level and generates explainable diagnostic reports. The large-scale evaluation identified 2,450 smells across 600 endpoints, with deficiencies present in all analyzed operations. Practitioner validation confirmed high agreement with the detected issues while also revealing contextual trade-offs in remediation decisions. The findings suggested that structural validity within microservice environments does not guarantee semantic readiness for agent-based consumption. Based on this evidence, the organization revised its adoption strategy, prioritizing selective endpoint adaptation, redefining documentation standards, and integrating automated documentation assessment into API governance workflows. This case illustrates how systematic artifact-level evaluation can function as a strategic decision-support mechanism, reducing technological risk and guiding evidence-based AI adoption in industrial software ecosystems.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14312v1)
