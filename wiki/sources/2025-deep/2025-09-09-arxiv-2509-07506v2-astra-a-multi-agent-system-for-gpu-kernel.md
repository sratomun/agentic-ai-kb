---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Astra: A Multi-Agent System for GPU Kernel Performance Optimization"
authors: Anjiang Wei, Tianran Sun, Yogesh Seenichamy, Hang Song et al.
url: https://arxiv.org/abs/2509.07506v2
date: 2025-09-09
citationCount: 39
influentialCitationCount: 1
velocity: 4.15
ingested: 2026-06-22
tags: [coding-agents, agent-memory, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Astra: A Multi-Agent System for GPU Kernel Performance Optimization

**arXiv [2509.07506v2](https://arxiv.org/abs/2509.07506v2)** · 2025-09-09 · **39 citations** (1 influential · 4.15/mo) · Anjiang Wei, Tianran Sun, Yogesh Seenichamy, Hang Song et al.

## Abstract
GPU kernel optimization has long been a central challenge at the intersection of high-performance computing and machine learning. Efficient kernels are crucial for accelerating large language model (LLM) training and serving, yet attaining high performance typically requires extensive manual tuning. Compiler-based systems reduce some of this burden, but still demand substantial manual design and engineering effort. Recently, researchers have explored using LLMs for GPU kernel generation, though prior work has largely focused on translating high-level PyTorch modules into CUDA code. In this work, we introduce Astra, the first LLM-based multi-agent system for GPU kernel optimization. Unlike previous approaches, Astra starts from existing CUDA implementations extracted from SGLang, a widely deployed framework for serving LLMs, rather than treating PyTorch modules as the specification. Within Astra, specialized LLM agents collaborate through iterative code generation, testing, profiling, and planning to produce kernels that are both correct and high-performance. On kernels from SGLang, Astra achieves an average speedup of 1.32x using zero-shot prompting with OpenAI o4-mini. A detailed case study further demonstrates that LLMs can autonomously apply loop transformations, optimize memory access patterns, exploit CUDA intrinsics, and leverage fast math operations to yield substantial performance gains. Our work highlights multi-agent LLM systems as a promising new paradigm for GPU kernel optimization. Our code is publicly available at https://github.com/Anjiang-Wei/Astra.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Multi-Agent Systems Compiler and Learning-Based Approaches to GPU Kernel Optimization LLM-Driven Approaches to High-Performance Code Generation 3 Method 3.1 Task Definition Correctness. Performance. 3.2 Multi-Agent System Agent Roles. Algorithm. Pre-Processing and Post-Processing. 4 Experimental Setup Metrics. Kernels. Performance Measurement. Implementation. 5 Results 5.1 Main Results Correctness. Performance. 5.2 Comparison with Single-Agent Approach Setup of Single-Agent Method. Performance. 5.3 Case Studies Kernel 1: merge_attn_states_lse Kernel 2: fused_add_rmsnorm Kernel 3: silu_and_mul 6 Discussion 6.1 Impact of Tensor Shapes on Performance Speedup 6.2 Limitations and Future Work 7 Conclusion \workshoptitle Fourth Workshop on Deep Learning for Code Astra: A Multi-Agent System for GPU Kernel Performance Optimization Anjiang Wei 1 Tianran Sun 2 Yogesh Seenichamy 1 Hang Song 1 Anne Ouyang 1 Azalia Mirhoseini 1 Ke Wang 3 Alex Aiken 1 1 S…

**Method / approach.** Method 3.1 Task Definition Correctness. Performance. 3.2 Multi-Agent System Agent Roles. Algorithm. Pre-Processing and Post-Processing. 4 Experimental Setup Metrics. Kernels. Performance Measurement. Implementation. 5 Results 5.1 Main Results Correctness. Performance. 5.2 Comparison with Single-Agent Approach Setup of Single-Agent Method. Performance. 5.3 Case Studies Kernel 1: merge_attn_states_lse Kernel 2: fused_add_rmsnorm Kernel 3: silu_and_mul 6 Discussion 6.1 Impact of Tensor Shapes on Performance Speedup 6.2 Limitations and Future Work 7 Conclusion \workshoptitle Fourth Workshop on Deep Learning for Code Astra: A Multi-Agent System for GPU Kernel Performance Optimization Anjiang Wei 1 Tianran Sun 2 Yogesh Seenichamy 1 Hang Song 1 Anne Ouyang 1 Azalia Mirhoseini 1 Ke Wang 3 Alex Aiken 1 1 Stanford University 2 Shanghai Jiao Tong University 3 Nanjing University Correspo…

**Results.** Experimental Setup Metrics. Kernels. Performance Measurement. Implementation. 5 Results 5.1 Main Results Correctness. Performance. 5.2 Comparison with Single-Agent Approach Setup of Single-Agent Method. Performance. 5.3 Case Studies Kernel 1: merge_attn_states_lse Kernel 2: fused_add_rmsnorm Kernel 3: silu_and_mul 6 Discussion 6.1 Impact of Tensor Shapes on Performance Speedup 6.2 Limitations and Future Work 7 Conclusion \workshoptitle Fourth Workshop on Deep Learning for Code Astra: A Multi-Agent System for GPU Kernel Performance Optimization Anjiang Wei 1 Tianran Sun 2 Yogesh Seenichamy 1 Hang Song 1 Anne Ouyang 1 Azalia Mirhoseini 1 Ke Wang 3 Alex Aiken 1 1 Stanford University 2 Shanghai Jiao Tong University 3 Nanjing University Correspondence to: anjiang@cs.stanford.edu Abstract GPU kernel optimization has long been a central challenge at th…

**Conclusion.** Conclusion \workshoptitle Fourth Workshop on Deep Learning for Code Astra: A Multi-Agent System for GPU Kernel Performance Optimization Anjiang Wei 1 Tianran Sun 2 Yogesh Seenichamy 1 Hang Song 1 Anne Ouyang 1 Azalia Mirhoseini 1 Ke Wang 3 Alex Aiken 1 1 Stanford University 2 Shanghai Jiao Tong University 3 Nanjing University Correspondence to: anjiang@cs.stanford.edu Abstract GPU kernel optimization has long been a central challenge at the intersection of high-performance computing and machine learning. Efficient kernels are crucial for accelerating large language model (LLM) training and serving, yet attaining high performance typically requires extensive manual tuning. Compiler-based systems reduce…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.07506v2.md` · `raw/arxiv/2509.07506v2.fulltext.md`
