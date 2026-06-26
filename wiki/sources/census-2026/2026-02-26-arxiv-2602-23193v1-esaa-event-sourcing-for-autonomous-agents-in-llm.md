---
type: source
source_type: arxiv
title: "ESAA: Event Sourcing for Autonomous Agents in LLM-Based Software Engineering"
authors: Elzo Brito dos Santos Filho
url: https://arxiv.org/abs/2602.23193v1
date: 2026-02-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [clinical-agents, coding-agents, agent-security, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# ESAA: Event Sourcing for Autonomous Agents in LLM-Based Software Engineering

**arXiv:** [2602.23193v1](https://arxiv.org/abs/2602.23193v1) · 2026-02-26 · cs.AI
**Authors:** Elzo Brito dos Santos Filho

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous agents based on Large Language Models (LLMs) have evolved from reactive assistants to systems capable of planning, executing actions via tools, and iterating over environment observations. However, they remain vulnerable to structural limitations: lack of native state, context degradation over long horizons, and the gap between probabilistic generation and deterministic execution requirements. This paper presents the ESAA (Event Sourcing for Autonomous Agents) architecture, which separates the agent's cognitive intention from the project's state mutation, inspired by the Event Sourcing pattern. In ESAA, agents emit only structured intentions in validated JSON (agent.result or issue.report); a deterministic orchestrator validates, persists events in an append-only log (activity.jsonl), applies file-writing effects, and projects a verifiable materialized view (roadmap.json). The proposal incorporates boundary contracts (AGENT_CONTRACT.yaml), metaprompting profiles (PARCER), and replay verification with hashing (esaa verify), ensuring the immutability of completed tasks and forensic traceability. Two case studies validate the architecture: (i) a landing page project (9 tasks, 49 events, single-agent composition) and (ii) a clinical dashboard system (50 tasks, 86 events, 4 concurrent agents across 8 phases), both concluding with run.status=success and verify_status=ok. The multi-agent case study demonstrates real concurrent orchestration with heterogeneous LLMs (Claude Sonnet 4.6, Codex GPT-5, Antigravity/Gemini 3 Pro, and Claude Opus 4.6), providing empirical evidence of the architecture's scalability beyond single-agent scenarios.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[coding-agents|Coding agents]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[claude]] · [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23193v1)
