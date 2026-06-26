---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving"
authors: Xiaosong Jia, Junqi You, Zhiyuan Zhang, Junchi Yan
url: https://arxiv.org/abs/2503.07656v2
date: 2025-03-07
citationCount: 111
influentialCitationCount: 10
velocity: 7.16
ingested: 2026-06-22
tags: [autonomous-driving-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving

**arXiv [2503.07656v2](https://arxiv.org/abs/2503.07656v2)** · 2025-03-07 · **111 citations** (10 influential · 7.16/mo) · Xiaosong Jia, Junqi You, Zhiyuan Zhang, Junchi Yan

## Abstract
End-to-end autonomous driving (E2E-AD) has emerged as a trend in the field of autonomous driving, promising a data-driven, scalable approach to system design. However, existing E2E-AD methods usually adopt the sequential paradigm of perception-prediction-planning, which leads to cumulative errors and training instability. The manual ordering of tasks also limits the system`s ability to leverage synergies between tasks (for example, planning-aware perception and game-theoretic interactive prediction and planning). Moreover, the dense BEV representation adopted by existing methods brings computational challenges for long-range perception and long-term temporal fusion. To address these challenges, we present DriveTransformer, a simplified E2E-AD framework for the ease of scaling up, characterized by three key features: Task Parallelism (All agent, map, and planning queries direct interact with each other at each block), Sparse Representation (Task queries direct interact with raw sensor features), and Streaming Processing (Task queries are stored and passed as history information). As a result, the new framework is composed of three unified operations: task self-attention, sensor cross-attention, temporal cross-attention, which significantly reduces the complexity of system and leads to better training stability. DriveTransformer achieves state-of-the-art performance in both simulated closed-loop benchmark Bench2Drive and real world open-loop benchmark nuScenes with high FPS.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 Method 3.1 Initialization Tokenization 3.2 Token Interaction 3.3 DETR-Style Task Head 3.4 Loss Optimization 4 Experiments 4.1 Dataset Benchmark 4.2 Comparison with State-of-the-Art Methods 4.3 Ablation Studies 4.4 Robustness Analysis 5 Conclusion A Implementation Details B Dev10 Benchmark C Limitations D Comparison of Middle Tasks E Comparison with Concurrent Parallel and Sparse based Methods F Training Stability Multi-Stage Training DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving Xiaosong Jia*, Junqi You*, Zhiyuan Zhang*, Junchi Yan † Sch. of Computer Science Sch. of Artificial Intelligence, Shanghai Jiao Tong University * Equal Contributions † Correspondence Author https://github.com/Thinklab-SJTU/DriveTransformer/ Abstract End-to-end autonomous driving (E2E-AD) has emerged as a trend in the field of autonomous driving, promising a data-driven, scalable approach to system design. However, existing E2E-AD methods usually adopt the sequential paradigm of…

**Method / approach.** Method 3.1 Initialization Tokenization 3.2 Token Interaction 3.3 DETR-Style Task Head 3.4 Loss Optimization 4 Experiments 4.1 Dataset Benchmark 4.2 Comparison with State-of-the-Art Methods 4.3 Ablation Studies 4.4 Robustness Analysis 5 Conclusion A Implementation Details B Dev10 Benchmark C Limitations D Comparison of Middle Tasks E Comparison with Concurrent Parallel and Sparse based Methods F Training Stability Multi-Stage Training DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving Xiaosong Jia*, Junqi You*, Zhiyuan Zhang*, Junchi Yan † Sch. of Computer Science Sch. of Artificial Intelligence, Shanghai Jiao Tong University * Equal Contributions † Correspondence Author https://github.com/Thinklab-SJTU/DriveTransformer/ Abstract End-to-end autonomous driving (E2E-AD) has emerged as a trend in the field of autonomous driving, promising a data-driven, scalable approach to system design. However, e…

**Results.** Experiments 4.1 Dataset Benchmark 4.2 Comparison with State-of-the-Art Methods 4.3 Ablation Studies 4.4 Robustness Analysis 5 Conclusion A Implementation Details B Dev10 Benchmark C Limitations D Comparison of Middle Tasks E Comparison with Concurrent Parallel and Sparse based Methods F Training Stability Multi-Stage Training DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving Xiaosong Jia*, Junqi You*, Zhiyuan Zhang*, Junchi Yan † Sch. of Computer Science Sch. of Artificial Intelligence, Shanghai Jiao Tong University * Equal Contributions † Correspondence Author https://github.com/Thinklab-SJTU/DriveTransformer/ Abstract End-to-end autonomous driving (E2E-AD) has emerged as a trend in the field of autonomous driving, promising a data-driven, scalable approach to system design. However, existing E2E-AD methods usually adopt the sequential paradigm of perception…

**Conclusion.** Conclusion A Implementation Details B Dev10 Benchmark C Limitations D Comparison of Middle Tasks E Comparison with Concurrent Parallel and Sparse based Methods F Training Stability Multi-Stage Training DriveTransformer: Unified Transformer for Scalable End-to-End Autonomous Driving Xiaosong Jia*, Junqi You*, Zhiyuan Zhang*, Junchi Yan † Sch. of Computer Science Sch. of Artificial Intelligence, Shanghai Jiao Tong University * Equal Contributions † Correspondence Author https://github.com/Thinklab-SJTU/DriveTransformer/ Abstract End-to-end autonomous driving (E2E-AD) has emerged as a trend in the field of autonomous driving, promising a data-driven, scalable approach to system design. However, existing E2E-A…

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.07656v2.md` · `raw/arxiv/2503.07656v2.fulltext.md`
