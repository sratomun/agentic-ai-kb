---
type: source
source_type: arxiv
title: "The Auton Agentic AI Framework"
authors: Sheng Cao, Zhao Chang, Chang Li, Hannan Li et al.
url: https://arxiv.org/abs/2602.23720v1
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agentic-rl, agent-security, agent-protocols, agent-memory, governance-gap, arxiv, auto-ingested]
---

# The Auton Agentic AI Framework

**arXiv:** [2602.23720v1](https://arxiv.org/abs/2602.23720v1) · 2026-02-27 · cs.AI
**Authors:** Sheng Cao, Zhao Chang, Chang Li, Hannan Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The field of Artificial Intelligence is undergoing a transition from Generative AI -- probabilistic generation of text and images -- to Agentic AI, in which autonomous systems execute actions within external environments on behalf of users. This transition exposes a fundamental architectural mismatch: Large Language Models (LLMs) produce stochastic, unstructured outputs, whereas the backend infrastructure they must control -- databases, APIs, cloud services -- requires deterministic, schema-conformant inputs. The present paper describes the Auton Agentic AI Framework, a principled architecture for standardizing the creation, execution, and governance of autonomous agent systems. The framework is organized around a strict separation between the Cognitive Blueprint, a declarative, language-agnostic specification of agent identity and capabilities, and the Runtime Engine, the platform-specific execution substrate that instantiates and runs the agent. This separation enables cross-language portability, formal auditability, and modular tool integration via the Model Context Protocol (MCP). The paper formalizes the agent execution model as an augmented Partially Observable Markov Decision Process (POMDP) with a latent reasoning space, introduces a hierarchical memory consolidation architecture inspired by biological episodic memory systems, defines a constraint manifold formalism for safety enforcement via policy projection rather than post-hoc filtering, presents a three-level self-evolution framework spanning in-context adaptation through reinforcement learning, and describes runtime optimizations -- including parallel graph execution, speculative inference, and dynamic context pruning -- that reduce end-to-end latency for multi-step agent workflows.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[governance-gap|Governance gap]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23720v1)
