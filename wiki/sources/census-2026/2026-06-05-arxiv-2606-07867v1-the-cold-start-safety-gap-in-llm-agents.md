---
type: source
source_type: arxiv
title: "The Cold-Start Safety Gap in LLM Agents"
authors: Chung-En Sun, Linbo Liu, Tsui-Wei Weng
url: https://arxiv.org/abs/2606.07867v1
date: 2026-06-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [recommendation-agents, agent-security, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# The Cold-Start Safety Gap in LLM Agents

**arXiv:** [2606.07867v1](https://arxiv.org/abs/2606.07867v1) · 2026-06-05 · cs.CL
**Authors:** Chung-En Sun, Linbo Liu, Tsui-Wei Weng

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Are tool-calling LLM agents equally safe throughout a conversation? We discover they are not: agents are most vulnerable at the very start of a session and become substantially safer after a few regular agentic tasks -- a phenomenon we term the cold-start safety gap. To study this systematically, we introduce Safety Over Depth for Agents (SODA), a benchmark that controls how many regular agentic tasks the agent completes before encountering a safety threat, supporting up to 20 preceding tasks. Evaluating 7 models from 4 families, safety improves by 9--52% as the number of preceding regular agentic tasks increases from zero to twenty. Representation analysis confirms that model hidden states gradually shift toward a safety-aligned region as more preceding tasks are present. By systematically studying which part of the preceding conversation matters most, we find that the regular agentic tasks themselves are the primary driver of safety, while the agent's own prior responses have less effect on safety but are essential for preserving later utility. This conclusion is further supported by evaluation on open-source safety benchmarks (AgentHarm, Agent Safety Bench) and utility benchmarks (BFCL, API-Bank), confirming that warming up the agent with regular agentic tasks before deployment makes it safer and preserves full capability. Based on these findings, we recommend a simple deployment strategy: having the agent complete a few regular agentic tasks before possible exposure to safety-critical requests mitigates the cold-start safety gap. Our code is available at https://github.com/Trustworthy-ML-Lab/Agent-Cold-Start-Safety-Gap

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.07867v1)
