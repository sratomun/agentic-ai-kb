---
type: source
source_type: arxiv
title: "LanG -- A Governance-Aware Agentic AI Platform for Unified Security Operations"
authors: Anes Abdennebi, Nadjia Kara, Laaziz Lahlou, Hakima Ould-Slimane
url: https://arxiv.org/abs/2604.05440v1
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CR
tags: [science-agents, human-agent-interaction, agent-security, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# LanG -- A Governance-Aware Agentic AI Platform for Unified Security Operations

**arXiv:** [2604.05440v1](https://arxiv.org/abs/2604.05440v1) · 2026-04-07 · cs.CR
**Authors:** Anes Abdennebi, Nadjia Kara, Laaziz Lahlou, Hakima Ould-Slimane

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern Security Operations Centers struggle with alert fatigue, fragmented tooling, and limited cross-source event correlation. Challenges that current Security Information Event Management and Extended Detection and Response systems only partially address through fragmented tools. This paper presents the LLM-assisted network Governance (LanG), an open-source, governance-aware agentic AI platform for unified security operations contributing: (i) a Unified Incident Context Record with a correlation engine (F1 = 87%), (ii) an Agentic AI Orchestrator on LangGraph with human-in-the-loop checkpoints, (iii) an LLM-based Rule Generator finetuned on four base models producing deployable Snort 2/3, Suricata, and YARA rules (average acceptance rate 96.2%), (iv) a Three-Phase Attack Reconstructor combining Louvain community detection, LLM-driven hypothesis generation, and Bayesian scoring (87.5% kill-chain accuracy), and (v) a layered Governance-MCP-Agentic AI-Security architecture where all tools are exposed via the Model Context Protocol, governed by an AI Governance Policy Engine with a two-layer guardrail pipeline (regex + Llama Prompt Guard 2 semantic classifier, achieving 98.1% F1 score with experimental zero false positives). Designed for Managed Security Service Providers, the platform supports multi-tenant isolation, role-based access, and fully local deployment. Finetuned anomaly and threat detectors achieve weighted F1 scores of 99.0% and 91.0%, respectively, in intrusion-detection benchmarks, running inferences in $\approx$21 ms with a machine-side mean time to detect of 1.58 s, and the rule generator exceeds 91% deployability on live IDS engines. A systematic comparison against eight SOC platforms confirms that LanG uniquely satisfies multiple industrial capabilities all in one open-source tool, while enforcing selected AI governance policies.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]] · [[llama]] · [[langgraph]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05440v1)
