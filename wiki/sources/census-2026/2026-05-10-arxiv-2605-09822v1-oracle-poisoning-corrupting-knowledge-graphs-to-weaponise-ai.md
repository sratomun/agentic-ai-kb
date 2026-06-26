---
type: source
source_type: arxiv
title: "Oracle Poisoning: Corrupting Knowledge Graphs to Weaponise AI Agent Reasoning"
authors: Ben Kereopa-Yorke, Guillermo Diaz, Holly Wright, Reagan Johnston et al.
url: https://arxiv.org/abs/2605.09822v1
date: 2026-05-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CR
tags: [knowledge-graph, agent-security, agent-skills, tool-use, arxiv, auto-ingested]
---

# Oracle Poisoning: Corrupting Knowledge Graphs to Weaponise AI Agent Reasoning

**arXiv:** [2605.09822v1](https://arxiv.org/abs/2605.09822v1) · 2026-05-10 · cs.CR
**Authors:** Ben Kereopa-Yorke, Guillermo Diaz, Holly Wright, Reagan Johnston et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We define Oracle Poisoning, an attack class in which an adversary corrupts a structured knowledge graph that AI agents query at runtime via tool-use protocols, causing incorrect conclusions through correct reasoning. Unlike prompt injection, Oracle Poisoning manipulates the data agents reason over, not their instructions. We demonstrate six attack scenarios against a production 42-million-node code knowledge graph, providing the first empirical demonstration of knowledge graph poisoning against a production-scale agentic system, distinct from CTI embedding poisoning. Primary evaluation uses real SDK tool-use across nine models from three providers (N=30 per model), where models autonomously invoke a graph query tool and reason from results. The result is unambiguous: every tested model trusts poisoned data at 100% at moderate attacker sophistication(L2), with 269 valid trials (of 270) accepting fabricated security claims under directed queries. Under open-ended prompts, trust drops to 3-55%, confirming prompt framing as a confound; we report both conditions. An attacker sophistication gradient reveals discrete break points, a minimum skill at which trust flips from 0% to 100%, reframing the attack as a question not of whether but of how much. A controlled delivery-mode comparison shows that inline evaluation produces false negatives: GPT-5.1 shows 0% trust inline but 100% under both simulated and real agentic tool-use, demonstrating that delivery mode is a first-order confound. We evaluate five defences; read-only access control eliminates the direct mutation vector, while the remaining four are partial and model-dependent. Analysis of four additional platforms suggests the attack may generalise across the knowledge-graph ecosystem.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-skills|Agent skills]] · [[tool-use|Tool use]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.09822v1)
