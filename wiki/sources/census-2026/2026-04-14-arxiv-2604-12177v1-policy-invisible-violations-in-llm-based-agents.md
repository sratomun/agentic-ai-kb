---
type: source
source_type: arxiv
title: "Policy-Invisible Violations in LLM-Based Agents"
authors: Jie Wu, Ming Gong
url: https://arxiv.org/abs/2604.12177v1
date: 2026-04-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.AI
tags: [knowledge-graph, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Policy-Invisible Violations in LLM-Based Agents

**arXiv:** [2604.12177v1](https://arxiv.org/abs/2604.12177v1) · 2026-04-14 · cs.AI
**Authors:** Jie Wu, Ming Gong

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based agents can execute actions that are syntactically valid, user-sanctioned, and semantically appropriate, yet still violate organizational policy because the facts needed for correct policy judgment are hidden at decision time. We call this failure mode policy-invisible violations: cases in which compliance depends on entity attributes, contextual state, or session history absent from the agent's visible context. We present PhantomPolicy, a benchmark spanning eight violation categories with balanced violation and safe-control cases, in which all tool responses contain clean business data without policy metadata. We manually review all 600 model traces produced by five frontier models and evaluate them using human-reviewed trace labels. Manual review changes 32 labels (5.3%) relative to the original case-level annotations, confirming the need for trace-level human review. To demonstrate what world-state-grounded enforcement can achieve under favorable conditions, we introduce Sentinel, an enforcement framework based on counterfactual graph simulation. Sentinel treats every agent action as a proposed mutation to an organizational knowledge graph, performs speculative execution to materialize the post-action world state, and verifies graph-structural invariants to decide Allow/Block/Clarify. Against human-reviewed trace labels, Sentinel substantially outperforms a content-only DLP baseline (68.8% vs. 93.0% accuracy) while maintaining high precision, though it still leaves room for improvement on certain violation categories. These results demonstrate what becomes achievable once policy-relevant world state is made available to the enforcement layer.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.12177v1)
