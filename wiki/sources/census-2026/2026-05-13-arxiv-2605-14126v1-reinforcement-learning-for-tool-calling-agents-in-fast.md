---
type: source
source_type: arxiv
title: "Reinforcement Learning for Tool-Calling Agents in Fast Healthcare Interoperability Resources (FHIR)"
authors: Marius S. Knorr, Robert Müller, Jan P. Bremer, Nils Schweingruber
url: https://arxiv.org/abs/2605.14126v1
date: 2026-05-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.LG
tags: [clinical-agents, agent-reliability, agentic-rl, agent-protocols, tool-use, arxiv, auto-ingested]
---

# Reinforcement Learning for Tool-Calling Agents in Fast Healthcare Interoperability Resources (FHIR)

**arXiv:** [2605.14126v1](https://arxiv.org/abs/2605.14126v1) · 2026-05-13 · cs.LG
**Authors:** Marius S. Knorr, Robert Müller, Jan P. Bremer, Nils Schweingruber

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Fast Healthcare Interoperability Resources (FHIR) is the dominant standard for interoperable exchange of healthcare data. In FHIR, electronic health records form a directed graph of resources. Answering clinically meaningful questions over FHIR requires agents to perform multi-step reasoning, filtering, and aggregation across multiple resource types. Prior work shows that even tool-augmented LLM agents (retrieval, code execution, multi-turn planning) often select the wrong resources or violate traversal constraints. We study this problem in the context of FHIR-AgentBench, a benchmark for realistic question answering over real-world hospital data, and frame reasoning on FHIR as a sequential decision-making problem over a queryable structured graph. We implement a multi-turn CodeAct agent and post-train it with reinforcement learning using a custom harness and tools. A LLM Judge provides execution-grounded rewards. Compared to prompt-based, closed-model baselines, RL post-training improves performance while enforcing data-integrity constraints. Empirically, our approach improves answer correctness from 50% (o4-mini) to 77% on FHIR-AgentBench using a smaller and cheaper Qwen3-8B model. We present an end-to-end post-training pipeline (environment building, harness construction, model training and custom evaluation) that reliably improves multi-turn reasoning over structured clinical graphs.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]] · [[agentbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14126v1)
