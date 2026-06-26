---
type: source
source_type: arxiv
title: "HypoAgent: An Agentic Framework for Interactive Abductive Hypothesis Generation over Knowledge Graphs"
authors: Yisen Gao, Yixi Cai, Tianshi Zheng, Jiaxin Bai et al.
url: https://arxiv.org/abs/2605.31370v1
date: 2026-05-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [clinical-agents, science-agents, knowledge-graph, agent-reliability, arxiv, auto-ingested]
---

# HypoAgent: An Agentic Framework for Interactive Abductive Hypothesis Generation over Knowledge Graphs

**arXiv:** [2605.31370v1](https://arxiv.org/abs/2605.31370v1) · 2026-05-29 · cs.AI
**Authors:** Yisen Gao, Yixi Cai, Tianshi Zheng, Jiaxin Bai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Abductive reasoning over knowledge graphs aims to generate logical hypotheses that explain observed entities or facts. Existing controllable hypothesis generation methods allow users to guide this process with explicit conditions, but they remain limited in interactive settings: they struggle to ground evolving natural-language intents across multi-turn dialogues and provide little fine-grained diagnosis when generated hypotheses fail. To address these limitations, we propose HypoAgent, an Agentic framework for interactive abductive Hypothesis Generation over knowledge graphs. HypoAgent integrates three agents: an Intent Recognition Agent that grounds user utterances and dialogue history into executable KG conditions, a Hypothesis Generation Agent that performs controllable hypothesis generation according to the extracted user intention, and a Root Cause Analysis Agent that diagnoses unreliable hypothesis fragments and leverages KG neighborhood probing to identify supported refinements. Experiments on commonsense and biomedical domain-specific knowledge graphs demonstrate that HypoAgent achieves state-of-the-art semantic similarity under single-turn, multi-turn, and unconditional settings. Our code is available at https://github.com/HKUST-KnowComp/HypoAgent.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.31370v1)
