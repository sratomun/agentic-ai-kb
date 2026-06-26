---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Memory in the Age of AI Agents"
authors: Yuyang Hu, Shichun Liu, Yanwei Yue, Guibin Zhang et al.
url: https://arxiv.org/abs/2512.13564v2
date: 2025-12-15
citationCount: 179
influentialCitationCount: 14
velocity: 28.83
ingested: 2026-06-22
tags: [agentic-rl, agentic-rag, agent-memory, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# Memory in the Age of AI Agents

**arXiv [2512.13564v2](https://arxiv.org/abs/2512.13564v2)** · 2025-12-15 · **179 citations** (14 influential · 28.83/mo) · Yuyang Hu, Shichun Liu, Yanwei Yue, Guibin Zhang et al.

## Abstract
Memory has emerged, and will continue to remain, a core capability of foundation model-based agents. As research on agent memory rapidly expands and attracts unprecedented attention, the field has also become increasingly fragmented. Existing works that fall under the umbrella of agent memory often differ substantially in their motivations, implementations, and evaluation protocols, while the proliferation of loosely defined memory terminologies has further obscured conceptual clarity. Traditional taxonomies such as long/short-term memory have proven insufficient to capture the diversity of contemporary agent memory systems. This work aims to provide an up-to-date landscape of current agent memory research. We begin by clearly delineating the scope of agent memory and distinguishing it from related concepts such as LLM memory, retrieval augmented generation (RAG), and context engineering. We then examine agent memory through the unified lenses of forms, functions, and dynamics. From the perspective of forms, we identify three dominant realizations of agent memory, namely token-level, parametric, and latent memory. From the perspective of functions, we propose a finer-grained taxonomy that distinguishes factual, experiential, and working memory. From the perspective of dynamics, we analyze how memory is formed, evolved, and retrieved over time. To support practical development, we compile a comprehensive summary of memory benchmarks and open-source frameworks. Beyond consolidation, we articulate a forward-looking perspective on emerging research frontiers, including memory automation, reinforcement learning integration, multimodal memory, multi-agent memory, and trustworthiness issues. We hope this survey serves not only as a reference for existing work, but also as a conceptual foundation for rethinking memory as a first-class primitive in the design of future agentic intelligence.

## From the paper (full-text excerpts)
**Introduction.** Introduction 4 2 Preliminaries: Formalizing Agents and Memory 2.1 LLM-based Agent Systems . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2.2 Agent Memory Systems . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2.3 Comparing Agent Memory with Other Key Concepts . . . . . . . . . . . . . . . . . . . . . . . 2.3.1 Agent Memory vs. LLM Memory . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2.3.2 Agent Memory vs. RAG . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2.3.3 Agent Memory vs. Context Engineering . . . . . . . . . . . . . . . . . . . . . . . . . . 6 6 7 8 9 10 11 3 Form: What Carries Memory? 3.1 Token-level Memory . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.1.1 Flat Memory (1D) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.1.2 Planar Memory (2D) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.1.3 Hierarchical Memory (3D) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .…

**Method / approach.** methodological advances and therefore do not fully reflect the current breadth and complexity of the research landscape. For example, emerging directions in 2025, such as memory frameworks that distill reusable tools from past experiences (Qiu et al., 2025a,c; Zhao et al., 2025c), or memory-augmented test-time scaling methods (Zhang et al., 2025g; Suzgun et al., 2025), remain underrepresented in earlier classification schemes. ❷ Conceptual Fragmentation: With the explosive growth of memory-related studies, the concept itself has become increasingly expansive and fragmented. Researchers often find that papers claiming to study “agent memory” differ drastically in implementation, objectives, and underlying assumptions. The proliferation of diverse terminologies (declarative, episodic, semantic, parametric memory, etc.) further obscures conceptual clarity, highlighting the urgent need for a coherent taxonomy that can unify these emerging concepts. Therefore, this paper seeks to establish…

**Results.** evaluation protocols, while the proliferation of loosely defined memory terminologies has further obscured conceptual clarity. Traditional taxonomies such as long/short-term memory have proven insufficient to capture the diversity and dynamics of contemporary agent memory systems. This survey aims to provide an up-to-date and comprehensive landscape of current agent memory research. We begin by clearly delineating the scope of agent memory and distinguishing it from related concepts such as LLM memory, retrieval augmented generation (RAG), and context engineering. We then examine agent memory through the unified lenses of forms, functions, and dynamics. From the perspective of forms, we identify three dominant realizations of agent memory, namely token-level, parametric, and latent memory. From the perspective of functions, we move beyond coarse temporal categorizations and propose a finer-grained taxonomy that distinguishes factual, ex…

**Conclusion.** Conclusion 76 3 Figure 1 Overview of agent memory organized by the unified taxonomy of forms (Section 3), functions (Section 4), and dynamics (Section 5). The diagram positions memory artifacts by their dominant form and primary function. It further maps representative systems into this taxonomy to provide a consolidated landscape. 1 Introduction The past two years have witnessed the overwhelming evolution of increasingly capable large language models (LLMs) into powerful AI agents (Matarazzo and Torlone, 2025; Minaee et al., 2025; Luo et al., 2025a). These foundation-model-powered agents have demonstrated remarkable progress across diverse domains such as deep research (Xu and Peng, 2025; Zhang et al., 2025p), software engineering…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2512.13564v2.md` · `raw/arxiv/2512.13564v2.fulltext.md`
