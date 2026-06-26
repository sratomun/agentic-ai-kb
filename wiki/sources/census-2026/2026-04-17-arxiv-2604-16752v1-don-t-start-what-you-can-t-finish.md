---
type: source
source_type: arxiv
title: "Don't Start What You Can't Finish: A Counterfactual Audit of Support-State Triage in LLM Agents"
authors: Eren Unlu
url: https://arxiv.org/abs/2604.16752v1
date: 2026-04-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agentic-rl, governance-gap, arxiv, auto-ingested]
---

# Don't Start What You Can't Finish: A Counterfactual Audit of Support-State Triage in LLM Agents

**arXiv:** [2604.16752v1](https://arxiv.org/abs/2604.16752v1) · 2026-04-17 · cs.AI
**Authors:** Eren Unlu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current agent evaluations largely reward execution on fully specified tasks, while recent work studies clarification [11, 22, 2], capability awareness [9, 1], abstention [8, 14], and search termination [20, 5] mostly in isolation. This leaves open whether agents can diagnose why a task is blocked before acting. We introduce the Support-State Triage Audit (SSTA-32), a matched-item diagnostic framework in which minimal counterfactual edits flip the same base request across four support states: Complete (ANSWER), Clarifiable (CLARIFY), Support-Blocked (REQUEST SUPPORT), and Unsupported-Now (ABSTAIN). We evaluate a frontier model under four prompting conditions - Direct, Action-Only, Confidence-Only, and a typed Preflight Support Check (PSC) - using Dual-Persona Auto-Auditing (DPAA) with deterministic heuristic scoring. Default execution overcommits heavily on non-complete tasks (41.7% overcommitment rate). Scalar confidence mapping avoids overcommitment but collapses the three-way deferral space (58.3% typed deferral accuracy). Conversely, both Action-Only and PSC achieve 91.7% typed deferral accuracy by surfacing the categorical ontology in the prompt. Targeted ablations confirm that removing the support-sufficiency dimension selectively degrades REQUEST SUPPORT accuracy, while removing the evidence-sufficiency dimension triggers systematic overcommitment on unsupported items. Because DPAA operates within a single context window, these results represent upper-bound capability estimates; nonetheless, the structural findings indicate that frontier models possess strong latent triage capabilities that require explicit categorical decision paths to activate safely.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.16752v1)
