---
type: source
source_type: arxiv
title: "Mozi: Governed Autonomy for Drug Discovery LLM Agents"
authors: He Cao, Siyu Liu, Fan Zhang, Zijing Liu et al.
url: https://arxiv.org/abs/2603.03655v1
date: 2026-03-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [science-agents, human-agent-interaction, agent-reliability, agent-skills, agent-memory, arxiv, auto-ingested]
---

# Mozi: Governed Autonomy for Drug Discovery LLM Agents

**arXiv:** [2603.03655v1](https://arxiv.org/abs/2603.03655v1) · 2026-03-04 · cs.AI
**Authors:** He Cao, Siyu Liu, Fan Zhang, Zijing Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-augmented large language model (LLM) agents promise to unify scientific reasoning with computation, yet their deployment in high-stakes domains like drug discovery is bottlenecked by two critical barriers: unconstrained tool-use governance and poor long-horizon reliability. In dependency-heavy pharmaceutical pipelines, autonomous agents often drift into irreproducible trajectories, where early-stage hallucinations multiplicatively compound into downstream failures. To overcome this, we present Mozi, a dual-layer architecture that bridges the flexibility of generative AI with the deterministic rigor of computational biology. Layer A (Control Plane) establishes a governed supervisor--worker hierarchy that enforces role-based tool isolation, limits execution to constrained action spaces, and drives reflection-based replanning. Layer B (Workflow Plane) operationalizes canonical drug discovery stages -- from Target Identification to Lead Optimization -- as stateful, composable skill graphs. This layer integrates strict data contracts and strategic human-in-the-loop (HITL) checkpoints to safeguard scientific validity at high-uncertainty decision boundaries. Operating on the design principle of ``free-form reasoning for safe tasks, structured execution for long-horizon pipelines,'' Mozi provides built-in robustness mechanisms and trace-level audibility to completely mitigate error accumulation. We evaluate Mozi on PharmaBench, a curated benchmark for biomedical agents, demonstrating superior orchestration accuracy over existing baselines. Furthermore, through end-to-end therapeutic case studies, we demonstrate Mozi's ability to navigate massive chemical spaces, enforce stringent toxicity filters, and generate highly competitive in silico candidates, effectively transforming the LLM from a fragile conversationalist into a reliable, governed co-scientist.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.03655v1)
