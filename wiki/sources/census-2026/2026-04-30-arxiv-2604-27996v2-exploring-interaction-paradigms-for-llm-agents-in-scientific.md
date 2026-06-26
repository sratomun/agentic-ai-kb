---
type: source
source_type: arxiv
title: "Exploring Interaction Paradigms for LLM Agents in Scientific Visualization"
authors: Jackson Vonderhorst, Kuangshi Ai, Haichao Miao, Shusen Liu et al.
url: https://arxiv.org/abs/2604.27996v2
date: 2026-04-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [coding-agents, computer-use-agents, agent-reliability, agent-protocols, agent-memory, arxiv, auto-ingested]
---

# Exploring Interaction Paradigms for LLM Agents in Scientific Visualization

**arXiv:** [2604.27996v2](https://arxiv.org/abs/2604.27996v2) · 2026-04-30 · cs.AI
**Authors:** Jackson Vonderhorst, Kuangshi Ai, Haichao Miao, Shusen Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper examines how different types of large language model (LLM) agents perform on scientific visualization (SciVis) tasks, where users generate visualization workflows from natural-language instructions. We compare three primary interaction paradigms, including domain-specific agents with structured tool use, computer-use agents, and general-purpose coding agents, by evaluating eight representative agents across 15 benchmark tasks and measuring visualization quality, efficiency, robustness, and computational cost. We further analyze interaction modalities, including code scripts and model context protocol (MCP) or API calls for structured tool use, as well as command-line interfaces (CLI) and graphical user interfaces (GUI) for more general interaction, while additionally studying the effect of persistent memory in selected agents. The results reveal clear tradeoffs across paradigms and modalities. General-purpose coding agents achieve the highest task success rates but are computationally expensive, while domain-specific agents are more efficient and stable but less flexible. Computer-use agents perform well on individual steps but struggle with longer multi-step workflows, indicating that long-horizon planning is their primary limitation. Across both CLI- and GUI-based settings, persistent memory improves performance over repeated trials, although its benefits depend on the underlying interaction mode and the quality of feedback. These findings suggest that no single approach is sufficient, and future SciVis systems should combine structured tool use, interactive capabilities, and adaptive memory mechanisms to balance performance, robustness, and flexibility.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.27996v2)
