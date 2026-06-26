---
type: source
source_type: arxiv
title: "From Business Events to Auditable Decisions: Ontology-Governed Graph Simulation for Enterprise AI"
authors: Hongyin Zhu, Jinming Liang, Mengjun Hou, Ruifan Tang et al.
url: https://arxiv.org/abs/2604.08603v1
date: 2026-04-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.AI
tags: [knowledge-graph, agent-skills, governance-gap, arxiv, auto-ingested]
---

# From Business Events to Auditable Decisions: Ontology-Governed Graph Simulation for Enterprise AI

**arXiv:** [2604.08603v1](https://arxiv.org/abs/2604.08603v1) · 2026-04-08 · cs.AI
**Authors:** Hongyin Zhu, Jinming Liang, Mengjun Hou, Ruifan Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing LLM-based agent systems share a common architectural failure: they answer from the unrestricted knowledge space without first simulating how active business scenarios reshape that space for the event at hand -- producing decisions that are fluent but ungrounded and carrying no audit trail. We present LOM-action, which equips enterprise AI with \emph{event-driven ontology simulation}: business events trigger scenario conditions encoded in the enterprise ontology~(EO), which drive deterministic graph mutations in an isolated sandbox, evolving a working copy of the subgraph into the scenario-valid simulation graph $G_{\text{sim}}$; all decisions are derived exclusively from this evolved graph. The core pipeline is \emph{event $\to$ simulation $\to$ decision}, realized through a dual-mode architecture -- \emph{skill mode} and \emph{reasoning mode}. Every decision produces a fully traceable audit log. LOM-action achieves 93.82% accuracy and 98.74% tool-chain F1 against frontier baselines Doubao-1.8 and DeepSeek-V3.2, which reach only 24--36% F1 despite 80% accuracy -- exposing the \emph{illusive accuracy} phenomenon. The four-fold F1 advantage confirms that ontology-governed, event-driven simulation, not model scale, is the architectural prerequisite for trustworthy enterprise decision intelligence.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-skills|Agent skills]] · [[governance-gap|Governance gap]]
- **Entities:** [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.08603v1)
