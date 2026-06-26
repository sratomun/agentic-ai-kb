---
type: source
source_type: arxiv
title: "Towards Verifiably Safe Tool Use for LLM Agents"
authors: Aarya Doshi, Yining Hong, Congying Xu, Eunsuk Kang et al.
url: https://arxiv.org/abs/2601.08012v1
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.SE
tags: [agent-reliability, agent-security, agent-protocols, tool-use, arxiv, auto-ingested]
---

# Towards Verifiably Safe Tool Use for LLM Agents

**arXiv:** [2601.08012v1](https://arxiv.org/abs/2601.08012v1) · 2026-01-12 · cs.SE
**Authors:** Aarya Doshi, Yining Hong, Congying Xu, Eunsuk Kang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM)-based AI agents extend LLM capabilities by enabling access to tools such as data sources, APIs, search engines, code sandboxes, and even other agents. While this empowers agents to perform complex tasks, LLMs may invoke unintended tool interactions and introduce risks, such as leaking sensitive data or overwriting critical records, which are unacceptable in enterprise contexts. Current approaches to mitigate these risks, such as model-based safeguards, enhance agents' reliability but cannot guarantee system safety. Methods like information flow control (IFC) and temporal constraints aim to provide guarantees but often require extensive human annotation. We propose a process that starts with applying System-Theoretic Process Analysis (STPA) to identify hazards in agent workflows, derive safety requirements, and formalize them as enforceable specifications on data flows and tool sequences. To enable this, we introduce a capability-enhanced Model Context Protocol (MCP) framework that requires structured labels on capabilities, confidentiality, and trust level. Together, these contributions aim to shift LLM-based agent safety from ad hoc reliability fixes to proactive guardrails with formal guarantees, while reducing dependence on user confirmation and making autonomy a deliberate design choice.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.08012v1)
