---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ACON: Optimizing Context Compression for Long-horizon LLM Agents"
authors: Minki Kang, Wei-Ning Chen, Dongge Han, Huseyin A. Inan et al.
url: https://arxiv.org/abs/2510.00615v3
date: 2025-10-01
citationCount: 51
influentialCitationCount: 4
velocity: 5.88
ingested: 2026-06-22
tags: [agent-reliability, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# ACON: Optimizing Context Compression for Long-horizon LLM Agents

**arXiv [2510.00615v3](https://arxiv.org/abs/2510.00615v3)** · 2025-10-01 · **51 citations** (4 influential · 5.88/mo) · Minki Kang, Wei-Ning Chen, Dongge Han, Huseyin A. Inan et al.

## Abstract
Large language models (LLMs) are increasingly deployed as agents in dynamic real-world environments, where success depends on maintaining precise records of actions and observations. However, the resulting unbounded context growth in long-horizon agentic tasks makes two critical bottlenecks: prohibitive inference memory costs and reasoning degradation due to irrelevant information. Existing compression methods fail to fully address this, often relying on brittle heuristics or requiring parameter updates impractical for proprietary or large-scale LLMs. We introduce Agent Context Optimization (ACON), a unified framework that optimally compresses both observations and history into concise, informative representations. Distinct from prior works, ACON employs an optimization in natural language space: it iteratively refines compression guidelines based on failure analysis of the agent, ensuring critical state information is preserved without model fine-tuning. To further minimize computational overhead, we distill the optimized compressor into smaller models. Experiments on AppWorld, OfficeBench, and Multi-objective QA demonstrate that ACON reduces peak token usage by 26-54% while improving task success over existing compression baselines. Notably, it enables smaller LMs to function effectively as long-horizon agents, achieving up to 46% performance improvement by mitigating context distraction. Our code is available at https://github.com/microsoft/acon.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works Long-horizon LLM agents. Context compression for LLMs. 3 Agent Context Optimization ( Acon ) 3.1 Problem Formulation Task. Cost function for context. 3.2 History Observation Compression with LLMs History compression. Latest observation compression. Optimization objective. Challenges. 3.3 Optimizing Compression Guidelines 3.4 Distilling Context Compression into Small Models 4 Experiments 4.1 Experimental Setup Benchmarks Metrics. Baselines. Our Methods. 4.2 Overall performance and token efficiency 4.3 Compressor distillation 4.4 Acon for distilled small agents 4.5 Analysis Compression threshold: moderate value yields the best trade-off. Prompt optimizer: o3 + contrastive feedback works best. Optimization cost: practical and lightweight. API cost analysis of compressors across different models. Practical efficiency trade-off. 5 Conclusion Limitations and Future Work. References A Limitations Future Works Scope of empirical evaluation. Real-world deployability…

**Method / approach.** Methods. 4.2 Overall performance and token efficiency 4.3 Compressor distillation 4.4 Acon for distilled small agents 4.5 Analysis Compression threshold: moderate value yields the best trade-off. Prompt optimizer: o3 + contrastive feedback works best. Optimization cost: practical and lightweight. API cost analysis of compressors across different models. Practical efficiency trade-off. 5 Conclusion Limitations and Future Work. References A Limitations Future Works Scope of empirical evaluation. Real-world deployability Convergence of natural language space optimization Distillation gap and data scalability Latency and KV-cache dynamics B Experimental Setup Details B.1 Datasets AppWorld (Trivedi et al. , 2024 ) . OfficeBench (Wang et al. , 2024b ) . 8-Objective QA (Zhou et al. , 2025 ) . B.2 Evaluation Metrics Peak tokens. Dependency. API Cost. B.3 Implementation Details Hyperparameters API Inference.…

**Results.** Experiments 4.1 Experimental Setup Benchmarks Metrics. Baselines. Our Methods. 4.2 Overall performance and token efficiency 4.3 Compressor distillation 4.4 Acon for distilled small agents 4.5 Analysis Compression threshold: moderate value yields the best trade-off. Prompt optimizer: o3 + contrastive feedback works best. Optimization cost: practical and lightweight. API cost analysis of compressors across different models. Practical efficiency trade-off. 5 Conclusion Limitations and Future Work. References A Limitations Future Works Scope of empirical evaluation. Real-world deployability Convergence of natural language space optimization Distillation gap and data scalability Latency and KV-cache dynamics B Experimental Setup Details B.1 Datasets AppWorld (Trivedi et al. , 2024 ) . OfficeBench (Wang et al. , 2024b ) . 8-Objective QA (Zhou et al. , 2025 ) . B.2…

**Conclusion.** Conclusion Limitations and Future Work. References A Limitations Future Works Scope of empirical evaluation. Real-world deployability Convergence of natural language space optimization Distillation gap and data scalability Latency and KV-cache dynamics B Experimental Setup Details B.1 Datasets AppWorld (Trivedi et al. , 2024 ) . OfficeBench (Wang et al. , 2024b ) . 8-Objective QA (Zhou et al. , 2025 ) . B.2 Evaluation Metrics Peak tokens. Dependency. API Cost. B.3 Implementation Details Hyperparameters API Inference. Compression. Prompt Optimization. Baselines Compressor Agent Distillation C Additional Results C.1 Results with different agent models Experiments with…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2510.00615v3.md` · `raw/arxiv/2510.00615v3.fulltext.md`
