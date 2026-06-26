---
type: source
source_type: arxiv
title: "Ask or Assume? Uncertainty-Aware Clarification-Seeking in Coding Agents"
authors: Nicholas Edwards, Sebastian Schuster
url: https://arxiv.org/abs/2603.26233v2
date: 2026-03-27
depth: abstract
auto: true
score: 9
primary: cs.CL
tags: [intent-understanding, coding-agents, human-agent-interaction, arxiv, auto-ingested]
---

# Ask or Assume? Uncertainty-Aware Clarification-Seeking in Coding Agents

**arXiv:** [2603.26233v2](https://arxiv.org/abs/2603.26233v2) · 2026-03-27 · cs.CL
**Authors:** Nicholas Edwards, Sebastian Schuster

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
As Large Language Model (LLM) agents are increasingly deployed in open-ended domains like software engineering, they frequently encounter underspecified instructions that lack crucial context. While human developers naturally resolve underspecification by asking clarifying questions, current agents are largely optimized for autonomous execution. In this work, we systematically evaluate the clarification-seeking abilities of LLM agents on an underspecified variant of SWE-bench Verified. We propose an uncertainty-aware multi-agent scaffold that decouples underspecification detection from code execution. Across both proprietary and open-weight frontier LLMs, our scaffold achieves a 69.40% task resolve rate, significantly outperforming a standard single-agent setup and closing the performance gap with agents operating on fully specified instructions. Furthermore, we find that the multi-agent system exhibits well-calibrated information-seeking behavior, conserving queries on simple tasks while proactively seeking information on more complex issues. These findings indicate that current models can be turned into proactive collaborators, where agents independently recognize when to ask questions to elicit missing information in real-world, underspecified tasks.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[coding-agents|Coding agents]] · [[human-agent-interaction|Human-agent interaction]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.26233v2)
