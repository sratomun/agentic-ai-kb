---
type: source
source_type: arxiv
title: "SafeMCP: Proactive Power Regulation for LLM Agent Defense via Environment-Grounded Look-Ahead Reasoning"
authors: Lichao Wang, Zhaoxing Ren, Tianzhuo Yang, Jiaming Ji et al.
url: https://arxiv.org/abs/2606.01991v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agentic-rl, agent-security, agent-protocols, arxiv, auto-ingested]
---

# SafeMCP: Proactive Power Regulation for LLM Agent Defense via Environment-Grounded Look-Ahead Reasoning

**arXiv:** [2606.01991v1](https://arxiv.org/abs/2606.01991v1) · 2026-06-01 · cs.AI
**Authors:** Lichao Wang, Zhaoxing Ren, Tianzhuo Yang, Jiaming Ji et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As Large Language Model (LLM) agents increasingly leverage the Model Context Protocol (MCP) to operate in complex environments, the expansion of their action spaces offers agents unsafe capabilities and underscores the risk of power-seeking. While broad action space and greater environment influence are essential for task fulfillment, they create a fragile risk surface where minor errors or hallucinations are magnified into catastrophic failures. In response, we propose SafeMCP, a {server-side} defense plugin that constrains tool acquisition via predictive reasoning regarding future safety risks. SafeMCP utilizes an internal world model for look-ahead reasoning to implement a two-tier defense: proactive tool filtering to constrain hazardous power expansion and immediate intervention as a fail-safe. To train SafeMCP, we introduce a three-stage pipeline comprising environmental dynamic grounding, safe policy initialization, and reinforcement learning (RL) with dual verifiable rewards. Experiments on PowerSeeking Bench, ToolEmu, and AgentHarm show that SafeMCP achieves a safe equilibrium, effectively mitigating risks while preserving agent utility.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01991v1)
