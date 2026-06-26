---
type: concept
tags: [agents, frontier-models, scaling]
created: 2026-06-22
updated: 2026-06-22
kind: domain
---

# Scaling Laws

*The empirical relationships between compute, data, parameters, and capability — the equations that told labs that bigger, trained right, reliably gets better.*

## What it is
The predictable, power-law relationship between a model's loss and the resources spent training it (compute, dataset size, parameter count). Kaplan's laws first quantified it; Chinchilla corrected the recipe, showing most large models were *under-trained* on data for their size and that compute-optimal training favors far more tokens per parameter than prior practice. The adjacent and contested strand is *emergence* — whether new capabilities appear abruptly at scale or are an artifact of how you measure.

## Why it matters
Scaling laws are why the frontier became a capital game: if capability is a predictable function of compute, the winning move is to buy more of it — which is exactly the logic export controls and the [[nvidia]]/[[vera-rubin]] buildout target. For the exec the current signal is the *bend* in the curve: pre-training scaling returns are flattening, which is what pushed the field toward inference-time and post-training scaling ([[reasoning-models]], [[post-training]]). Where the next order-of-magnitude of capability comes from — more pre-training compute vs. more reasoning compute — is the single biggest strategic question in the stack.

## What the evidence shows
**Foundations.** Kaplan et al. established the loss-vs-compute power laws (arXiv:2001.08361); Chinchilla reset compute-optimal allocation toward more data per parameter (arXiv:2203.15556). The emergence debate is two-sided on the record: "Emergent Abilities of LLMs" argued for sharp capability jumps (arXiv:2206.07682), and "Are Emergent Abilities a Mirage?" argued they're largely an artifact of discontinuous metrics (arXiv:2304.15004).

**Recent developments.** The 2025 read is that the dominant scaling axis shifted from training compute toward inference-time compute → [[2025-12-30-blog-raschka-state-of-llms-2025]]; RL itself is now discussed as following its own scaling curve → [[2025-10-20-blog-lambert-how-to-scale-rl]].

## Relationships
- governs [[pretraining]], [[mixture-of-experts]]; cross-cuts [[frontier-model-training]]
- bent toward inference-time scaling in [[reasoning-models]], [[post-training]]
- cashed out in compute via [[nvidia]], [[vera-rubin]]
- explained by [[sebastian-raschka]], [[nathan-lambert]]

## Key papers (full-text ingested)
- [[2026-06-22-arxiv-2001-08361-scaling-laws-for-neural-language-models|Scaling Laws (Kaplan)]] — smooth power laws of loss vs compute/data/params
- [[2022-03-29-arxiv-2203-15556-compute-optimal-chinchilla|Chinchilla]] — compute-optimal ≈20 tokens/param; 70B on 1.4T beats Gopher 280B & GPT-3 175B
- [[2022-06-15-arxiv-2206-07682-emergent-abilities|Emergent Abilities]] — sharp above-random jumps at scale thresholds
- [[2023-04-28-arxiv-2304-15004-emergence-mirage|Emergence: a Mirage?]] — >92% of "emergence" lives under 2 discontinuous metrics; smooth under continuous ones
- [[2022-02-11-arxiv-2202-05924-compute-trends-three-eras|Compute Trends (3 eras)]] — compute doubling time fell to ~5.7 months in the deep-learning era
