---
type: source
source_type: arxiv
title: "A Novel Hierarchical Multi-Agent System for Payments Using LLMs"
authors: Joon Kiat Chua, Donghao Huang, Zhaoxia Wang
url: https://arxiv.org/abs/2602.24068v1
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.MA
tags: [computer-use-agents, multi-agent-systems, arxiv, auto-ingested]
---

# A Novel Hierarchical Multi-Agent System for Payments Using LLMs

**arXiv:** [2602.24068v1](https://arxiv.org/abs/2602.24068v1) · 2026-02-27 · cs.MA
**Authors:** Joon Kiat Chua, Donghao Huang, Zhaoxia Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM) agents, such as OpenAI's Operator and Claude's Computer Use, can automate workflows but unable to handle payment tasks. Existing agentic solutions have gained significant attention; however, even the latest approaches face challenges in implementing end-to-end agentic payment workflows. To address this gap, this research proposes the Hierarchical Multi-Agent System for Payments (HMASP), which provides an end-to-end agentic method for completing payment workflows. The proposed HMASP leverages either open-weight or proprietary LLMs and employs a modular architecture consisting of the Conversational Payment Agent (CPA - first agent level), Supervisor agents (second agent level), Routing agents (third agent level), and the Process summary agent (fourth agent level). The CPA serves as the central entry point, handling all external requests and coordinating subsequent tasks across hierarchical levels. HMASP incorporates architectural patterns that enable modular task execution across agents and levels for payment operations, including shared state variables, decoupled message states, and structured handoff protocols that facilitate coordination across agents and workflows. Experimental results demonstrate the feasibility of the proposed HMASP. To our knowledge, HMASP is the first LLM-based multi-agent system to implement end-to-end agentic payment workflows. This work lays a foundation for extending agentic capabilities into the payment domain.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.24068v1)
