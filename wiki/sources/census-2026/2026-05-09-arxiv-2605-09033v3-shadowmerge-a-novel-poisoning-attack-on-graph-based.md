---
type: source
source_type: arxiv
title: "ShadowMerge: A Novel Poisoning Attack on Graph-Based Agent Memory via Relation-Channel Conflicts"
authors: Yang Luo, Zifeng Kang, Tiantian Ji, Xinran Liu et al.
url: https://arxiv.org/abs/2605.09033v3
date: 2026-05-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.CR
tags: [knowledge-graph, agent-security, agent-memory, arxiv, auto-ingested]
---

# ShadowMerge: A Novel Poisoning Attack on Graph-Based Agent Memory via Relation-Channel Conflicts

**arXiv:** [2605.09033v3](https://arxiv.org/abs/2605.09033v3) · 2026-05-09 · cs.CR
**Authors:** Yang Luo, Zifeng Kang, Tiantian Ji, Xinran Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph-based agent memory is increasingly used in LLM agents to support structured long-term recall and multi-hop reasoning, but it also creates a new poisoning surface: an attacker can inject a crafted relation into graph memory so that it is later retrieved and influences agent behavior. Existing agent-memory poisoning attacks mainly target flat textual records and are ineffective in graph-based memory because malicious relations often fail to be extracted, merged into the target anchor neighborhood, or retrieved for the victim query. We present SHADOWMERGE, a poisoning attack against graph-based agent memory that exploits relation-channel conflicts. Its key insight is that a poisoned relation can share the same query-activated anchor and canonicalized relation channel as benign evidence while carrying a conflicting value. To realize this, we design AIR, a pipeline that converts the conflict into an ordinary interaction that can be extracted, merged, and retrieved by the graph-memory system. We evaluate SHADOWMERGE on Mem0 and three public real-world datasets: PubMedQA, WebShop, and ToolEmu. SHADOWMERGE achieves 93.8% average attack success rate, improving the best baseline by 50.3 absolute points, while having negligible impact on unrelated benign tasks. Mechanism studies show that SHADOWMERGE overcomes the three key limitations of existing agent-memory poisoning attacks, and defense analysis shows that representative input-side defenses are insufficient to mitigate it. We have responsibly disclosed our findings to affected graph-memory vendors and open sourced SHADOWMERGE.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.09033v3)
