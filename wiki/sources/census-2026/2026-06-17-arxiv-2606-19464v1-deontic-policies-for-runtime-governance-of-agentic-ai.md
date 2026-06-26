---
type: source
source_type: arxiv
title: "Deontic Policies for Runtime Governance of Agentic AI Systems"
authors: Anupam Joshi, Tim Finin, Karuna Pande Joshi, Lalana Kagal
url: https://arxiv.org/abs/2606.19464v1
date: 2026-06-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-security, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Deontic Policies for Runtime Governance of Agentic AI Systems

**arXiv:** [2606.19464v1](https://arxiv.org/abs/2606.19464v1) · 2026-06-17 · cs.AI
**Authors:** Anupam Joshi, Tim Finin, Karuna Pande Joshi, Lalana Kagal

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous agentic AI systems driven by Large Language Models (LLMs) introduce a new class of security, privacy, and compliance challenges: an agent that can invoke tools, manipulate data, install software, and coordinate with peer agents across organizational boundaries must be constrained not just by authentication and access control, but by the full structure of enterprise governance. This includes specifying what agents are permitted and prohibited from doing, what they areobliged to do after certain actions (e.g., notify the CISO), under what conditions a standing obligation may be waived, and which rules take precedence when policies conflict. This governance problem exceeds what current policy engines provide. Systems such as XACML, Rego, and Cedar address only the permit/prohibit subset of this governance structure. They do not provide obligation lifecycle management, meta-policy conflict resolution, dispensations that waive obligations in specific circumstances, and ontological reasoning over domain class hierarchies commonly found in applications such as healthcare, cybersecurity, or data privacy. We propose AgenticRei, which realizes key governance requirements such as obligations, dispensations, policy conflict resolutions, and reasoning over policies, as well as the basic permit/prohibit constraints. We use a deontic policy language built on the Rei framework, expressed as OWL (Web Ontology Language) and evaluated at runtime by a high-performance logic engine entirely outside the LLM. The same pipeline governs both tool invocations by the agent and agent-to-agent messages. We show through examples that deontic policies capture governance constraints around security and privacy that mostly cannot be expressed in current production engines. Our approach composes naturally with industry-standard frameworks like A2AS.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.19464v1)
