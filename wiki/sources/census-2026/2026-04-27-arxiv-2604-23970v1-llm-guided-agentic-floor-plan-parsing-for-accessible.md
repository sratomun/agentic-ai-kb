---
type: source
source_type: arxiv
title: "LLM-Guided Agentic Floor Plan Parsing for Accessible Indoor Navigation of Blind and Low-Vision People"
authors: Aydin Ayanzadeh, Tim Oates
url: https://arxiv.org/abs/2604.23970v1
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [embodied-agents, knowledge-graph, agent-security, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# LLM-Guided Agentic Floor Plan Parsing for Accessible Indoor Navigation of Blind and Low-Vision People

**arXiv:** [2604.23970v1](https://arxiv.org/abs/2604.23970v1) · 2026-04-27 · cs.AI
**Authors:** Aydin Ayanzadeh, Tim Oates

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Indoor navigation remains a critical accessibility challenge for the blind and low-vision (BLV) individuals, as existing solutions rely on costly per-building infrastructure. We present an agentic framework that converts a single floor plan image into a structured, retrievable knowledge base to generate safe, accessible navigation instructions with lightweight infrastructure. The system has two phases: a multi-agent module that parses the floor plan into a spatial knowledge graph through a self-correcting pipeline with iterative retry loops and corrective feedback; and a Path Planner that generates accessible navigation instructions, with a Safety Evaluator agent assessing potential hazards along each route. We evaluate the system on the real-world UMBC Math and Psychology building (floors MP-1 and MP-3) and on the CVC-FP benchmark. On MP-1, we achieve success rates of 92.31%, 76.92%, and 61.54% for short, medium, and long routes, outperforming the strongest single-call baseline (Claude 3.7 Sonnet) at 84.62%, 69.23%, and 53.85%. On MP-3, we reach 76.92%, 61.54%, and 38.46%, compared to the best baseline at 61.54%, 46.15%, and 23.08%. These results show consistent gains over single-call LLM baselines and demonstrate that our workflow is a scalable solution for accessible indoor navigation for BLV individuals.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23970v1)
