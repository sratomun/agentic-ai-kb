---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Assemble Your Crew: Automatic Multi-agent Communication Topology Design via Autoregressive Graph Generation"
authors: Shiyuan Li, Yixin Liu, Qingsong Wen, Chengqi Zhang et al.
url: https://arxiv.org/abs/2507.18224v4
date: 2025-07-24
citationCount: 44
influentialCitationCount: 6
velocity: 4.02
ingested: 2026-06-22
tags: [multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Assemble Your Crew: Automatic Multi-agent Communication Topology Design via Autoregressive Graph Generation

**arXiv [2507.18224v4](https://arxiv.org/abs/2507.18224v4)** · 2025-07-24 · **44 citations** (6 influential · 4.02/mo) · Shiyuan Li, Yixin Liu, Qingsong Wen, Chengqi Zhang et al.

## Abstract
Multi-agent systems (MAS) based on large language models (LLMs) have emerged as a powerful solution for dealing with complex problems across diverse domains. The effectiveness of MAS is critically dependent on its collaboration topology, which has become a focal point for automated design research. However, existing approaches are fundamentally constrained by their reliance on a template graph modification paradigm with a predefined set of agents and hard-coded interaction structures, significantly limiting their adaptability to task-specific requirements. To address these limitations, we reframe MAS design as a conditional autoregressive graph generation task, where both the system composition and structure are designed jointly. We propose ARG-Designer, a novel autoregressive model that operationalizes this paradigm by constructing the collaboration graph from scratch. Conditioned on a natural language task query, ARG-Designer sequentially and dynamically determines the required number of agents, selects their appropriate roles from an extensible pool, and establishes the optimal communication links between them. This generative approach creates a customized topology in a flexible and extensible manner, precisely tailored to the unique demands of different tasks. Extensive experiments across six diverse benchmarks demonstrate that ARG-Designer not only achieves state-of-the-art performance but also enjoys significantly greater token efficiency and enhanced extensibility. The source code of ARG-Designer is available at https://github.com/Shiy-Li/ARG-Designer.

## From the paper (full-text excerpts)
**Introduction.** Introduction Problem Formulation ARG-Designer for MAS Topology Design Model Architecture Training and Inference Strategy Data Construction of Curriculum Learning. Model Training. Inference. Experiments Experimental Setting Experimental Results Related Work Autoregressive Graph Generation LLM-based Multi-Agent System Conclusion Assemble Your Crew: Automatic Multi-agent Communication Topology Design via Autoregressive Graph Generation Shiyuan Li 1 , Yixin Liu 1 , Qingsong Wen 2 , Chengqi Zhang 3 , Shirui Pan 1 Corresponding Author Abstract Multi-agent systems (MAS) based on large language models (LLMs) have emerged as a powerful solution for dealing with complex problems across diverse domains. The effectiveness of MAS is critically dependent on its collaboration topology, which has become a focal point for automated design research. However, existing approaches are fundamentally constrained by their reliance on a template graph modification paradigm with a predefined set of agents and hard-coded interaction structures, significant…

**Method / approach.** methods often follow a shared paradigm: template graph modification (Fig. 1 a). That is, they typically start from a fixed communication template based on a predefined set of agents and hard-coded interaction structures, and apply learnable adjustments, such as edge reweighting or pruning, to adapt the topology to specific tasks ( zhang2024cut ; zhang2024g ) . Despite offering reasonable adaptability in constrained settings, this paradigm exhibits two inherent limitations. Limitation 1: Redundant Composition . To ensure structural flexibility, template graphs are often initialized with numerous agent roles and densely connected edges, many of which are unnecessary for a specific task. Even with pruning mechanisms, irrelevant agents or connections may be retained in the learned task-specific topology, leading not only to reduced efficiency but also to potential sub-optimal decision-making during execution. Limitation 2: Limited Extensibility . In the fast-evolving field of LLM-based…

**Results.** Experiments Experimental Setting Experimental Results Related Work Autoregressive Graph Generation LLM-based Multi-Agent System Conclusion Assemble Your Crew: Automatic Multi-agent Communication Topology Design via Autoregressive Graph Generation Shiyuan Li 1 , Yixin Liu 1 , Qingsong Wen 2 , Chengqi Zhang 3 , Shirui Pan 1 Corresponding Author Abstract Multi-agent systems (MAS) based on large language models (LLMs) have emerged as a powerful solution for dealing with complex problems across diverse domains. The effectiveness of MAS is critically dependent on its collaboration topology, which has become a focal point for automated design research. However, existing approaches are fundamentally constrained by their reliance on a template graph modification paradigm with a predefined set of agents and hard-coded interaction structures, significantly limiting their adaptability to task-specific requirements. To…

**Conclusion.** Conclusion Assemble Your Crew: Automatic Multi-agent Communication Topology Design via Autoregressive Graph Generation Shiyuan Li 1 , Yixin Liu 1 , Qingsong Wen 2 , Chengqi Zhang 3 , Shirui Pan 1 Corresponding Author Abstract Multi-agent systems (MAS) based on large language models (LLMs) have emerged as a powerful solution for dealing with complex problems across diverse domains. The effectiveness of MAS is critically dependent on its collaboration topology, which has become a focal point for automated design research. However, existing approaches are fundamentally constrained by their reliance on a template graph modification paradigm with a predefined set of agents and hard-coded interaction structures, significantly limiting…

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.18224v4.md` · `raw/arxiv/2507.18224v4.fulltext.md`
