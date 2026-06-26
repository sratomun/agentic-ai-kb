---
type: source
source_type: arxiv
title: "PRISM: Protocol Refinement through Intelligent Simulation Modeling"
authors: Brian Hsu, Priyanka V Setty, Rory M Butler, Ryan Lewis et al.
url: https://arxiv.org/abs/2601.05356v1
date: 2026-01-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.RO
tags: [autonomous-driving-agents, embodied-agents, agent-protocols, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# PRISM: Protocol Refinement through Intelligent Simulation Modeling

**arXiv:** [2601.05356v1](https://arxiv.org/abs/2601.05356v1) · 2026-01-08 · cs.RO
**Authors:** Brian Hsu, Priyanka V Setty, Rory M Butler, Ryan Lewis et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Automating experimental protocol design and execution remains as a fundamental bottleneck in realizing self-driving laboratories. We introduce PRISM (Protocol Refinement through Intelligent Simulation Modeling), a framework that automates the design, validation, and execution of experimental protocols on a laboratory platform composed of off-the-shelf robotic instruments. PRISM uses a set of language-model-based agents that work together to generate and refine experimental steps. The process begins with automatically gathering relevant procedures from web-based sources describing experimental workflows. These are converted into structured experimental steps (e.g., liquid handling steps, deck layout and other related operations) through a planning, critique, and validation loop. The finalized steps are translated into the Argonne MADSci protocol format, which provides a unified interface for coordinating multiple robotic instruments (Opentrons OT-2 liquid handler, PF400 arm, Azenta plate sealer and peeler) without requiring human intervention between steps. To evaluate protocol-generation performance, we benchmarked both single reasoning models and multi-agent workflow across constrained and open-ended prompting paradigms. The resulting protocols were validated in a digital-twin environment built in NVIDIA Omniverse to detect physical or sequencing errors before execution. Using Luna qPCR amplification and Cell Painting as case studies, we demonstrate PRISM as a practical end-to-end workflow that bridges language-based protocol generation, simulation-based validation, and automated robotic execution.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.05356v1)
