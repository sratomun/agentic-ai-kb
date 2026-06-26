---
type: source
source_type: arxiv
title: "Mimosa Framework: Toward Evolving Multi-Agent Systems for Scientific Research"
authors: Martin Legrand, Tao Jiang, Matthieu Feraud, Benjamin Navet et al.
url: https://arxiv.org/abs/2603.28986v1
date: 2026-03-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 26
primary: cs.AI
tags: [agent-protocols, multi-agent-systems, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Mimosa Framework: Toward Evolving Multi-Agent Systems for Scientific Research

**arXiv:** [2603.28986v1](https://arxiv.org/abs/2603.28986v1) · 2026-03-30 · cs.AI
**Authors:** Martin Legrand, Tao Jiang, Matthieu Feraud, Benjamin Navet et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current Autonomous Scientific Research (ASR) systems, despite leveraging large language models (LLMs) and agentic architectures, remain constrained by fixed workflows and toolsets that prevent adaptation to evolving tasks and environments. We introduce Mimosa, an evolving multi-agent framework that automatically synthesizes task-specific multi-agent workflows and iteratively refines them through experimental feedback. Mimosa leverages the Model Context Protocol (MCP) for dynamic tool discovery, generates workflow topologies via a meta-orchestrator, executes subtasks through code-generating agents that invoke available tools and scientific software libraries, and scores executions with an LLM-based judge whose feedback drives workflow refinement. On ScienceAgentBench, Mimosa achieves a success rate of 43.1% with DeepSeek-V3.2, surpassing both single-agent baselines and static multi-agent configurations. Our results further reveal that models respond heterogeneously to multi-agent decomposition and iterative learning, indicating that the benefits of workflow evolution depend on the capabilities of the underlying execution model. Beyond these benchmarks, Mimosa modular architecture and tool-agnostic design make it readily extensible, and its fully logged execution traces and archived workflows support auditability by preserving every analytical step for inspection and potential replication. Combined with domain-expert guidance, the framework has the potential to automate a broad range of computationally accessible scientific tasks across disciplines. Released as a fully open-source platform, Mimosa aims to provide an open foundation for community-driven ASR.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Entities:** [[mcp]] · [[deepseek]] · [[agentbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.28986v1)
