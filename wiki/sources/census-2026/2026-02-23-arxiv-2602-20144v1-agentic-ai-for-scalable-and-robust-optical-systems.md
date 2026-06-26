---
type: source
source_type: arxiv
title: "Agentic AI for Scalable and Robust Optical Systems Control"
authors: Zehao Wang, Mingzhe Han, Wei Cheng, Yue-Kai Huang et al.
url: https://arxiv.org/abs/2602.20144v1
date: 2026-02-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: eess.SY
tags: [coding-agents, agent-reliability, agent-protocols, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Agentic AI for Scalable and Robust Optical Systems Control

**arXiv:** [2602.20144v1](https://arxiv.org/abs/2602.20144v1) · 2026-02-23 · eess.SY
**Authors:** Zehao Wang, Mingzhe Han, Wei Cheng, Yue-Kai Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present AgentOptics, an agentic AI framework for high-fidelity, autonomous optical system control built on the Model Context Protocol (MCP). AgentOptics interprets natural language tasks and executes protocol-compliant actions on heterogeneous optical devices through a structured tool abstraction layer. We implement 64 standardized MCP tools across 8 representative optical devices and construct a 410-task benchmark to evaluate request understanding, role-aware responses, multi-step coordination, robustness to linguistic variation, and error handling. We assess two deployment configurations--commercial online LLMs and locally hosted open-source LLMs--and compare them with LLM-based code generation baselines. AgentOptics achieves 87.7%--99.0% average task success rates, significantly outperforming code-generation approaches, which reach up to 50% success. We further demonstrate broader applicability through five case studies extending beyond device-level control to system orchestration, monitoring, and closed-loop optimization. These include DWDM link provisioning and coordinated monitoring of coherent 400 GbE and analog radio-over-fiber (ARoF) channels; autonomous characterization and bias optimization of a wideband ARoF link carrying 5G fronthaul traffic; multi-span channel provisioning with launch power optimization; closed-loop fiber polarization stabilization; and distributed acoustic sensing (DAS)-based fiber monitoring with LLM-assisted event detection. These results establish AgentOptics as a scalable, robust paradigm for autonomous control and orchestration of heterogeneous optical systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.20144v1)
