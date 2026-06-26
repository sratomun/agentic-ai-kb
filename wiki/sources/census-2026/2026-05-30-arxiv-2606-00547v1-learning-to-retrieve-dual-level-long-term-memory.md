---
type: source
source_type: arxiv
title: "Learning to Retrieve: Dual-Level Long-Term Memory for Text-to-SQL Agents"
authors: Yibo Wang, Nikki Lijing Kuang, Philip S. Yu, Zhewei Yao et al.
url: https://arxiv.org/abs/2606.00547v1
date: 2026-05-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.CL
tags: [data-query-agents, agentic-rl, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Learning to Retrieve: Dual-Level Long-Term Memory for Text-to-SQL Agents

**arXiv:** [2606.00547v1](https://arxiv.org/abs/2606.00547v1) · 2026-05-30 · cs.CL
**Authors:** Yibo Wang, Nikki Lijing Kuang, Philip S. Yu, Zhewei Yao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Interactive text-to-SQL agents solve database tasks through multi-turn interactions involving schema exploration, query execution, feedback interpretation, and decision revision. Long-term memory helps agents reuse past experiences, but existing retrieval methods remain limited. Static methods rely on fixed similarity heuristics that do not optimize downstream utility, while dynamic methods often learn from sparse final outcomes and retrieve memories at a single decision horizon. This is insufficient when memory usefulness changes across interaction stages, since memories useful for initial planning may differ from those needed for local, state-conditioned execution. We propose MERIT, a dynamic multi-horizon memory retrieval framework. MERIT maintains episode-level memory for global strategic guidance and turn-level memory for local decision support. Both levels use learned retrieval policies optimized with reinforcement learning. To train turn-level retrieval despite limited intermediate supervision, MERIT uses a lightweight Process Reward Model to provide dense proxy rewards for local memory selection. Experiments on BIRD-Interact show that MERIT outperforms no-memory, static-retrieval, and dynamic-retrieval baselines in success rate while reducing average interaction turns. Transfer results on Spider2-Snow further show positive cross-benchmark transfer without benchmark-specific tuning. These results suggest that multi-horizon retrieval improves experience reuse in interactive text-to-SQL agents.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.00547v1)
