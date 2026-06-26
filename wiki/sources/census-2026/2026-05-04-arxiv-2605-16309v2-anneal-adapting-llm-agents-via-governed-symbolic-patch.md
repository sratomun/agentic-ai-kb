---
type: source
source_type: arxiv
title: "ANNEAL: Adapting LLM Agents via Governed Symbolic Patch Learning"
authors: Safayat Bin Hakim, Keyan Guo, Wenkai Tan, Alvaro Velasquez et al.
url: https://arxiv.org/abs/2605.16309v2
date: 2026-05-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [knowledge-graph, agent-reliability, self-evolving-agents, agent-memory, governance-gap, arxiv, auto-ingested]
---

# ANNEAL: Adapting LLM Agents via Governed Symbolic Patch Learning

**arXiv:** [2605.16309v2](https://arxiv.org/abs/2605.16309v2) · 2026-05-04 · cs.AI
**Authors:** Safayat Bin Hakim, Keyan Guo, Wenkai Tan, Alvaro Velasquez et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based agents can recover from individual execution errors, yet they repeatedly fail on the same fault when the underlying process knowledge--operator schemas, preconditions, and constraints--remains unrepaired. Existing self-evolving approaches address this gap by updating prompts, memory, or model weights, but none directly repair the symbolic structures that encode how tasks are executed, and few provide the governance guarantees required for safe deployment. We introduce ANNEAL, a neuro-symbolic agent that converts recurring failures into governed symbolic edits of a process knowledge graph without modifying foundation model weights. Its core mechanism, Failure-Driven Knowledge Acquisition (FDKA), localizes the responsible operator, synthesizes a typed patch through constrained LLM generation, and validates the proposal via multi-dimensional scoring, symbolic guardrails, and canary testing before commit. Every accepted edit carries full provenance and deterministic rollback capability. Across four domains and 27 multi-seed runs, ANNEAL is the only evaluated system that commits persistent structural repairs--strong baselines such as ReAct and Reflexion achieve high episodic recovery yet retain 72--100% holdout failure rates on recurring faults, whereas ANNEAL reduces these to 0% in the tested recurring-failure settings. Ablation confirms that removing FDKA eliminates all structural repairs and drops success rate by up to 26.7 percentage points. These results suggest that governed symbolic repair offers a complementary paradigm to weight-level and prompt-level adaptation for persistent fault elimination.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16309v2)
