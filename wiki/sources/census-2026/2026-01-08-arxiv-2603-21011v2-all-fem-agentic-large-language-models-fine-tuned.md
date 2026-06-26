---
type: source
source_type: arxiv
title: "ALL-FEM: Agentic Large Language models Fine-tuned for Finite Element Methods"
authors: Rushikesh Deotale, Adithya Srinivasan, Yuan Tian, Tianyi Zhang et al.
url: https://arxiv.org/abs/2603.21011v2
date: 2026-01-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CE
tags: [coding-agents, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# ALL-FEM: Agentic Large Language models Fine-tuned for Finite Element Methods

**arXiv:** [2603.21011v2](https://arxiv.org/abs/2603.21011v2) · 2026-01-08 · cs.CE
**Authors:** Rushikesh Deotale, Adithya Srinivasan, Yuan Tian, Tianyi Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Finite element (FE) analysis guides the design and verification of nearly all manufactured objects. It is at the core of computational engineering, enabling simulation of complex physical systems, from fluids and solids to multiphysics systems. However, implementing FE codes and analyzing simulation results demands expertise across numerical analysis, continuum mechanics, and programming. Conventional Large Language Models (LLMs) can generate FE code, but they hallucinate, lack awareness of variational structures, and cannot close the loop from problem statement to a verified solution. Here, we propose ALL-FEM, an autonomous simulation system that integrates agentic AI with domain-specific, fine-tuned LLMs for FEniCS code generation across solid, fluid, and multiphysics applications. We construct a corpus of 1000+ verified FEniCS scripts by combining 500+ curated expert codes with a retrieval-augmented, multi-LLM pipeline that generates and filters codes for diverse PDEs, geometries, and boundary conditions. We used the corpus to fine-tune LLMs with 3B to 120B parameters. Our agentic framework orchestrates specialized agents, powered by fine-tuned LLMs, to formulate problems as PDEs, generate and debug code and visualize the results. We evaluated the system on 39 benchmarks that include problems of linear/nonlinear elasticity, plasticity, Newtonian/non-Newtonian flow, thermofluids, fluid-structure interaction, phase separation, and transport on moving domains. Embedded in a multi-agent workflow with runtime feedback, the best fine-tuned model (GPT OSS 120B) achieves code-level success of 71.79%, outperforming a non-agentic deployment of GPT 5 Thinking. By showing that relatively small, fine-tuned LLMs, orchestrated through agentic frameworks, can automate FE workflows, ALL-FEM offers a blueprint for autonomous simulation systems in computational science and engineering.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.21011v2)
