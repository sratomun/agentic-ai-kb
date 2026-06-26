---
type: source
source_type: arxiv
title: "AgentSkiller: Scaling Generalist Agent Intelligence through Semantically Integrated Cross-Domain Data Synthesis"
authors: Zexu Sun, Bokai Ji, Hengyi Cai, Shuaiqiang Wang et al.
url: https://arxiv.org/abs/2602.09372v1
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.CL
tags: [knowledge-graph, agent-reliability, agent-protocols, agent-memory, tool-use, arxiv, auto-ingested]
---

# AgentSkiller: Scaling Generalist Agent Intelligence through Semantically Integrated Cross-Domain Data Synthesis

**arXiv:** [2602.09372v1](https://arxiv.org/abs/2602.09372v1) · 2026-02-10 · cs.CL
**Authors:** Zexu Sun, Bokai Ji, Hengyi Cai, Shuaiqiang Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model agents demonstrate potential in solving real-world problems via tools, yet generalist intelligence is bottlenecked by scarce high-quality, long-horizon data. Existing methods collect privacy-constrained API logs or generate scripted interactions lacking diversity, which struggle to produce data requisite for scaling capabilities. We propose AgentSkiller, a fully automated framework synthesizing multi-turn interaction data across realistic, semantically linked domains. It employs a DAG-based architecture with explicit state transitions to ensure determinism and recoverability. The pipeline builds a domain ontology and Person-Centric Entity Graph, defines tool interfaces via Service Blueprints for Model Context Protocol servers, and populates environments with consistent databases and strict Domain Policies. A cross-domain fusion mechanism links services to simulate complex tasks. Finally, the pipeline creates user tasks by verifying solution paths, filtering via execution-based validation, and generating queries using a Persona-based Simulator for automated rollout. This produces reliable environments with clear state changes. To demonstrate effectiveness, we synthesized $\approx$ 11K interaction samples; experimental results indicate that models trained on this dataset achieve significant improvements on function calling over baselines, particularly in larger parameter regimes.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.09372v1)
