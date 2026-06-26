---
type: source
source_type: arxiv
title: "Peak-Then-Collapse and the Four Interface Channels of Knowledge-Graph Tool Use"
authors: Tianda Sun, Dimitar Kazakov
url: https://arxiv.org/abs/2605.26037v1
date: 2026-05-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.CL
tags: [embodied-agents, knowledge-graph, agentic-rl, tool-use, arxiv, auto-ingested]
---

# Peak-Then-Collapse and the Four Interface Channels of Knowledge-Graph Tool Use

**arXiv:** [2605.26037v1](https://arxiv.org/abs/2605.26037v1) · 2026-05-25 · cs.CL
**Authors:** Tianda Sun, Dimitar Kazakov

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We test the standard RLVR tool-use recipe -- GRPO on Qwen2.5-7B-Instruct -- on a deliberately minimal knowledge-graph tool API: four Freebase navigation verbs over Complex WebQuestions. Under a self-verifiable retrieval reward, the policy's tool-grounded answer rate climbs from $3.8\%$ to $9.6\%$ over 250 steps, then collapses to $0\%$ within a single 50-step window -- a \emph{peak-then-collapse} pattern replicated across four seeds. Across seven reward designs, we find four recurring failure modes: adding denser or more targeted proxy rewards shifts the failure mode rather than eliminating it. We argue that a key difference from Python interpreters, web search, and JSON APIs is interface feedback: their failures often leak natural-language signal the model saw in pretraining. A Python traceback names the failing line; an empty Freebase result \texttt{[]} does not. Stripping away that surface exposes a degradation regime that same-family reward redesigns do not fix. A direct oracle ablation rules out relation selection: injecting gold relations at every retrieval call lifts exact-match accuracy by only $+0.20$~pp, and $95.4\%$ of retrieval-dependent errors are retrieval-composition failures rather than answer-extraction failures. As a mitigation, one-iteration self-distillation reaches $40.0\%$ EM at 7B and is capacity-invariant: doubling capacity to 14B improves EM by only $0.25$~pp, and initialization barely matters -- the ceiling appears interface-bound within the 7B--14B range tested.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26037v1)
