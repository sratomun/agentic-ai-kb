---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "In Prospect and Retrospect: Reflective Memory Management for Long-term Personalized Dialogue Agents"
authors: Zhen Tan, Jun Yan, I-Hung Hsu, Rujun Han et al.
url: https://arxiv.org/abs/2503.08026v2
date: 2025-03-11
citationCount: 71
influentialCitationCount: 6
velocity: 4.62
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# In Prospect and Retrospect: Reflective Memory Management for Long-term Personalized Dialogue Agents

**arXiv [2503.08026v2](https://arxiv.org/abs/2503.08026v2)** · 2025-03-11 · **71 citations** (6 influential · 4.62/mo) · Zhen Tan, Jun Yan, I-Hung Hsu, Rujun Han et al.

## Abstract
Large Language Models (LLMs) have made significant progress in open-ended dialogue, yet their inability to retain and retrieve relevant information from long-term interactions limits their effectiveness in applications requiring sustained personalization. External memory mechanisms have been proposed to address this limitation, enabling LLMs to maintain conversational continuity. However, existing approaches struggle with two key challenges. First, rigid memory granularity fails to capture the natural semantic structure of conversations, leading to fragmented and incomplete representations. Second, fixed retrieval mechanisms cannot adapt to diverse dialogue contexts and user interaction patterns. In this work, we propose Reflective Memory Management (RMM), a novel mechanism for long-term dialogue agents, integrating forward- and backward-looking reflections: (1) Prospective Reflection, which dynamically summarizes interactions across granularities-utterances, turns, and sessions-into a personalized memory bank for effective future retrieval, and (2) Retrospective Reflection, which iteratively refines the retrieval in an online reinforcement learning (RL) manner based on LLMs' cited evidence. Experiments show that RMM demonstrates consistent improvement across various metrics and benchmarks. For example, RMM shows more than 10% accuracy improvement over the baseline without memory management on the LongMemEval dataset.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Language Models (LLMs) have demonstrated remarkable capabilities in engaging in open-ended dialogue (Lee et al., 2023; Mendonça et al., 2024), yet their inherent statelessness poses a significant challenge for maintaining coherent, personalized conversations over time (Chen et al., 2024; Li et al., 2024b; Tseng et al., 2024), which are crucial across various real-world applications (e.g., customer service (Kolasani, 2023), virtual assistants (Guan et al., 2024), and education platforms (Wen et al., 2024; Zhang et al., 2024d)). As illustrated in Figure 1, effective personalization requires not only understanding the immediate context but also recalling relevant information from the user’s previous interactions (Dong et al., 2024; Whittaker et al., 2002; Williams and Hollan, 1981). The limitations with current LLMs to naturally retain and recall information from past Current Dialogue Session (Today) User I now have a headache, and the fever is gone. So the fever subsided, the cough persists, and a headache started. Considering your Agent allergy, let's explore ……

**Method / approach.** methods require white-box access to model internals, making them infeasible for 2 In Prospect and Retrospect: Reflective Memory Management for Long-term Personalized Dialogue Agents proprietary or API-based LLMs. (2) Summarization-based methods, which condense long contexts into structured events or topics for direct conditioning or retrieval (Jiang et al., 2025; Li et al., 2024a; Lu et al., 2023; Wang et al., 2023). RMM falls into this category but explicitly addresses the issue of fragmented topics arising from fixed granularity and incorporates retrospective reflection to refine the retrieval process, encouraging more coherent and contextual responses. Memory-based Personalized Dialogue Agents. The development of memory-based personalized dialogue agents has further enhanced long-term interactions by enabling systems to retain and utilize information from past conversations (Bae et al., 2022). Traditional methods Walker et al. (1997); Weizenbaum (1966) laid the groundwork for un…

**Results.** Experiments show that RMM demonstrates consistent improvement across various metrics and benchmarks. For example, RMM shows more than 10% accuracy improvement over the baseline without memory management on the LongMemEval dataset. 1. Introduction Large Language Models (LLMs) have demonstrated remarkable capabilities in engaging in open-ended dialogue (Lee et al., 2023; Mendonça et al., 2024), yet their inherent statelessness poses a significant challenge for maintaining coherent, personalized conversations over time (Chen et al., 2024; Li et al., 2024b; Tseng et al., 2024), which are crucial across various real-world applications (e.g., customer service (Kolasani, 2023), virtual assistants (Guan et al., 2024), and education platforms (Wen et al., 2024; Zhang et al., 2024d)). As illustrated in Figure 1, effective personalization requires not only understanding the immediate context but also recalling relevant information from the user’s…

**Conclusion.** conclusion of each session and consists of two key steps: memory extraction and memory update. Memory Merge Memory Addition Finished Dialogue Session … Current Memory Bank Topic Summary Raw Dialogue User is an undergrad. … User enjoys hiking. … User is 19 years old. … Retrieve and update relevant memory (if exists) Updated Memory Bank Decompose & Summarize Topic Summary Raw Dialogue Raw Dialogue User is an undergrad. … User likes hiking and running. … User likes running. … User is 19 years old. … User is allergic to eggs. … User is allergic to eggs. … Topic Summary Figure 2 | Illustration of Prospective Reflection. After each session, the agent decomposes and summarizes the session into specific topics. These…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2503.08026v2.md` · `raw/arxiv/2503.08026v2.fulltext.md`
