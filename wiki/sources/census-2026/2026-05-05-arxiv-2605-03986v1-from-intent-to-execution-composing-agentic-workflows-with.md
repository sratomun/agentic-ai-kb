---
type: source
source_type: arxiv
title: "From Intent to Execution: Composing Agentic Workflows with Agent Recommendation"
authors: Kishan Athrey, Ramin Pishehvar, Brian Riordan, Mahesh Viswanathan
url: https://arxiv.org/abs/2605.03986v1
date: 2026-05-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [recommendation-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# From Intent to Execution: Composing Agentic Workflows with Agent Recommendation

**arXiv:** [2605.03986v1](https://arxiv.org/abs/2605.03986v1) · 2026-05-05 · cs.AI
**Authors:** Kishan Athrey, Ramin Pishehvar, Brian Riordan, Mahesh Viswanathan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-Agent Systems (MAS) built using AI agents fulfill a variety of user intents that may be used to design and build a family of related applications. However, the creation of such MAS currently involves manual composition of the plan, manual selection of appropriate agents, and manual creation of execution graphs. This paper introduces a framework for the automated creation of multi-agent systems which replaces multiple manual steps with an automated framework. The proposed framework consists of software modules and a workflow to orchestrate the requisite task- specific application. The modules include: an LLM-derived planner, a set of tasks described in natural language, a dynamic call graph, an orchestrator for map agents to tasks, and an agent recommender that finds the most suitable agent(s) from local and global agent registries. The agent recommender uses a two-stage information retrieval (IR) system comprising a fast retriever and an LLM-based re-ranker. We implemented a series of experiments exploring the choice of embedders, re- rankers, agent description enrichment, and supervising critique agent. We benchmarked this system end-to-end, evaluating the combination of planning, agent selection, and task completion, with our proposed approach. Our experimental results show that our approach outperforms the state-of-the- art in terms of the recall rate and is more robust and scalable compared to previous approaches. The critique agent holistically reevaluates both agent and tool recommendations against the overall plan. We show that the inclusion of the critique agent further enhances the recall score, proving that the comprehensive review and revision of task-based agent selection is an essential step in building end-to-end multi-agent systems.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.03986v1)
