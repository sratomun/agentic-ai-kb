---
type: source
source_type: arxiv
title: "JAF: Judge Agent Forest"
authors: Sahil Garg, Brad Cheezum, Sridhar Dutta, Vishal Agarwal (Averlon)
url: https://arxiv.org/abs/2601.22269v1
date: 2026-01-29
ingested: 2026-06-22
depth: full-text
tags: [agent-evaluation, llm-as-judge, arxiv]
---

# JAF: Judge Agent Forest

**Why it matters:** A practical fix for **LLM-as-judge**: judge a *cohort* of related responses jointly instead of scoring each in isolation, so the judge catches cross-instance inconsistencies — and ships with an explicit **consistency metric** (acceptance probability over randomized re-judgings) that doubles as a triage signal for human review. Pairs directly with the Contagion-Networks warning that how you wire judges changes the verdict.

## What it is
A single judge LLM (here Llama3.3-Nemotron-Super-49B-v1.5) is repeatedly invoked on each focal query–response pair **together with a small, relation-aware random subset of peer pairs** from the same logical cohort (e.g. all vulnerability–asset pairs for a tenant). Overlapping neighborhoods form a cohort-level knowledge graph; repeated randomized passes give belief-propagation / random-forest-style ensembling — all in-context, no architecture change. Optional learned LSH selects diverse exemplars (not evaluated here; the paper uses a "vanilla" 4-positive/4-negative neighbor scheme). Running example: vulnerability/misconfig triage in cloud environments.

## Metric (the contribution for eval pipelines)
- **Probabilistic correctness / empirical acceptance probability** p̂ᵢ = fraction of R=10 randomized judge re-evaluations (each with a freshly sampled neighborhood) that accept the answer. High, stable p̂ᵢ = robust decision; low or variable p̂ᵢ = fragile → escalate to human review. This is an explicit **consistency score**, not single-shot agreement — important under extreme class imbalance (often <0.1% of findings are actually exploitable, so the final label alone is not enough; the *reasoning* must be sound).

## Findings
- On 315 assets, vs an isolated-judge self-refinement baseline, JAF shifts the correctness-probability mass markedly higher with **lower variance** — more answers near p̂ᵢ≈1.
- **Converges in fewer refinement iterations:** JAF after 5 iterations already resembles the baseline after 10; baseline retains a persistent low-confidence tail.
- JAF preserves and *clarifies* the genuinely hard cases (low p̂ᵢ under both) — exactly the issues to route to humans.
- Even the naive instantiation (no embeddings/LSH, neighbors by shared claimed-software overlap) delivers the gain.

## So what
If you use agent-as-judge: isolated per-item scoring is the weak baseline; cohort judging plus a randomized-re-judging consistency score (p̂ᵢ) is more accurate, more stable, and gives a built-in human-escalation signal. Still an LLM judge — validate per model and cross-check ([[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]]).

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[llm-as-judge|LLM-as-judge]]
- **Entities:** [[jaf]]
- **Raw:** alphaXiv full-text (id 2601.22269v1)

## Relationships
- introduced by [[jaf]]
- addresses [[llm-as-judge]]
- part of [[agent-evaluation]]
