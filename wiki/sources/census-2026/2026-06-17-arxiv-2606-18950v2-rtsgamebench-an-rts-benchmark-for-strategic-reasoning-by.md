---
type: source
source_type: arxiv
title: "RTSGameBench: An RTS Benchmark for Strategic Reasoning by Vision-Language Models"
authors: San Kim, Daechul Ahn, Reokyoung Kim, Hyeonbeom Choi et al.
url: https://arxiv.org/abs/2606.18950v2
date: 2026-06-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, agent-reliability, self-evolving-agents, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# RTSGameBench: An RTS Benchmark for Strategic Reasoning by Vision-Language Models

**arXiv:** [2606.18950v2](https://arxiv.org/abs/2606.18950v2) · 2026-06-17 · cs.AI
**Authors:** San Kim, Daechul Ahn, Reokyoung Kim, Hyeonbeom Choi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern Vision-Language Models (VLMs) often struggle with strategic reasoning, i.e., anticipating and influencing other agents' actions, under uncertainty in competitive and cooperative settings. Real-time strategy (RTS) games can be a natural testbed for diagnosing this limitation, as they demand coordination with allies, adaptation to opponents' strategy, and long-horizon planning under partial observability. However, existing RTS benchmarks offer limited evaluation scope, lack systematic competency diagnosis, and remain fixed in the pre-designed scenario coverage. To address these limitations, we present RTSGameBench, which is built on Beyond All Reason, a large-scale RTS game with an expanded battlefield that demands broader strategy diversity than the existing testbeds. The proposed benchmark provides evaluations through diverse gameplay across various matchup structures, diagnostic assessment via mini-games, each targeting an individual strategic competency, and extensible coverage via a self-evolving generation framework that converts free-form queries into new mini-games, improving over successive cycles. Additionally, for VLMs to operate in large-scale RTS games, we provide RTSGameAgent that manages units by an FSM with agentic memory. We empirically validate that multiple state-of-the-art VLMs do not perform well when matchups demand tighter coordination, multiagent coordination and when task scale increases.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.18950v2)
