---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AlphaEvolve: A coding agent for scientific and algorithmic discovery"
authors: Alexander Novikov, Ngân Vũ, Marvin Eisenberger, Emilien Dupont et al.
url: https://arxiv.org/abs/2506.13131v1
date: 2025-06-16
citationCount: 559
influentialCitationCount: 78
velocity: 45.87
ingested: 2026-06-22
tags: [coding-agents, self-evolving-agents, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# AlphaEvolve: A coding agent for scientific and algorithmic discovery

**arXiv [2506.13131v1](https://arxiv.org/abs/2506.13131v1)** · 2025-06-16 · **559 citations** (78 influential · 45.87/mo) · Alexander Novikov, Ngân Vũ, Marvin Eisenberger, Emilien Dupont et al.

**Significance:** DeepMind's evolutionary coding agent; proof that agents can discover novel algorithms, not just apply them.

## Abstract
In this white paper, we present AlphaEvolve, an evolutionary coding agent that substantially enhances capabilities of state-of-the-art LLMs on highly challenging tasks such as tackling open scientific problems or optimizing critical pieces of computational infrastructure. AlphaEvolve orchestrates an autonomous pipeline of LLMs, whose task is to improve an algorithm by making direct changes to the code. Using an evolutionary approach, continuously receiving feedback from one or more evaluators, AlphaEvolve iteratively improves the algorithm, potentially leading to new scientific and practical discoveries. We demonstrate the broad applicability of this approach by applying it to a number of important computational problems. When applied to optimizing critical components of large-scale computational stacks at Google, AlphaEvolve developed a more efficient scheduling algorithm for data centers, found a functionally equivalent simplification in the circuit design of hardware accelerators, and accelerated the training of the LLM underpinning AlphaEvolve itself. Furthermore, AlphaEvolve discovered novel, provably correct algorithms that surpass state-of-the-art solutions on a spectrum of problems in mathematics and computer science, significantly expanding the scope of prior automated discovery methods (Romera-Paredes et al., 2023). Notably, AlphaEvolve developed a search algorithm that found a procedure to multiply two $4 \times 4$ complex-valued matrices using $48$ scalar multiplications; offering the first improvement, after 56 years, over Strassen's algorithm in this setting. We believe AlphaEvolve and coding agents like it can have a significant impact in improving solutions of problems across many areas of science and computation.

## From the paper (full-text excerpts)
**Introduction.** Introduction Discovering new high-value knowledge, such as making a novel scientific discovery or developing a commercially valuable algorithm, generally requires a prolonged process of ideation, exploration, backtracking on unpromising hypotheses, experimentation, and validation. There has been much recent interest in using large language models (LLMs) to automate significant parts of this process. Hopes of success here are driven by the breathtaking power of recent LLMs [32, 76], which can enhance their capabilities using test-time compute, and the rise of agents that combine language generation and action [88, 114]. These advances have improved performance across a range of established benchmarks and accelerated discoveryoriented tasks like hypothesis generation [34] and experiment design [7, 43]. However, getting LLM pipelines all the way to making entirely new scientific or practical discoveries remains challenging. In this white paper, we present an LLM code superoptimization agent, called AlphaEvolve, that takes on this challenge using a combination of evolutionary computation…

**Method / approach.** methods with coding LLMs has been previously explored in various specialized settings. In particular, AlphaEvolve is a substantial enhancement of FunSearch [83] (see Table 1), which used LLM-guided evolution to discover heuristics in order to construct novel mathematical objects or to drive the operation of online algorithms. Also, related approaches have been used in tasks such as discovering policies for simulated robots [57], symbolic regression [35, 89], and the synthesis of heuristic functions for combinatorial optimization [63]. In contrast to these systems, AlphaEvolve leverages state-of-the-art (SOTA) LLMs to evolve large pieces of code that implement complex algorithms spanning multiple functions and components. As a result, it is able to go significantly beyond its predecessors in scale and generality. FunSearch [83] AlphaEvolve evolves single function evolves up to 10-20 lines of code evolves code in Python needs fast evaluation (≤ 20min on 1 CPU) millions of LLM samples…

**Results.** experimentation, and validation. There has been much recent interest in using large language models (LLMs) to automate significant parts of this process. Hopes of success here are driven by the breathtaking power of recent LLMs [32, 76], which can enhance their capabilities using test-time compute, and the rise of agents that combine language generation and action [88, 114]. These advances have improved performance across a range of established benchmarks and accelerated discoveryoriented tasks like hypothesis generation [34] and experiment design [7, 43]. However, getting LLM pipelines all the way to making entirely new scientific or practical discoveries remains challenging. In this white paper, we present an LLM code superoptimization agent, called AlphaEvolve, that takes on this challenge using a combination of evolutionary computation and LLM-based code generation. AlphaEvolve focuses on the broad spectrum of scientific and enginee…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[alphaevolve]]
- **Raw:** `raw/arxiv/2506.13131v1.md` · `raw/arxiv/2506.13131v1.fulltext.md`
