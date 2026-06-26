---
type: source
source_type: arxiv
title: "MAGE: Multi-Agent Self-Evolution with Co-Evolutionary Knowledge Graphs"
authors: Ruiyi Yang, Zechen Li, Hao Xue, Imran Razzak et al.
url: https://arxiv.org/abs/2605.10064v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 15
primary: cs.AI
tags: [clinical-agents, computer-use-agents, embodied-agents, finance-agents, knowledge-graph, arxiv, auto-ingested]
---

# MAGE: Multi-Agent Self-Evolution with Co-Evolutionary Knowledge Graphs

**arXiv:** [2605.10064v1](https://arxiv.org/abs/2605.10064v1) · 2026-05-11 · cs.AI
**Authors:** Ruiyi Yang, Zechen Li, Hao Xue, Imran Razzak et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Self-evolving language-model agents must decide what to learn next and how to preserve what they have learned across iterations. Existing systems typically carry this cross-iteration knowledge as natural-language feedback, flat episodic memory, or implicit reinforcement signals, none of which cleanly supports a frozen weak backbone at inference time. This paper introduces MAGE (Multi-Agent Graph-guided Evolution), a framework that externalizes self-knowledge into a four-subgraph co-evolutionary knowledge graph. Its experience subgraph stores both teacher-written failure corrections and the learner's own past correct reasoning traces, which are retrieved as task-conditioned guidance for a frozen execution model. During evolution, the graph, a task-level search bandit, and a skill-level routing bandit are updated from the same reward stream, while the learner's backbone remains unchanged. We further provide structural analysis showing how append-only memory growth, bounded curriculum coverage, and task-filtered retrieval together support stable improvement of the retrieval substrate for frozen-learner evolution. Across nine benchmarks spanning mathematical reasoning, multi-hop and open-domain question answering, spatio-temporal analysis, financial numerical reasoning, medical multiple-choice, an open-world survival game, and web navigation, MAGE achieves strong performance against prompt-based frozen-backbone baselines. Ablations show that self-harvested success traces and teacher-written corrections are complementary, with success memories contributing most on reasoning-template-heavy tasks and corrective memories supporting harder composition and interaction settings.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10064v1)
