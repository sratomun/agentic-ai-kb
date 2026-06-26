---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepSeek-V3 Technical Report"
authors: DeepSeek-AI et al.
url: https://arxiv.org/abs/2412.19437
date: 2025-02-18
ingested: 2026-06-22
tags: [arxiv, pretraining]
---

# DeepSeek-V3 Technical Report

**arXiv [2412.19437](https://arxiv.org/abs/2412.19437)** · 2025-02-18 (v2) · DeepSeek-AI et al.

**Significance.** A 671B-parameter open-weight MoE that matches leading closed models while pre-training for only ~2.788M H800 GPU-hours (~$5.6M) — a step-change in frontier-model training economics.

## Abstract
We present DeepSeek-V3, a strong Mixture-of-Experts (MoE) language model with 671B total parameters with 37B activated for each token. To achieve efficient inference and cost-effective training, DeepSeek-V3 adopts Multi-head Latent Attention (MLA) and DeepSeekMoE architectures, which were thoroughly validated in DeepSeek-V2. Furthermore, DeepSeek-V3 pioneers an auxiliary-loss-free strategy for load balancing and sets a multi-token prediction training objective for stronger performance. We pre-train DeepSeek-V3 on 14.8 trillion diverse and high-quality tokens, followed by Supervised Fine-Tuning and Reinforcement Learning stages to fully harness its capabilities. Comprehensive evaluations reveal that DeepSeek-V3 outperforms other open-source models and achieves performance comparable to leading closed-source models. Despite its excellent performance, DeepSeek-V3 requires only 2.788M H800 GPU hours for its full training. In addition, its training process is remarkably stable. Throughout the entire training process, we did not experience any irrecoverable loss spikes or perform any rollbacks. The model checkpoints are available at https://github.com/deepseek-ai/DeepSeek-V3.

## From the paper (full-text)

**Contribution / method.** A [[mixture-of-experts|MoE]] transformer (61 layers, hidden dim 7168; 1 shared + 256 routed experts per MoE layer, top-8 routed experts activated per token) built on two architectures validated in DeepSeek-V2: **Multi-head Latent Attention (MLA)** — low-rank joint KV compression (KV compression dim 512, query compression dim 1536) to shrink the inference KV cache — and **DeepSeekMoE**. Two new ingredients: (1) an **auxiliary-loss-free load-balancing** strategy that adjusts a per-expert routing bias (update speed γ = 0.001 for the first 14.3T tokens, then 0.0) instead of penalizing imbalance with an auxiliary loss; (2) a **Multi-Token Prediction (MTP)** training objective (depth D = 1, each token predicts one extra token; loss weight λ = 0.3 then 0.1), which can also be repurposed for speculative decoding. Trained with an **FP8 mixed-precision** framework — first validation of FP8 at this scale — with fine-grained tile-wise (1×128) / block-wise (128×128) quantization, keeping FP8 vs BF16 relative loss error below 0.25%, plus the DualPipe pipeline-parallel algorithm for near-full computation-communication overlap.

**Results.** **671B total parameters, 37B activated per token.** Pre-trained on **14.8T tokens** (max sequence length 4K), then YaRN-extended in two phases to **128K context**. Trained on a cluster of **2048 NVIDIA H800 GPUs**; total training cost **2.788M H800 GPU-hours** (2.664M pre-training + 119K context extension + 5K post-training), i.e. **~$5.576M** at $2/GPU-hour — pre-training alone is 180K GPU-hours per trillion tokens (~3.7 days). No irrecoverable loss spikes or rollbacks. The base model beats Qwen2.5-72B and LLaMA-3.1-405B base on most benchmarks: **MMLU 87.1, MMLU-Pro 64.4, MATH 61.6, HumanEval 65.2, GSM8K 89.3** (vs LLaMA-3.1-405B's 84.4 / 52.8 / 49.0 / 54.9 / 83.5). The chat model reaches MMLU 88.5, GPQA 59.1, MATH-500 90.2 — comparable to GPT-4o and Claude-3.5-Sonnet, and SOTA on math among non-long-CoT models. Reasoning was distilled from the DeepSeek-R1 series during post-training (SFT + RL via GRPO).

**Takeaway.** Co-designing algorithm, framework, and hardware (MLA + DeepSeekMoE + auxiliary-loss-free balancing + MTP + FP8 + DualPipe) brings frontier-grade [[pretraining|pre-training]] within reach at roughly an order of magnitude less compute than comparable dense models.

## Graph
- **Concepts:** [[pretraining|Pre-training]] · [[mixture-of-experts|Mixture of experts]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2412.19437.fulltext.md`
