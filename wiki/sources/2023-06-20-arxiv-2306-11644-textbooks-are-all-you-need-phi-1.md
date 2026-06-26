---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Textbooks Are All You Need"
authors: Suriya Gunasekar et al.
url: https://arxiv.org/abs/2306.11644
date: 2023-06-20
ingested: 2026-06-22
tags: [arxiv, synthetic-data, data]
---

# Textbooks Are All You Need

**arXiv [2306.11644](https://arxiv.org/abs/2306.11644)** · 2023-06-20 · Suriya Gunasekar, Yi Zhang, Sébastien Bubeck, Ronen Eldan, Yuanzhi Li, et al. (Microsoft Research)

**Significance.** The phi-1 paper — the loudest argument that "textbook-quality" synthetic data can bend scaling laws, letting a 1.3B model beat code models 10–100x its size. Launched the phi family and the data-quality-over-scale thesis.

## Abstract
We introduce phi-1, a new large language model for code, with significantly smaller size than competing models: phi-1 is a Transformer-based model with 1.3B parameters, trained for 4 days on 8 A100s, using a selection of "textbook quality" data from the web (6B tokens) and synthetically generated textbooks and exercises with GPT-3.5 (1B tokens). Despite this small scale, phi-1 attains pass@1 accuracy 50.6% on HumanEval and 55.5% on MBPP. It also displays surprising emergent properties compared to phi-1-base, our model before our finetuning stage on a dataset of coding exercises, and phi-1-small, a smaller model with 350M parameters trained with the same pipeline that still achieves 45% on HumanEval.

## From the paper (full-text)
**Contribution / method.** A data-centric pipeline rather than an architectural one. Pretraining ("CodeTextbook") uses two pieces: ~6B tokens of web Python code filtered by a GPT-4-labeled classifier scoring "educational value," plus <1B tokens of GPT-3.5-generated synthetic textbooks (diversity injected by randomizing topic/audience constraints in the prompt). Finetuning ("CodeExercises") uses ~180M tokens of GPT-3.5-generated Python exercises (docstring → function). The model is a conventional 1.3B decoder-only Transformer (FlashAttention, RoPE, codegen-350M tokenizer), pretrained in under 4 days on 8 A100s + 7 hours finetuning.

**Results.** phi-1 (1.3B, ~7B total tokens) reaches 50.6% pass@1 on HumanEval and 55.5% on MBPP, beating CodeGen-Mono-16.1B (29.3%), StarCoder-Prompted 15.5B (40.8%), PaLM 2-S, and GPT-3.5 (47%) on HumanEval despite being orders of magnitude smaller. phi-1-base (no finetuning) already hits 29% HumanEval; the ~180M-token finetune jumps it to 50.6% and unlocks emergent use of external libraries (Pygame, Tkinter, PyTorch) absent from the finetuning set. phi-1-small (350M) reaches 45%. To rebut contamination claims, the authors graded 50 new unconventional problems with GPT-4 (phi-1 averaged 52% vs. StarCoder 51%) and retrained after aggressively pruning up to 40% (354K of 879.5K) of CodeExercises by embedding/AST similarity to HumanEval — phi-1 still beat StarCoder-Prompted (45.1% vs 41.5% at τ=0.8).

**Takeaway.** Curating and synthesizing high-signal "textbook" data can substitute for raw scale on a narrow task; finetuning on a small high-quality exercise set is what triggers emergent capability.

## Graph
- **Concepts:** [[synthetic-data|Synthetic data]] · [[scaling-laws|Scaling laws]]
- **Entities:** [[microsoft]]
- **Raw:** `raw/arxiv/2306.11644.fulltext.md`
