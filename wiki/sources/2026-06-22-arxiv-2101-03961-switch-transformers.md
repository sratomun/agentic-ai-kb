---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity"
authors: William Fedus et al.
url: https://arxiv.org/abs/2101.03961
date: 2021-01-11
ingested: 2026-06-22
tags: [arxiv, mixture-of-experts]
---

# Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity

**arXiv [2101.03961](https://arxiv.org/abs/2101.03961)** · 2021-01-11 · William Fedus, Barret Zoph, Noam Shazeer

**Significance.** Showed that routing each token to a single expert (top-1) makes MoE simple and stable enough to scale to a trillion-plus parameters while holding FLOPs/token fixed, turning sparsity into a practical scaling axis.

## Abstract
In deep learning, models typically reuse the same parameters for all inputs. Mixture of Experts (MoE) models defy this and instead select different parameters for each incoming example. The result is a sparsely-activated model—with an outrageous number of parameters—but a constant computational cost. However, despite several notable successes of MoE, widespread adoption has been hindered by complexity, communication costs, and training instability. We address these with the introduction of the Switch Transformer. We simplify the MoE routing algorithm and design intuitive improved models with reduced communication and computational costs. Our proposed training techniques mitigate the instabilities, and we show large sparse models may be trained, for the first time, with lower precision (bfloat16) formats. We design models based off T5-Base and T5-Large (Raffel et al., 2019) to obtain up to 7x increases in pre-training speed with the same computational resources. These improvements extend into multilingual settings where we measure gains over the mT5-Base version across all 101 languages. Finally, we advance the current scale of language models by pre-training up to trillion parameter models on the "Colossal Clean Crawled Corpus", and achieve a 4x speedup over the T5-XXL model.

## From the paper (full-text)
**Contribution / method.** The core move is **Switch routing**: contrary to Shazeer et al. (2017), who argued routing to k>1 experts was needed for non-trivial routing gradients, the authors route each token to **only a single (top-1) expert** — the "Switch layer." This cuts router computation, at least halves each expert's batch (expert capacity), and simplifies communication. Each expert sits on its own device with unique FFN weights, so total parameters grow with the number of devices while FLOPs/token stay fixed. **Expert capacity** = (tokens_per_batch / num_experts) × **capacity factor**; a factor >1.0 buffers against uneven routing, and tokens that overflow an expert are dropped (passed via the residual connection). A **differentiable auxiliary load-balancing loss** (coefficient α = 10⁻²) pushes routing toward uniform. Stability comes from **selective precision** — casting only the router's local computation to float32 while keeping bfloat16 elsewhere, enabling (for the first time) large sparse training in low precision — plus a smaller init scale (reduce default s=1.0 by 10×) and, for fine-tuning, **expert dropout** (e.g. 0.1 on non-expert layers, 0.4 inside experts). Large sparse teachers can be **distilled into small dense students**, initializing the student with the teacher's non-expert weights and mixing 0.75 hard / 0.25 soft loss.

**Results.** Switch-Base hits **7x+ pre-training speedup** over T5-Base at fixed FLOPs/token (Switch-Base 64-expert reaches T5-Base's step-60k quality at step 450k, a 7.5x step speedup); on a wall-clock basis the 64-expert model trains to similar perplexity in **one-seventh the time** of T5-Base, and yields a **2.5x speedup over T5-Large** despite T5-Large using 3.5x more FLOPs/token. Scaling experts from 2 up to a **256-expert model (14.7B params)** improves quality at equal compute. Two large models combine data/model/expert parallelism: **Switch-XXL (395B params)** and **Switch-C (1.571T / "1.6T" params, 2048 experts, 15 layers, 890B FLOPs/seq)**; Switch-C is **4x faster to a fixed perplexity than T5-XXL**. Notably, the 1.6T Switch-C showed **no training instability**, while the FLOP-heavier Switch-XXL was sometimes unstable. Fine-tuning: FLOP-matched Switch variants beat T5-Base/T5-Large on SuperGLUE by **+4.4 and +2 points** (e.g. SuperGLUE 79.5 vs 75.1 for Base, 84.7 vs 82.7 for Large). Distillation: compressing a sparse teacher up to **99%** (down to 223M dense) still retains **~28-30% of the quality gain** (37% retained at 82% compression of the 1.1B model); a fine-tuned 7.4B Switch-Base distilled into 223M T5-Base keeps 30% of the gain at 97% compression. Multilingual: gains on **all 101 languages**, mean **5x step speedup** over mT5-Base with **91% of languages ≥4x**.

**Takeaway.** Top-1 routing plus a handful of stability tricks (selective float32 routing, smaller init, load-balancing loss) makes sparse expert models simple, stable, and scalable — establishing parameter count (decoupled from FLOPs) as a first-class scaling axis.

## Graph
- **Concepts:** [[mixture-of-experts|Mixture-of-Experts]]
- **Raw:** `raw/arxiv/2101.03961.fulltext.md`
