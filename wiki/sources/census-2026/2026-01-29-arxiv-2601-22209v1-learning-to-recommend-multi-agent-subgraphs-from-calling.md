---
type: source
source_type: arxiv
title: "Learning to Recommend Multi-Agent Subgraphs from Calling Trees"
authors: Xinyuan Song, Liang Zhao
url: https://arxiv.org/abs/2601.22209v1
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.MA
tags: [recommendation-agents, agent-economies, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Learning to Recommend Multi-Agent Subgraphs from Calling Trees

**arXiv:** [2601.22209v1](https://arxiv.org/abs/2601.22209v1) · 2026-01-29 · cs.MA
**Authors:** Xinyuan Song, Liang Zhao

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent systems (MAS) increasingly solve complex tasks by orchestrating agents and tools selected from rapidly growing marketplaces. As these marketplaces expand, many candidates become functionally overlapping, making selection not just a retrieval problem: beyond filtering relevant agents, an orchestrator must choose options that are reliable, compatible with the current execution context, and able to cooperate with other selected agents. Existing recommender systems -- largely built for item-level ranking from flat user-item logs -- do not directly address the structured, sequential, and interaction-dependent nature of agent orchestration. We address this gap by \textbf{formulating agent recommendation in MAS as a constrained decision problem} and introducing a generic \textbf{constrained recommendation framework} that first uses retrieval to build a compact candidate set conditioned on the current subtask and context, and then performs \textbf{utility optimization} within this feasible set using a learned scorer that accounts for relevance, reliability, and interaction effects. We ground both the formulation and learning signals in \textbf{historical calling trees}, which capture the execution structure of MAS (parent-child calls, branching dependencies, and local cooperation patterns) beyond what flat logs provide. The framework supports two complementary settings: \textbf{agent-level recommendation} (select the next agent/tool) and \textbf{system-level recommendation} (select a small, connected agent team/subgraph for coordinated execution). To enable systematic evaluation, we construct a unified calling-tree benchmark by normalizing invocation logs from eight heterogeneous multi-agent corpora into a shared structured representation.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agent-economies|Agent economies]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.22209v1)
