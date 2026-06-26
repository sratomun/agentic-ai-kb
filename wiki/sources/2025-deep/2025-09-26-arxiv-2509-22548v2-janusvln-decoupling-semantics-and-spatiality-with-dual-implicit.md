---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "JanusVLN: Decoupling Semantics and Spatiality with Dual Implicit Memory for Vision-Language Navigation"
authors: Shuang Zeng, Dekang Qi, Xinyuan Chang, Feng Xiong et al.
url: https://arxiv.org/abs/2509.22548v2
date: 2025-09-26
citationCount: 80
influentialCitationCount: 4
velocity: 9.05
ingested: 2026-06-22
tags: [embodied-agents, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# JanusVLN: Decoupling Semantics and Spatiality with Dual Implicit Memory for Vision-Language Navigation

**arXiv [2509.22548v2](https://arxiv.org/abs/2509.22548v2)** · 2025-09-26 · **80 citations** (4 influential · 9.05/mo) · Shuang Zeng, Dekang Qi, Xinyuan Chang, Feng Xiong et al.

## Abstract
Vision-and-Language Navigation requires an embodied agent to navigate through unseen environments, guided by natural language instructions and a continuous video stream. Recent advances in VLN have been driven by the powerful semantic understanding of Multimodal Large Language Models. However, these methods typically rely on explicit semantic memory, such as building textual cognitive maps or storing historical visual frames. This type of method suffers from spatial information loss, computational redundancy, and memory bloat, which impede efficient navigation. Inspired by the implicit scene representation in human navigation, analogous to the left brain's semantic understanding and the right brain's spatial cognition, we propose JanusVLN, a novel VLN framework featuring a dual implicit neural memory that models spatial-geometric and visual-semantic memory as separate, compact, and fixed-size neural representations. This framework first extends the MLLM to incorporate 3D prior knowledge from the spatial-geometric encoder, thereby enhancing the spatial reasoning capabilities of models based solely on RGB input. Then, the historical key-value caches from the spatial-geometric and visual-semantic encoders are constructed into a dual implicit memory. By retaining only the KVs of tokens in the initial and sliding window, redundant computation is avoided, enabling efficient incremental updates. Extensive experiments demonstrate that JanusVLN outperforms over 20 recent methods to achieve SOTA performance. For example, the success rate improves by 10.5-35.5 compared to methods using multiple data types as input and by 3.6-10.8 compared to methods using more RGB training data. This indicates that the proposed dual implicit neural memory, as a novel paradigm, explores promising new directions for future VLN research. Ours project page: https://miv-xjtu.github.io/JanusVLN.github.io/.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related work 2.1 Vision-language navigation with multiple visual inputs 2.2 Multi-modal large language models for RGB only navigation 2.3 Spatial reasoning via vision-language models 3 Method 3.1 Preliminary Navigation task definition. Visual geometry grounded transformer (VGGT). 3.2 Dual implicit memory Implicit neural representation. Hybrid incremental update. 3.3 JanusVLN architecture Decoupling visual perception: semantics and spatiality. Spatial-aware feature fusion. 4 Experiments 4.1 Experimental setup Simulation environments and metrics. Real-world evaluation setup. Implementation details. 4.2 Main results Results on VLN-CE benchmark. Real-world qualitative results. 4.3 Ablation study Ablation of the dual implicit memory. Ablation of 3D geometric priors. Ablation on memory size. 5 Conclusion A The use of large language models (LLMs) B Model structure details C More ablation studies Real world quantitative results. Results on recent HM3D-OVON. Ablation of fusion strateg…

**Method / approach.** Method 3.1 Preliminary Navigation task definition. Visual geometry grounded transformer (VGGT). 3.2 Dual implicit memory Implicit neural representation. Hybrid incremental update. 3.3 JanusVLN architecture Decoupling visual perception: semantics and spatiality. Spatial-aware feature fusion. 4 Experiments 4.1 Experimental setup Simulation environments and metrics. Real-world evaluation setup. Implementation details. 4.2 Main results Results on VLN-CE benchmark. Real-world qualitative results. 4.3 Ablation study Ablation of the dual implicit memory. Ablation of 3D geometric priors. Ablation on memory size. 5 Conclusion A The use of large language models (LLMs) B Model structure details C More ablation studies Real world quantitative results. Results on recent HM3D-OVON. Ablation of fusion strategies. Data Ablation. D Statistical analysis Success and strengths analysis. Performance by instruction l…

**Results.** Experiments 4.1 Experimental setup Simulation environments and metrics. Real-world evaluation setup. Implementation details. 4.2 Main results Results on VLN-CE benchmark. Real-world qualitative results. 4.3 Ablation study Ablation of the dual implicit memory. Ablation of 3D geometric priors. Ablation on memory size. 5 Conclusion A The use of large language models (LLMs) B Model structure details C More ablation studies Real world quantitative results. Results on recent HM3D-OVON. Ablation of fusion strategies. Data Ablation. D Statistical analysis Success and strengths analysis. Performance by instruction length. Failure case analysis. E More qualitative results Visualization analysis of spatial geometric tokens. More qualitative results. † † footnotetext: ∗ Work done during the internship at Amap, Alibaba Group. † † footnotetext: † Corresponding author. JanusV…

**Conclusion.** Conclusion A The use of large language models (LLMs) B Model structure details C More ablation studies Real world quantitative results. Results on recent HM3D-OVON. Ablation of fusion strategies. Data Ablation. D Statistical analysis Success and strengths analysis. Performance by instruction length. Failure case analysis. E More qualitative results Visualization analysis of spatial geometric tokens. More qualitative results. † † footnotetext: ∗ Work done during the internship at Amap, Alibaba Group. † † footnotetext: † Corresponding author. JanusVLN: Decoupling Semantics and Spatiality with Dual Implicit Memory for Vision-Language Navigation Shuang Zeng 1, 2 * , Dekang Qi 2 , Xinyuan Chang 2…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.22548v2.md` · `raw/arxiv/2509.22548v2.fulltext.md`
