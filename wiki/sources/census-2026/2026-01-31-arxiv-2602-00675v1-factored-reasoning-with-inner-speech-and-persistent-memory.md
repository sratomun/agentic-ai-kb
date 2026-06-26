---
type: source
source_type: arxiv
title: "Factored Reasoning with Inner Speech and Persistent Memory for Evidence-Grounded Human-Robot Interaction"
authors: Valerio Belcamino, Mariya Kilina, Alessandro Carfì, Valeria Seidita et al.
url: https://arxiv.org/abs/2602.00675v1
date: 2026-01-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.RO
tags: [embodied-agents, knowledge-graph, agent-memory, governance-gap, arxiv, auto-ingested]
---

# Factored Reasoning with Inner Speech and Persistent Memory for Evidence-Grounded Human-Robot Interaction

**arXiv:** [2602.00675v1](https://arxiv.org/abs/2602.00675v1) · 2026-01-31 · cs.RO
**Authors:** Valerio Belcamino, Mariya Kilina, Alessandro Carfì, Valeria Seidita et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Dialogue-based human-robot interaction requires robot cognitive assistants to maintain persistent user context, recover from underspecified requests, and ground responses in external evidence, while keeping intermediate decisions verifiable. In this paper we introduce JANUS, a cognitive architecture for assistive robots that models interaction as a partially observable Markov decision process and realizes control as a factored controller with typed interfaces. To this aim, Janus (i) decomposes the overall behavior into specialized modules, related to scope detection, intent recognition, memory, inner speech, query generation, and outer speech, and (ii) exposes explicit policies for information sufficiency, execution readiness, and tool grounding. A dedicated memory agent maintains a bounded recent-history buffer, a compact core memory, and an archival store with semantic retrieval, coupled through controlled consolidation and revision policies. Models inspired by the notion of inner speech in cognitive theories provide a control-oriented internal textual flow that validates parameter completeness and triggers clarification before grounding, while a faithfulness constraint ties robot-to-human claims to an evidence bundle combining working context and retrieved tool outputs. We evaluate JANUS through module-level unit tests in a dietary assistance domain grounded on a knowledge graph, reporting high agreement with curated references and practical latency profiles. These results support factored reasoning as a promising path to scalable, auditable, and evidence-grounded robot assistance over extended interaction horizons.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.00675v1)
