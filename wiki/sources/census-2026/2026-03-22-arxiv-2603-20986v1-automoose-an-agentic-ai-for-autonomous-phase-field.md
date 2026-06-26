---
type: source
source_type: arxiv
title: "AutoMOOSE: An Agentic AI for Autonomous Phase-Field Simulation"
authors: Sukriti Manna, Henry Chan, Subramanian K. R. S. Sankaranarayanan
url: https://arxiv.org/abs/2603.20986v1
date: 2026-03-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [autonomous-driving-agents, clinical-agents, science-agents, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# AutoMOOSE: An Agentic AI for Autonomous Phase-Field Simulation

**arXiv:** [2603.20986v1](https://arxiv.org/abs/2603.20986v1) · 2026-03-22 · cs.AI
**Authors:** Sukriti Manna, Henry Chan, Subramanian K. R. S. Sankaranarayanan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multiphysics simulation frameworks such as MOOSE provide rigorous engines for phase-field materials modeling, yet adoption is constrained by the expertise required to construct valid input files, coordinate parameter sweeps, diagnose failures, and extract quantitative results. We introduce AutoMOOSE, an open-source agentic framework that orchestrates the full simulation lifecycle from a single natural-language prompt. AutoMOOSE deploys a five-agent pipeline in which the Input Writer coordinates six sub-agents and the Reviewer autonomously corrects runtime failures without user intervention. A modular plugin architecture enables new phase-field formulations without modifying the core framework, and a Model Context Protocol (MCP) server exposes the workflow as ten structured tools for interoperability with any MCP-compatible client. Validated on a four-temperature copper grain growth benchmark, AutoMOOSE generates MOOSE input files with 6 of 12 structural blocks matching a human expert reference exactly and 4 functionally equivalent, executes all runs in parallel with a 1.8x speedup, and performs an end-to-end physical consistency check spanning intent, finite-element execution, and Arrhenius kinetics with no human verification. Grain coarsening kinetics are recovered with R^2 = 0.90-0.95 at T >= 600 K; the recovered activation energy Q_fit = 0.296 eV is consistent with a human-written reference (Q_fit = 0.267 eV) under identical parameters. Three runtime failure classes were diagnosed and resolved autonomously within a single correction cycle, and every run produces a provenance record satisfying FAIR data principles. These results show that the gap between knowing the physics and executing a validated simulation campaign can be bridged by a lightweight multi-agent orchestration layer, providing a pathway toward AI-driven materials discovery and self-driving laboratories.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.20986v1)
