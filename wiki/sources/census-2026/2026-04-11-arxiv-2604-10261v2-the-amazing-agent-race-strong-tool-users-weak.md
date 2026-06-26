---
type: source
source_type: arxiv
title: "The Amazing Agent Race: Strong Tool Users, Weak Navigators"
authors: Zae Myung Kim, Dongseok Lee, Jaehyung Kim, Vipul Raheja et al.
url: https://arxiv.org/abs/2604.10261v2
date: 2026-04-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, embodied-agents, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# The Amazing Agent Race: Strong Tool Users, Weak Navigators

**arXiv:** [2604.10261v2](https://arxiv.org/abs/2604.10261v2) · 2026-04-11 · cs.AI
**Authors:** Zae Myung Kim, Dongseok Lee, Jaehyung Kim, Vipul Raheja et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing tool-use benchmarks for LLM agents are overwhelmingly linear: our analysis of six benchmarks shows 55 to 100% of instances are simple chains of 2 to 5 steps. We introduce The Amazing Agent Race (AAR), a benchmark featuring directed acyclic graph (DAG) puzzles (or "legs") with fork-merge tool chains. We release 1,400 instances across two variants: sequential (800 legs) and compositional (600 DAG legs). Agents must navigate Wikipedia, execute multi-step tool chains, and aggregate results into a verifiable answer. Legs are procedurally generated from Wikipedia seeds across four difficulty levels with live-API validation. Three complementary metrics (finish-line accuracy, pit-stop visit rate, and roadblock completion rate) separately diagnose navigation, tool-use, and arithmetic failures. Evaluating three agent frameworks on 1,400 legs, the best achieves only 37.2% accuracy. Navigation errors dominate (27 to 52% of trials) while tool-use errors remain below 17%, and agent architecture matters as much as model scale (Claude Code matches Codex CLI at 37% with 6x fewer tokens). The compositional structure of AAR reveals that agents fail not at calling tools but at navigating to the right pages, a blind spot invisible to linear benchmarks. The project page can be accessed at: https://minnesotanlp.github.io/the-amazing-agent-race

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[embodied-agents|Embodied agents]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.10261v2)
