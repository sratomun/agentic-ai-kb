---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live"
authors: Hanchen Li, Runyuan He, Qiuyang Mang, Qizheng Zhang et al.
url: https://arxiv.org/abs/2511.02230v6
date: 2025-11-04
citationCount: 31
influentialCitationCount: 5
velocity: 4.1
ingested: 2026-06-22
tags: [coding-agents, agent-memory, tool-use, agentic-ai, arxiv, 2025, cited]
---

# Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live

**arXiv [2511.02230v6](https://arxiv.org/abs/2511.02230v6)** · 2025-11-04 · **31 citations** (5 influential · 4.1/mo) · Hanchen Li, Runyuan He, Qiuyang Mang, Qizheng Zhang et al.

## Abstract
KV cache management is essential for efficient LLM inference. To maximize utilization, existing inference engines evict finished requests' KV cache if new requests are waiting. This policy breaks for agentic workloads, which interleave LLM calls with tools, introducing pauses that prevent effective KV reuse across turns. Since many tool calls have much shorter durations than human response multi-turn chatbot, it would be promising to retain the KV cache in during these tools. However, many challenges remain. First, we need to consider both the potential cost of recomputation or reloading (if offloading enabled) as well as the increasing queueing delays after eviction from GPU. Second, due to the internal variance of tool call durations, the method needs to remain robust under limited predictability of tool call durations. We present Continuum, a serving system to optimize job completion time for multi-turn agent workloads by introducing time-to-live mechanism for KV cache retention. For requests that generate tool calls, Continuum selectively pins the KV cache in GPU memory with a time-to-live value determined by the reload cost and potential queueing delay induced by eviction. When the TTL expires, the KV cache can be automatically evicted to free up GPU memory, providing robust performance under edge cases. When combined with program-level first-come-first-serve, Continuum preserves multi-turn continuity, and reduces delay for agentic workflows. Evaluations on real-world agents (SWE-Bench, BFCL, OpenHand) with Llama-3.1 8B/70B, Gemma-3 12B, and GLM-4.5 355B shows that Continuum improves the average job completion times by over 8x while improving throughput.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background 2.1 ReAct Paradigm for Agents 2.2 Limitations of Existing Methods 3 Motivation 3.1 Agentic Traces 3.2 Challenges for Agentic Workloads 4 Continuum Scheduling Algorithm 4.1 Utility Model Cost Estimation. Benefit Estimation. 4.2 Setting the TTL Value Cold-start Handling. 4.3 Scheduling Priority 5 Continuum System Design 5.1 Tool Call Handler 5.2 Efficient Pin with TTL in Scheduler 5.3 Implementation 6 Evaluation 6.1 Setup 6.2 End-to-End Experiments 6.3 Sensitivity Analysis 6.4 Ablation Studies and Microbenchmarking 7 Related Work 8 Conclusion References A Tool Call Parser Implementation Example B More Function Call Examples C Extended Discussions of Related Work C.1 Novel Tool-Calling Styles C.2 Model Architecture D Limitations and Future Work License: CC BY 4.0 arXiv:2511.02230v6 [cs.OS] 25 May 2026 Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live Hanchen Li ∗1 , Runyuan He ∗1 , Qiuyang Mang 1 , Qizheng Zhang 2 , Huanzhi…

**Method / approach.** Methods 3 Motivation 3.1 Agentic Traces 3.2 Challenges for Agentic Workloads 4 Continuum Scheduling Algorithm 4.1 Utility Model Cost Estimation. Benefit Estimation. 4.2 Setting the TTL Value Cold-start Handling. 4.3 Scheduling Priority 5 Continuum System Design 5.1 Tool Call Handler 5.2 Efficient Pin with TTL in Scheduler 5.3 Implementation 6 Evaluation 6.1 Setup 6.2 End-to-End Experiments 6.3 Sensitivity Analysis 6.4 Ablation Studies and Microbenchmarking 7 Related Work 8 Conclusion References A Tool Call Parser Implementation Example B More Function Call Examples C Extended Discussions of Related Work C.1 Novel Tool-Calling Styles C.2 Model Architecture D Limitations and Future Work License: CC BY 4.0 arXiv:2511.02230v6 [cs.OS] 25 May 2026 Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live Hanchen Li ∗1 , Runyuan He ∗1 , Qiuyang Mang 1 , Qizheng Zhang 2 , H…

**Results.** Experiments 6.3 Sensitivity Analysis 6.4 Ablation Studies and Microbenchmarking 7 Related Work 8 Conclusion References A Tool Call Parser Implementation Example B More Function Call Examples C Extended Discussions of Related Work C.1 Novel Tool-Calling Styles C.2 Model Architecture D Limitations and Future Work License: CC BY 4.0 arXiv:2511.02230v6 [cs.OS] 25 May 2026 Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live Hanchen Li ∗1 , Runyuan He ∗1 , Qiuyang Mang 1 , Qizheng Zhang 2 , Huanzhi Mao 1 , Xiaokun Chen 3 , Hangrui Zhou 4 , Alvin Cheung 1 , Joseph Gonzalez 1 , Ion Stoica 1 1 UC Berkeley 2 Stanford University 3 Tensormesh 4 Tsinghua University Abstract KV cache management is essential for efficient LLM inference. To maximize utilization, existing inference engines evict finished requests’ KV cache if new requests are waiting. This p…

**Conclusion.** Conclusion References A Tool Call Parser Implementation Example B More Function Call Examples C Extended Discussions of Related Work C.1 Novel Tool-Calling Styles C.2 Model Architecture D Limitations and Future Work License: CC BY 4.0 arXiv:2511.02230v6 [cs.OS] 25 May 2026 Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live Hanchen Li ∗1 , Runyuan He ∗1 , Qiuyang Mang 1 , Qizheng Zhang 2 , Huanzhi Mao 1 , Xiaokun Chen 3 , Hangrui Zhou 4 , Alvin Cheung 1 , Joseph Gonzalez 1 , Ion Stoica 1 1 UC Berkeley 2 Stanford University 3 Tensormesh 4 Tsinghua University Abstract KV cache management is essential for efficient LLM inference. To maximize utilization, ex…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]] · [[bfcl]]
- **Raw:** `raw/arxiv/2511.02230v6.md` · `raw/arxiv/2511.02230v6.fulltext.md`
