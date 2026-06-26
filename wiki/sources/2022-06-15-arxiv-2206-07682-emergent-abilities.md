---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Emergent Abilities of Large Language Models"
authors: Jason Wei et al.
url: https://arxiv.org/abs/2206.07682
date: 2022-06-15
citationCount: omit
tags: [arxiv, scaling-laws]
---

# Emergent Abilities of Large Language Models

**arXiv [2206.07682](https://arxiv.org/abs/2206.07682)** · 2022-06-15 · Jason Wei et al.

**Significance.** Coined and catalogued "emergent abilities" — capabilities absent in smaller models that appear sharply, as phase transitions, past a critical scale.

## Abstract
Scaling up language models has been shown to predictably improve performance and sample efficiency on a wide range of downstream tasks. This paper instead discusses an unpredictable phenomenon that we refer to as emergent abilities of large language models. We consider an ability to be emergent if it is not present in smaller models but is present in larger models. Thus, emergent abilities cannot be predicted simply by extrapolating the performance of smaller models. The existence of such emergence raises the question of whether additional scaling could potentially further expand the range of capabilities of language models.

## From the paper (full-text)
**Contribution / method.** Define emergence precisely — "An ability is emergent if it is not present in smaller models but is present in larger models" — and survey few-shot-prompting and augmented-prompting tasks across model families (GPT-3, LaMDA, Gopher, Chinchilla, PaLM, FLAN), plotting performance against training FLOPs / parameters to locate sharp, above-random jumps ("phase transitions").

**Results.** Emergence thresholds (training FLOPs / params / model): 3-digit addition/subtraction jumps above random at 2.3E22 FLOPs / 13B (GPT-3); MMLU (57-topic avg) at 3.1E23 / 175B (GPT-3); TruthfulQA at 5.0E23 / 280B (Gopher), jumping >20% above random; Word-in-Context (WiC) only emerges at 2.5E24 / 540B (PaLM). Augmented prompting: chain-of-thought surpasses standard prompting only at ≈10^23 FLOPs (~100B params); instruction-following finetuning hurts at ≤7E21 / 8B but helps from ≈10^23 / ~100B; scratchpad 8-digit addition emerges at 8.9E19 / 40M (LaMDA). Performance is near-random below the threshold, then climbs steeply above it.

**Takeaway.** Some capabilities can't be forecast from small-model scaling curves — they switch on suddenly at scale, which is both a research opportunity and an alignment risk.

## Graph
- **Concepts:** [[scaling-laws|Scaling laws]]
- **Entities:** PaLM, GPT-3, LaMDA, Gopher, Chinchilla, BIG-Bench, MMLU, chain-of-thought
- **Raw:** `raw/arxiv/2206.07682.fulltext.md`
