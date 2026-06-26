---
type: source
source_type: arxiv
title: "AgentRob: From Virtual Forum Agents to Hijacked Physical Robots"
authors: Wenrui Liu, Yaxuan Wang, Xun Zhang, Yanshu Wang et al.
url: https://arxiv.org/abs/2602.13591v1
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.RO
tags: [embodied-agents, agent-protocols, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# AgentRob: From Virtual Forum Agents to Hijacked Physical Robots

**arXiv:** [2602.13591v1](https://arxiv.org/abs/2602.13591v1) · 2026-02-14 · cs.RO
**Authors:** Wenrui Liu, Yaxuan Wang, Xun Zhang, Yanshu Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM)-powered autonomous agents have demonstrated significant capabilities in virtual environments, yet their integration with the physical world remains narrowly confined to direct control interfaces. We present AgentRob, a framework that bridges online community forums, LLM-powered agents, and physical robots through the Model Context Protocol (MCP). AgentRob enables a novel paradigm where autonomous agents participate in online forums--reading posts, extracting natural language commands, dispatching physical robot actions, and reporting results back to the community. The system comprises three layers: a Forum Layer providing asynchronous, persistent, multi-agent interaction; an Agent Layer with forum agents that poll for @mention-targeted commands; and a Robot Layer with VLM-driven controllers and Unitree Go2/G1 hardware that translate commands into robot primitives via iterative tool calling. The framework supports multiple concurrent agents with distinct identities and physical embodiments coexisting in the same forum, establishing the feasibility of forum-mediated multi-agent robot orchestration.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13591v1)
