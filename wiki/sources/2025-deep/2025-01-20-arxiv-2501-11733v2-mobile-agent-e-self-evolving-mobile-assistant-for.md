---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Mobile-Agent-E: Self-Evolving Mobile Assistant for Complex Tasks"
authors: Zhenhailong Wang, Haiyang Xu, Junyang Wang, Xi Zhang et al.
url: https://arxiv.org/abs/2501.11733v2
date: 2025-01-20
citationCount: 114
influentialCitationCount: 13
velocity: 6.7
ingested: 2026-06-22
tags: [computer-use-agents, self-evolving-agents, agent-memory, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# Mobile-Agent-E: Self-Evolving Mobile Assistant for Complex Tasks

**arXiv [2501.11733v2](https://arxiv.org/abs/2501.11733v2)** · 2025-01-20 · **114 citations** (13 influential · 6.7/mo) · Zhenhailong Wang, Haiyang Xu, Junyang Wang, Xi Zhang et al.

## Abstract
Smartphones have become indispensable in modern life, yet navigating complex tasks on mobile devices often remains frustrating. Recent advancements in large multimodal model (LMM)-based mobile agents have demonstrated the ability to perceive and act in mobile environments. However, current approaches face significant limitations: they fall short in addressing real-world human needs, struggle with reasoning-intensive and long-horizon tasks, and lack mechanisms to learn and improve from prior experiences. To overcome these challenges, we introduce Mobile-Agent-E, a hierarchical multi-agent framework capable of self-evolution through past experience. By hierarchical, we mean an explicit separation of high-level planning and low-level action execution. The framework comprises a Manager, responsible for devising overall plans by breaking down complex tasks into subgoals, and four subordinate agents--Perceptor, Operator, Action Reflector, and Notetaker--which handle fine-grained visual perception, immediate action execution, error verification, and information aggregation, respectively. Mobile-Agent-E also features a novel self-evolution module which maintains a persistent long-term memory comprising Tips and Shortcuts. Tips are general guidance and lessons learned from prior tasks on how to effectively interact with the environment. Shortcuts are reusable, executable sequences of atomic operations tailored for specific subroutines. The inclusion of Tips and Shortcuts facilitates continuous refinement in performance and efficiency. Alongside this framework, we introduce Mobile-Eval-E, a new benchmark featuring complex mobile tasks requiring long-horizon, multi-app interactions. Empirical results show that Mobile-Agent-E achieves a 22% absolute improvement over previous state-of-the-art approaches across three foundation model backbones. Project page: https://x-plug.github.io/MobileAgent.

## From the paper (full-text excerpts)
**Introduction.** Introduction 3 Mobile-Agent-E 3.1 Hierachical Multi-Agent Framework Manager ( 𝒜 M subscript 𝒜 𝑀 \mathcal{A}_{M} caligraphic_A start_POSTSUBSCRIPT italic_M end_POSTSUBSCRIPT ): High-level planning. Perceptor ( 𝒜 P subscript 𝒜 𝑃 \mathcal{A}_{P} caligraphic_A start_POSTSUBSCRIPT italic_P end_POSTSUBSCRIPT ): Fine-grained visual perception. Operator ( 𝒜 O subscript 𝒜 𝑂 \mathcal{A}_{O} caligraphic_A start_POSTSUBSCRIPT italic_O end_POSTSUBSCRIPT ): Low-level action decisions. Action Reflector ( 𝒜 R subscript 𝒜 𝑅 \mathcal{A}_{R} caligraphic_A start_POSTSUBSCRIPT italic_R end_POSTSUBSCRIPT ): Reflection on the action outcome. Notetaker ( 𝒜 N subscript 𝒜 𝑁 \mathcal{A}_{N} caligraphic_A start_POSTSUBSCRIPT italic_N end_POSTSUBSCRIPT ): Information aggregation. 3.2 Self-Evolution Module 4 Experiments 4.1 A More Challenging Benchmark: Mobile-Eval-E 4.2 Metrics with Better Human Alignment 4.3 Evaluating Self-Evolving Mobile Agents 4.4 Models Baselines. Backbones. Perceptor Implementation in Mobile-Agent-E. 5 Results 5.1 Evaluation on Performance…

**Method / approach.** methods achieving only about 50–70% of human satisfaction. Empirical results show that Mobile-Agent-E achieves an average absolute gain of 22.1% over previous state-of-the-art approaches across three different foundation model backbones. Mobile-Agent-E also demonstrates promising self-evolution behavior in both performance and efficiency, resulting in a 6.5% absolute improvement compared to no evolution. The incorporation of Shortcuts further reduces the computational overhead, achieving speeds comparable to prior models while delivering significantly better performance. Additionally, we provide a comprehensive analysis of various aspects of self-evolution’s impact and outline directions for future work. Figure 2: An overview of the Mobile-Agent-E framework, where the Manager, Perceptor ( 𝒜 P subscript 𝒜 𝑃 \mathcal{A}_{P} caligraphic_A start_POSTSUBSCRIPT italic_P end_POSTSUBSCRIPT ), Operator, Action Reflector, and Notetaker are involved in the main agent loop for each task, wh…

**Results.** Experiments 4.1 A More Challenging Benchmark: Mobile-Eval-E 4.2 Metrics with Better Human Alignment 4.3 Evaluating Self-Evolving Mobile Agents 4.4 Models Baselines. Backbones. Perceptor Implementation in Mobile-Agent-E. 5 Results 5.1 Evaluation on Performance Comparison with state-of-the-art. Varying reasoning backbones. 5.2 Evaluation on Efficiency 5.3 Further Analysis Progressive impact of self-evolution over time. Shortcut reduces computational overhead. Unique impact from Tips. 5.4 Case Study: A Closed-Loop Self-Evolving Agent 6 Related Work 6.1 GUI Agents 6.2 Self-Evolution in Foundation Models 7 Conclusion and Future Work A Full Trajectory Comparison Example with Previous SOTA B Error Recovery with Escalation to Manager C Remaining Limitations C.1 Misuse of Shortcuts due to Incorrect Perception of Phone State C.2 Errors and Imperfections in Self-Evolved Sh…

**Conclusion.** Conclusion and Future Work A Full Trajectory Comparison Example with Previous SOTA B Error Recovery with Escalation to Manager C Remaining Limitations C.1 Misuse of Shortcuts due to Incorrect Perception of Phone State C.2 Errors and Imperfections in Self-Evolved Shortcuts D All Tasks in Mobile-Eval-E Benchmark E Atomic Operation Space F Full list of Self-Evolved Shortcuts G Full list of Self-Evolved Tips Mobile-Agent-E: Self-Evolving Mobile Assistant for Complex Tasks Zhenhailong Wang * Haiyang Xu * Junyang Wang Xi Zhang Ming Yan Ji Zhang Fei Huang Heng Ji * Abstract Smartphones have become indispensable in modern life, yet navigating complex, multi-step tasks on mobile devices often remains…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2501.11733v2.md` · `raw/arxiv/2501.11733v2.fulltext.md`
