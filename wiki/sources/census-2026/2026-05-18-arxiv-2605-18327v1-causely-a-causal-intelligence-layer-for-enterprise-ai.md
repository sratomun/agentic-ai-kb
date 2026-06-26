---
type: source
source_type: arxiv
title: "Causely: A Causal Intelligence Layer for Enterprise AI A Benchmark Study on SRE and Reliability Workflows"
authors: Dhairya Dalal, Endre Sara, Ben Yemini, Christine Miller et al.
url: https://arxiv.org/abs/2605.18327v1
date: 2026-05-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-reliability, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Causely: A Causal Intelligence Layer for Enterprise AI A Benchmark Study on SRE and Reliability Workflows

**arXiv:** [2605.18327v1](https://arxiv.org/abs/2605.18327v1) · 2026-05-18 · cs.AI
**Authors:** Dhairya Dalal, Endre Sara, Ben Yemini, Christine Miller et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
AI agents deployed into SRE workflows currently derive their understanding of environment state from raw observability telemetry at query time, paying a semantic-interpretation tax in tokens, latency, and inferential reliability. We propose Causely, a causal intelligence layer that maintains a structured representation of environment topology, attribute dependencies, and causal relationships that are anchroed to a ontological representation of the managed environment. Causely transforms raw telemetry into a live, queryable model providing the semantic and causal foundation AI agents require to diagnose, evaluate impact, and act safely in production. We evaluate this value proposition through a benchmark study conducted in a controlled setting with injected faults in a 24-microservice OpenTelemetry demo application. Our experiments compare four agent configurations (Claude Code, OpenAI Codex, HolmesGPT with Sonnet and Gemini backends). Experiments are run with and without access to Causely under two scenarios: an active incident and a healthy baseline. On the active-fault scenario, causal grounding reduces mean time-to-diagnosis by 63\%, mean token consumption by 60\%, and mean tool-call count by 78\%, compressing the investigation footprint by 4.8$\times$ and lowering direct API cost per run by 57\%; root-cause-diagnosis accuracy rises from 75\% to 100\%.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.18327v1)
