---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "StreamingVLM: Real-Time Understanding for Infinite Video Streams"
authors: Ruyi Xu, Guangxuan Xiao, Yukang Chen, Liuning He et al.
url: https://arxiv.org/abs/2510.09608v2
date: 2025-10-10
citationCount: 59
influentialCitationCount: 7
velocity: 7.04
ingested: 2026-06-22
tags: [agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# StreamingVLM: Real-Time Understanding for Infinite Video Streams

**arXiv [2510.09608v2](https://arxiv.org/abs/2510.09608v2)** · 2025-10-10 · **59 citations** (7 influential · 7.04/mo) · Ruyi Xu, Guangxuan Xiao, Yukang Chen, Liuning He et al.

## Abstract
Vision-language models (VLMs) could power real-time assistants and autonomous agents, but they face a critical challenge: understanding near-infinite video streams without escalating latency and memory usage. Processing entire videos with full attention leads to quadratic computational costs and poor performance on long videos. Meanwhile, simple sliding window methods are also flawed, as they either break coherence or suffer from high latency due to redundant recomputation. In this paper, we introduce StreamingVLM, a model designed for real-time, stable understanding of infinite visual input. Our approach is a unified framework that aligns training with streaming inference. During inference, we maintain a compact KV cache by reusing states of attention sinks, a short window of recent vision tokens, and a long window of recent text tokens. This streaming ability is instilled via a simple supervised fine-tuning (SFT) strategy that applies full attention on short, overlapped video chunks, which effectively mimics the inference-time attention pattern without training on prohibitively long contexts. For evaluation, we build Inf-Streams-Eval, a new benchmark with videos averaging over two hours that requires dense, per-second alignment between frames and text. On Inf-Streams-Eval, StreamingVLM achieves a 66.18% win rate against GPT-4O mini and maintains stable, real-time performance at up to 8 FPS on a single NVIDIA H100. Notably, our SFT strategy also enhances general VQA abilities without any VQA-specific fine-tuning, improving performance on LongVideoBench by +4.30 and OVOBench Realtime by +5.96. Code is available at https://github.com/mit-han-lab/streaming-vlm.

## From the paper (full-text excerpts)
**Introduction.** introduction 2 Method 2.1 Inference Scheme of StreamingVLM Streaming-aware KV Cache Contiguous RoPE 2.2 Training Strategy 2.3 Data Curation Pipeline 2.3.1 Video Collection and ASR 2.3.2 Data Cleaning 2.3.3 SFT and Evaluation Data Segmentation 2.3.4 High-quality Annealing Data 3 Experiments 3.1 Experimental Setup Training Baselines 3.2 Accuracy Results 3.2.1 Captioning 3.2.2 VQA 3.3 Efficiency Tests 3.4 Ablation Study 3.4.1 Contiguous RoPE 3.4.2 Sliding Window and Sink 3.4.3 Training Strategy and Dataset 4 Related Work Vision–Language Models Long-Context and Streaming Inference in Text LLMs Streaming and Online Video LLMs VLMs Benchmarks and Evaluation 5 conclusion References A Appendix A.1 LLM Usage Statement A.2 Stability Over Time A.3 Sensitivity Analysis of Sink Token Window Size A.4 Demo License: CC BY 4.0 arXiv:2510.09608v2 [cs.CV] 31 May 2026 StreamingVLM: Real-Time Understanding for Infinite Video Streams Ruyi Xu 1∗ Guangxuan Xiao 1∗ Yukang Chen 2 Liuning He 1 Ya…

**Method / approach.** Method 2.1 Inference Scheme of StreamingVLM Streaming-aware KV Cache Contiguous RoPE 2.2 Training Strategy 2.3 Data Curation Pipeline 2.3.1 Video Collection and ASR 2.3.2 Data Cleaning 2.3.3 SFT and Evaluation Data Segmentation 2.3.4 High-quality Annealing Data 3 Experiments 3.1 Experimental Setup Training Baselines 3.2 Accuracy Results 3.2.1 Captioning 3.2.2 VQA 3.3 Efficiency Tests 3.4 Ablation Study 3.4.1 Contiguous RoPE 3.4.2 Sliding Window and Sink 3.4.3 Training Strategy and Dataset 4 Related Work Vision–Language Models Long-Context and Streaming Inference in Text LLMs Streaming and Online Video LLMs VLMs Benchmarks and Evaluation 5 conclusion References A Appendix A.1 LLM Usage Statement A.2 Stability Over Time A.3 Sensitivity Analysis of Sink Token Window Size A.4 Demo License: CC BY 4.0 arXiv:2510.09608v2 [cs.CV] 31 May 2026 StreamingVLM: Real-Time Understanding for Infinite…

**Results.** Experiments 3.1 Experimental Setup Training Baselines 3.2 Accuracy Results 3.2.1 Captioning 3.2.2 VQA 3.3 Efficiency Tests 3.4 Ablation Study 3.4.1 Contiguous RoPE 3.4.2 Sliding Window and Sink 3.4.3 Training Strategy and Dataset 4 Related Work Vision–Language Models Long-Context and Streaming Inference in Text LLMs Streaming and Online Video LLMs VLMs Benchmarks and Evaluation 5 conclusion References A Appendix A.1 LLM Usage Statement A.2 Stability Over Time A.3 Sensitivity Analysis of Sink Token Window Size A.4 Demo License: CC BY 4.0 arXiv:2510.09608v2 [cs.CV] 31 May 2026 StreamingVLM: Real-Time Understanding for Infinite Video Streams Ruyi Xu 1∗ Guangxuan Xiao 1∗ Yukang Chen 2 Liuning He 1 Yao Lu 2 Song Han 1,2 1 MIT 2 NVIDIA https://github.com/mit-han-lab/streaming-vlm Abstract Vision-language models (VLMs) could power real-time assistant…

**Conclusion.** conclusion References A Appendix A.1 LLM Usage Statement A.2 Stability Over Time A.3 Sensitivity Analysis of Sink Token Window Size A.4 Demo License: CC BY 4.0 arXiv:2510.09608v2 [cs.CV] 31 May 2026 StreamingVLM: Real-Time Understanding for Infinite Video Streams Ruyi Xu 1∗ Guangxuan Xiao 1∗ Yukang Chen 2 Liuning He 1 Yao Lu 2 Song Han 1,2 1 MIT 2 NVIDIA https://github.com/mit-han-lab/streaming-vlm Abstract Vision-language models (VLMs) could power real-time assistants and autonomous agents, but they face a critical challenge: understanding near-infinite video streams without escalating latency and memory usage. Processing entire videos with full attention leads to quadratic computational costs…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2510.09608v2.md` · `raw/arxiv/2510.09608v2.fulltext.md`
