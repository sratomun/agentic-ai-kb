---
type: source
source_type: arxiv
title: "GraphPilot: GUI Task Automation with One-Step LLM Reasoning Powered by Knowledge Graph"
authors: Mingxian Yu, Siqi Luo, Xu Chen
url: https://arxiv.org/abs/2601.17418v1
date: 2026-01-24
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.HC
tags: [computer-use-agents, knowledge-graph, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# GraphPilot: GUI Task Automation with One-Step LLM Reasoning Powered by Knowledge Graph

**arXiv:** [2601.17418v1](https://arxiv.org/abs/2601.17418v1) · 2026-01-24 · cs.HC
**Authors:** Mingxian Yu, Siqi Luo, Xu Chen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Mobile graphical user interface (GUI) agents are designed to automate everyday tasks on smartphones. Recent advances in large language models (LLMs) have significantly enhanced the capabilities of mobile GUI agents. However, most LLM-powered mobile GUI agents operate in stepwise query-act loops, which incur high latency due to repeated LLM queries. We present GraphPilot, a mobile GUI agent that leverages knowledge graphs of the target apps to complete user tasks in almost one LLM query. GraphPilot operates in two complementary phases to enable efficient and reliable LLM-powered GUI task automation. In the offline phase, it explores target apps, records and analyzes interaction history, and constructs an app-specific knowledge graph that encodes functions of pages and elements as well as transition rules for each app. In the online phase, given an app and a user task, it leverages the knowledge graph of the given app to guide the reasoning process of LLM. When the reasoning process encounters uncertainty, GraphPilot dynamically requests the HTML representation of the current interface to refine subsequent reasoning. Finally, a validator checks the generated sequence of actions against the transition rules in the knowledge graph, performing iterative corrections to ensure it is valid. The structured, informative information in the knowledge graph allows the LLM to plan the complete sequence of actions required to complete the user task. On the DroidTask benchmark, GraphPilot improves task completion rate over Mind2Web and AutoDroid, while substantially reducing latency and the number of LLM queries.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17418v1)
