---
type: source
source_type: arxiv
title: "Catalyst-Agent: Autonomous heterogeneous catalyst screening with an LLM Agent"
authors: Achuth Chandrasekhar, Janghoon Ock, Amir Barati Farimani
url: https://arxiv.org/abs/2603.01311v2
date: 2026-03-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [agent-protocols, tool-use, arxiv, auto-ingested]
---

# Catalyst-Agent: Autonomous heterogeneous catalyst screening with an LLM Agent

**arXiv:** [2603.01311v2](https://arxiv.org/abs/2603.01311v2) · 2026-03-01 · cs.CL
**Authors:** Achuth Chandrasekhar, Janghoon Ock, Amir Barati Farimani

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The discovery of novel catalysts tailored for particular applications is a major challenge for the twenty-first century. Traditional methods for this include time-consuming and expensive experimental trial-and-error approaches in labs based on chemical theory or heavily computational first-principles approaches based on density functional theory. Recent studies show that deep learning models like graph neural networks (GNNs) can significantly speed up the screening of catalyst materials by many orders of magnitude, with very high accuracy and fidelity. In this work, we introduce Catalyst-Agent, a Model Context Protocol (MCP) server-based, LLM-powered AI agent. It can explore vast material databases using the OPTIMADE API, make structural modifications, calculate adsorption energies using Meta FAIRchem's UMA (GNN) model via FAIRchem's AdsorbML workflow and slab construction, and make useful material suggestions to the researcher in a closed-loop manner, including structural modifications to refine near-miss candidates. It is tested on three pivotal reactions: the oxygen reduction reaction (ORR), the nitrogen reduction reaction (NRR), and the CO2 reduction reaction (CO2RR). Catalyst-Agent achieves a success rate of 33-41% among all the materials it chooses and evaluates, and manages to converge in 1-4 trials per successful material on average. This work demonstrates the potential of AI agents to exercise their planning capabilities and tool use for autonomous catalyst screening workflows.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01311v2)
