---
type: source
source_type: arxiv
title: "Decoupled Intelligence: A Multi-Agent LLM Framework for Controllable Traffic Scenario Generation in SUMO"
authors: Shuyang Li, Ruimin Ke
url: https://arxiv.org/abs/2605.27685v1
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 25
primary: cs.MA
tags: [autonomous-driving-agents, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# Decoupled Intelligence: A Multi-Agent LLM Framework for Controllable Traffic Scenario Generation in SUMO

**arXiv:** [2605.27685v1](https://arxiv.org/abs/2605.27685v1) · 2026-05-26 · cs.MA
**Authors:** Shuyang Li, Ruimin Ke

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The integration of Large Language Models (LLMs) with microscopic traffic simulation offers a promising path toward autonomous urban planning and intelligent transportation analysis. However, existing monolithic agent architectures often struggle with the complexity of end-to-end simulation workflows, leading to reasoning failures, parameter inconsistency, and a lack of systematic state management. This paper proposes a novel multi-agent collaborative framework designed to automate the entire lifecycle of traffic simulation in SUMO (Simulation of Urban Mobility). Our approach decouples the simulation pipeline into specialized roles, including Planner, Builder, Demand, Runner, and Analyst, coordinated by a high-level reasoning engine. We introduce a state-persistent Orchestrator leveraging the Model Context Protocol (MCP) to ensure seamless data handover and environmental consistency across distributed agent actions. This architecture enables a robust closed-loop refinement process, where simulation outcomes are iteratively analyzed and optimized to satisfy user-defined Key Performance Indicators (KPIs). Experimental results through role ablation studies demonstrate that the proposed multi-agent framework significantly enhances task success rates and parameter accuracy compared to single-agent baselines. Furthermore, case studies on real-world network extraction and traffic optimization highlight the system's capability to bridge the gap between high-level natural language intent and low-level simulation execution.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27685v1)
