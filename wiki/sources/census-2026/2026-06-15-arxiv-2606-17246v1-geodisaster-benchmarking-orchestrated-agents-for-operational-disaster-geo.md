---
type: source
source_type: arxiv
title: "GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence"
authors: Maram Hasan, Aman Verma, Savitra Roy, Hariseetharam Gunduboina et al.
url: https://arxiv.org/abs/2606.17246v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.CV
tags: [clinical-agents, agent-reliability, agentic-rl, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence

**arXiv:** [2606.17246v1](https://arxiv.org/abs/2606.17246v1) · 2026-06-15 · cs.CV
**Authors:** Maram Hasan, Aman Verma, Savitra Roy, Hariseetharam Gunduboina et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Remote-sensing vision-language models (RS-VLMs) have advanced Earth-observation analysis toward visual interpretation and instruction-following, yet fall short of operational geo-intelligence, which demands tool-grounded spatial reasoning and structured, evidence-backed decisions. We introduce GeoDisaster, an operational geospatial disaster reasoning benchmark with 2,921 verified instances across 43 question types and five task families: deforestation monitoring, multi-hazard analysis, building-damage assessment, flood-safe routing, and Sentinel-1 SAR flood monitoring. Instances integrate heterogeneous EO/GIS evidence-optical and SAR imagery, raster masks, vector geometries, road networks, and exposure layers-spanning hazard detection, damage assessment, exposure estimation, and diagnostic report generation. Ground-truth answers are grounded in executable geospatial workflows and deterministic consistency checks, removing the need for language-model annotation. We further propose an orchestrated multi-agent framework with 18 disaster-oriented tools, where role-specialized agents coordinate through explicit execution contracts, aligned via Role-Contract Expectation Alignment (RCEA): failure-aware supervised fine-tuning combined with contract-grounded reinforcement learning over dense step-level signals. Experiments show that GeoDisaster challenges existing RS-VLMs and agentic systems, while RCEA improves tool use, evidence grounding, state consistency, and decision generation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.17246v1)
