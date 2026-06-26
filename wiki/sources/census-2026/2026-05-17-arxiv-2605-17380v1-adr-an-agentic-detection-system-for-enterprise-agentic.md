---
type: source
source_type: arxiv
title: "ADR: An Agentic Detection System for Enterprise Agentic AI Security"
authors: Chenning Li, Pan Hu, Justin Xu, Baris Ozbas et al.
url: https://arxiv.org/abs/2605.17380v1
date: 2026-05-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agent-reliability, agent-security, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# ADR: An Agentic Detection System for Enterprise Agentic AI Security

**arXiv:** [2605.17380v1](https://arxiv.org/abs/2605.17380v1) · 2026-05-17 · cs.AI
**Authors:** Chenning Li, Pan Hu, Justin Xu, Baris Ozbas et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present the Agentic AI Detection and Response (ADR) system, the first large-scale, production-proven enterprise framework for securing AI agents operating through the Model Context Protocol (MCP). We identify three persistent challenges in this domain: (1) limited observability -- existing Endpoint Detection and Response (EDR) tools see file writes but not the agent reasoning, prompts, or causal chains linking intent to execution; (2) insufficient robustness -- static defenses constrained by pre-defined rules fail to generalize across diverse attack techniques and enterprise contexts; and (3) high detection costs -- LLM-based inference is prohibitively expensive at scale. ADR addresses these challenges via three components: the ADR Sensor for high-fidelity agentic telemetry, the ADR Explorer for systematic pre-deployment red teaming and hard-example generation, and the ADR Detector for scalable, two-tier online detection combining fast triage with context-aware reasoning. Deployed at Uber for over ten months, ADR has sustained reliable detection in production with growing adoption reaching over 7,200 unique hosts and processing over 10,000 agent sessions daily, uncovering hundreds of credential exposures across 26 categories and enabling a shift-left prevention layer (97.2% precision, 206 detected credentials). To validate the approach and enable community adoption, we introduce ADR-Bench (302 tasks, 17 techniques, 133 MCP servers), where ADR achieves zero false positives while detecting 67% of attacks -- outperforming three state-of-the-art baselines (ALRPHFS, GuardAgent, LlamaFirewall) by 2--4x in F1-score. On AgentDojo (public prompt injection benchmark), ADR detects all attacks with only three false alarms out of 93 tasks.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[llama]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.17380v1)
