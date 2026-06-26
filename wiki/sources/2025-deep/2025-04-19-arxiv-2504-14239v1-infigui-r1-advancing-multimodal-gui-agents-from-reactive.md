---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "InfiGUI-R1: Advancing Multimodal GUI Agents from Reactive Actors to Deliberative Reasoners"
authors: Yuhang Liu, Pengxiang Li, Congkai Xie, Xavier Hu et al.
url: https://arxiv.org/abs/2504.14239v1
date: 2025-04-19
citationCount: 122
influentialCitationCount: 13
velocity: 8.66
ingested: 2026-06-22
tags: [computer-use-agents, agent-reliability, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# InfiGUI-R1: Advancing Multimodal GUI Agents from Reactive Actors to Deliberative Reasoners

**arXiv [2504.14239v1](https://arxiv.org/abs/2504.14239v1)** · 2025-04-19 · **122 citations** (13 influential · 8.66/mo) · Yuhang Liu, Pengxiang Li, Congkai Xie, Xavier Hu et al.

## Abstract
Multimodal Large Language Models (MLLMs) have powered Graphical User Interface (GUI) Agents, showing promise in automating tasks on computing devices. Recent works have begun exploring reasoning in GUI tasks with encouraging results. However, many current approaches rely on manually designed reasoning templates, which may result in reasoning that is not sufficiently robust and adaptive for complex GUI environments. Meanwhile, some existing agents continue to operate as Reactive Actors, relying primarily on implicit reasoning that may lack sufficient depth for GUI tasks demanding planning and error recovery. We argue that advancing these agents requires a shift from reactive acting towards acting based on deliberate reasoning. To facilitate this transformation, we introduce InfiGUI-R1, an MLLM-based GUI agent developed through our Actor2Reasoner framework, a reasoning-centric, two-stage training approach designed to progressively evolve agents from Reactive Actors to Deliberative Reasoners. The first stage, Reasoning Injection, focuses on establishing a basic reasoner. We employ Spatial Reasoning Distillation to transfer cross-modal spatial reasoning capabilities from teacher models to MLLMs through trajectories with explicit reasoning steps, enabling models to integrate GUI visual-spatial information with logical reasoning before action generation. The second stage, Deliberation Enhancement, refines the basic reasoner into a deliberative one using Reinforcement Learning. This stage introduces two approaches: Sub-goal Guidance, which rewards models for generating accurate intermediate sub-goals, and Error Recovery Scenario Construction, which creates failure-and-recovery training scenarios from identified prone-to-error steps. Experimental results show InfiGUI-R1 achieves strong performance in GUI grounding and trajectory tasks. Resources at https://github.com/Reallm-Labs/InfiGUI-R1.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Multimodal LLMs 2.2 MLLM-based GUI Agents 3 Actor2Reasoner 3.1 Stage 1: Reasoning Injection 3.1.1 Pinpointing Reasoning Bottleneck Samples 3.1.2 Generating Spatial Reasoning Trajectories Spatial Information Extraction and Compression Reasoning Trajectory Generation 3.1.3 Injecting Reasoning via SFT 3.2 Stage 2: Deliberation Enhancement 3.2.1 Reinforcement Learning Setup Agent Trajectory Task Reward ( R agent subscript 𝑅 agent R_{\text{agent}} italic_R start_POSTSUBSCRIPT agent end_POSTSUBSCRIPT ): Grounding Task Rewards: Other Task Rewards ( R other subscript 𝑅 other R_{\text{other}} italic_R start_POSTSUBSCRIPT other end_POSTSUBSCRIPT ): 3.2.2 Sub-goal Guidance Sub-goal Quality Assessment. 3.2.3 Error Recovery Scenario Construction Identify Prone-to-error Steps: Constructing Recovery Scenarios: Error Escape Scenario. Back on Track Scenario. 4 Experiments 4.1 Setup Implementation Details. Training Data. Training Parameters. 4.2 Evaluation Benchmarks ScreenSpot…

**Method / approach.** methodology designed to progressively evolve GUI agents from Reactive Actors to Deliberative Reasoners. Our framework culminates in InfiGUI-R1-3B , an MLLM-based agent demonstrating enhanced reasoning and robustness. The Actor2Reasoner framework tackles two core challenges: 1) reliably injecting foundational reasoning capabilities, particularly bridging the critical cross-modal gap between visual-spatial perception and textual reasoning, to achieve the initial leap from Actor to Reasoner; and 2) refining and elevating the reasoning quality of this foundational Reasoner to instill advanced planning and reflection capabilities, ultimately reaching the Deliberative stage. The Actor2Reasoner framework unfolds in two distinct stages: • Stage 1: Reasoning Injection (Laying the Foundation for the Reasoner): This stage focuses on the pivotal transition from Actor to Reasoner. We employ Spatial Reasoning Distillation , leveraging trajectories from a powerful reasoning teacher model t…

**Results.** Experiments 4.1 Setup Implementation Details. Training Data. Training Parameters. 4.2 Evaluation Benchmarks ScreenSpot ScreenSpot-Pro: AndroidControl: 4.3 Results Performance on ScreenSpot. Performance on ScreenSpot-Pro. Performance on AndroidControl. 4.4 Visualization 5 Conclusion InfiGUI-R1: Advancing Multimodal GUI Agents from Reactive Actors to Deliberative Reasoners Yuhang Liu Zhejiang University liuyuhang@zju.edu.cn , Pengxiang Li Dalian University of Technology lipengxiang@mail.dlut.edu.cn , Congkai Xie Reallm Labs xieck13@gmail.com , Xavier Hu Zhejiang University xavier.hu.research@gmail.com , Xiaotian Han xiaotian.sky.han@gmail.com , Shengyu Zhang Zhejiang University sy˙zhang@zju.edu.cn , Hongxia Yang The Hong Kong Polytechnic University hongxia.yang@polyu.edu.hk and Fei Wu Zhejiang Uni…

**Conclusion.** Conclusion InfiGUI-R1: Advancing Multimodal GUI Agents from Reactive Actors to Deliberative Reasoners Yuhang Liu Zhejiang University liuyuhang@zju.edu.cn , Pengxiang Li Dalian University of Technology lipengxiang@mail.dlut.edu.cn , Congkai Xie Reallm Labs xieck13@gmail.com , Xavier Hu Zhejiang University xavier.hu.research@gmail.com , Xiaotian Han xiaotian.sky.han@gmail.com , Shengyu Zhang Zhejiang University sy˙zhang@zju.edu.cn , Hongxia Yang The Hong Kong Polytechnic University hongxia.yang@polyu.edu.hk and Fei Wu Zhejiang University wufei@zju.edu.cn Abstract. Multimodal Large Language Models (MLLMs) have powered Graphical U…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.14239v1.md` · `raw/arxiv/2504.14239v1.fulltext.md`
