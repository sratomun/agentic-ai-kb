---
type: source
source_type: arxiv
title: "UI-KOBE: Knowledge-Oriented Behavior Exploration for Lightweight Graph-Guided GUI Agents"
authors: Yuxiang Chai, Han Xiao, Xinyu Fu, Jinpeng Chen et al.
url: https://arxiv.org/abs/2605.29534v1
date: 2026-05-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [computer-use-agents, knowledge-graph, agent-reliability, agent-memory, arxiv, auto-ingested]
---

# UI-KOBE: Knowledge-Oriented Behavior Exploration for Lightweight Graph-Guided GUI Agents

**arXiv:** [2605.29534v1](https://arxiv.org/abs/2605.29534v1) · 2026-05-28 · cs.AI
**Authors:** Yuxiang Chai, Han Xiao, Xinyu Fu, Jinpeng Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in mobile GUI agents have shown strong potential for automating mobile tasks, but most effective systems still depend on large vision-language models for screenshot understanding and long-horizon planning. Small GUI agents that can be deployed directly on mobile devices are more attractive for practical use, offering lower inference cost and better protection of sensitive on-device information. However, due to limited model capacity, such lightweight agents remain unreliable when planning and executing GUI tasks end-to-end from screenshots alone. We propose Knowledge-Oriented Behavior Exploration (\textbf{UI-KOBE}), a framework that improves lightweight mobile GUI agents with reusable app-specific graph knowledge. UI-KOBE first autonomously explores a mobile application and constructs an app knowledge graph, where nodes represent distinct UI states and edges represent executable transitions. At runtime, a lightweight GUI agent uses the graph as external guidance: given a user task and the current screenshot, it identifies the current graph node and selects among self-loop actions, neighboring transitions, task completion, or fallback free actions associated with that node. By supporting runtime decisions with app-specific graph guidance, UI-KOBE reduces the burden of end-to-end GUI planning and helps lightweight models perform mobile GUI tasks more effectively, offering a practical step toward efficient, interpretable, and privacy-conscious on-device GUI agents.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.29534v1)
