---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling"
authors: Meng Wei, Chenyang Wan, Xiqian Yu, Tai Wang et al.
url: https://arxiv.org/abs/2507.05240v1
date: 2025-07-07
citationCount: 83
influentialCitationCount: 22
velocity: 7.22
ingested: 2026-06-22
tags: [embodied-agents, agent-reliability, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling

**arXiv [2507.05240v1](https://arxiv.org/abs/2507.05240v1)** · 2025-07-07 · **83 citations** (22 influential · 7.22/mo) · Meng Wei, Chenyang Wan, Xiqian Yu, Tai Wang et al.

## Abstract
Vision-and-Language Navigation (VLN) in real-world settings requires agents to process continuous visual streams and generate actions with low latency grounded in language instructions. While Video-based Large Language Models (Video-LLMs) have driven recent progress, current VLN methods based on Video-LLM often face trade-offs among fine-grained visual understanding, long-term context modeling and computational efficiency. We introduce StreamVLN, a streaming VLN framework that employs a hybrid slow-fast context modeling strategy to support multi-modal reasoning over interleaved vision, language and action inputs. The fast-streaming dialogue context facilitates responsive action generation through a sliding-window of active dialogues, while the slow-updating memory context compresses historical visual states using a 3D-aware token pruning strategy. With this slow-fast design, StreamVLN achieves coherent multi-turn dialogue through efficient KV cache reuse, supporting long video streams with bounded context size and inference cost. Experiments on VLN-CE benchmarks demonstrate state-of-the-art performance with stable low latency, ensuring robustness and efficiency in real-world deployment. The project page is: \href{https://streamvln.github.io/}{https://streamvln.github.io/}.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Method 3.1 Preliminary: Continuous Multi-Turn Autoregressive Generation 3.2 Fast-Streaming Dialogue Context 3.3 Slow-Updating Memory Context 3.4 Co-Training with Multi-Source Data. 4 Experiments 4.1 Experimental Setup 4.2 Implementation Details 4.3 Comparisons with State-of-the-Arts 4.4 Ablation Studies 5 Conclusion 6 Limitations 1 Navigation Instruction Design 2 Results on Zero-Shot Object Navigation 3 Voxel-based Spatial Pruning. 4 More Qualitative Results StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling Meng Wei ∗,1,2 Chenyang Wan ∗,1,3 Xiqian Yu ∗,1 Tai Wang ∗†,1 Yuqiang Yang 1 Xiaohan Mao 1,4 Chenming Zhu 1,2 Wenzhe Cai 1 Hanqing Wang 1 Yilun Chen 1 Xihui Liu ‡,2 Jiangmiao Pang ‡,1 1 Shanghai AI Laboratory 2 The University of Hong Kong 3 Zhejiang University 4 Shanghai Jiao Tong University Abstract Vision-and-Language Navigation (VLN) in real-world settings requires agents to process continuous visual streams and generate actions with lo…

**Method / approach.** Method 3.1 Preliminary: Continuous Multi-Turn Autoregressive Generation 3.2 Fast-Streaming Dialogue Context 3.3 Slow-Updating Memory Context 3.4 Co-Training with Multi-Source Data. 4 Experiments 4.1 Experimental Setup 4.2 Implementation Details 4.3 Comparisons with State-of-the-Arts 4.4 Ablation Studies 5 Conclusion 6 Limitations 1 Navigation Instruction Design 2 Results on Zero-Shot Object Navigation 3 Voxel-based Spatial Pruning. 4 More Qualitative Results StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling Meng Wei ∗,1,2 Chenyang Wan ∗,1,3 Xiqian Yu ∗,1 Tai Wang ∗†,1 Yuqiang Yang 1 Xiaohan Mao 1,4 Chenming Zhu 1,2 Wenzhe Cai 1 Hanqing Wang 1 Yilun Chen 1 Xihui Liu ‡,2 Jiangmiao Pang ‡,1 1 Shanghai AI Laboratory 2 The University of Hong Kong 3 Zhejiang University 4 Shanghai Jiao Tong University Abstract Vision-and-Language Navigation (VLN) in real-world settings requires agents…

**Results.** Experiments 4.1 Experimental Setup 4.2 Implementation Details 4.3 Comparisons with State-of-the-Arts 4.4 Ablation Studies 5 Conclusion 6 Limitations 1 Navigation Instruction Design 2 Results on Zero-Shot Object Navigation 3 Voxel-based Spatial Pruning. 4 More Qualitative Results StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling Meng Wei ∗,1,2 Chenyang Wan ∗,1,3 Xiqian Yu ∗,1 Tai Wang ∗†,1 Yuqiang Yang 1 Xiaohan Mao 1,4 Chenming Zhu 1,2 Wenzhe Cai 1 Hanqing Wang 1 Yilun Chen 1 Xihui Liu ‡,2 Jiangmiao Pang ‡,1 1 Shanghai AI Laboratory 2 The University of Hong Kong 3 Zhejiang University 4 Shanghai Jiao Tong University Abstract Vision-and-Language Navigation (VLN) in real-world settings requires agents to process continuous visual streams and generate actions with low latency grounded in language instructions. While Video-based Large Language Mode…

**Conclusion.** Conclusion 6 Limitations 1 Navigation Instruction Design 2 Results on Zero-Shot Object Navigation 3 Voxel-based Spatial Pruning. 4 More Qualitative Results StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling Meng Wei ∗,1,2 Chenyang Wan ∗,1,3 Xiqian Yu ∗,1 Tai Wang ∗†,1 Yuqiang Yang 1 Xiaohan Mao 1,4 Chenming Zhu 1,2 Wenzhe Cai 1 Hanqing Wang 1 Yilun Chen 1 Xihui Liu ‡,2 Jiangmiao Pang ‡,1 1 Shanghai AI Laboratory 2 The University of Hong Kong 3 Zhejiang University 4 Shanghai Jiao Tong University Abstract Vision-and-Language Navigation (VLN) in real-world settings requires agents to process continuous visual streams and generate actions with low latency grounded…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2507.05240v1.md` · `raw/arxiv/2507.05240v1.fulltext.md`
