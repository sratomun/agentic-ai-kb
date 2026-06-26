---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Towards General Agentic Intelligence via Environment Scaling"
authors: Runnan Fang, Shihao Cai, Baixuan Li, Jialong Wu et al.
url: https://arxiv.org/abs/2509.13311v1
date: 2025-09-16
citationCount: 44
influentialCitationCount: 6
velocity: 4.8
ingested: 2026-06-22
tags: [agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Towards General Agentic Intelligence via Environment Scaling

**arXiv [2509.13311v1](https://arxiv.org/abs/2509.13311v1)** · 2025-09-16 · **44 citations** (6 influential · 4.8/mo) · Runnan Fang, Shihao Cai, Baixuan Li, Jialong Wu et al.

## Abstract
Advanced agentic intelligence is a prerequisite for deploying Large Language Models in practical, real-world applications. Diverse real-world APIs demand precise, robust function-calling intelligence, which needs agents to develop these capabilities through interaction in varied environments. The breadth of function-calling competence is closely tied to the diversity of environments in which agents are trained. In this work, we scale up environments as a step towards advancing general agentic intelligence. This gives rise to two central challenges: (i) how to scale environments in a principled manner, and (ii) how to effectively train agentic capabilities from experiences derived through interactions with these environments. To address these, we design a scalable framework that automatically constructs heterogeneous environments that are fully simulated, systematically broadening the space of function-calling scenarios. We further adapt a two-phase agent fine-tuning strategy: first endowing agents with fundamental agentic capabilities, then specializing them for domain-specific contexts. Extensive experiments on agentic benchmarks, tau-bench, tau2-Bench, and ACEBench, demonstrate that our trained model, AgentScaler, significantly enhances the function-calling capability of models.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Environment Build and Scaling 2.1 Environment Automatic Build 2.2 Agentic Task Construction 3 Agent Experience Learning 3.1 Human–Agent Interplay for Experience Collection Interplay Filtering 3.2 Agentic Experience Learning Two-stage Experience Learning 4 Experiments 4.1 Setup 4.2 Experimental Results Main Results Ablation Study 5 Analysis Our synthetic data approach enables efficient knowledge transfer and strong robustness and generalization. Long-horizon tool calling remains a fundamental challenge for agentic models. 6 Related Work 6.1 Tool-Use Environments 6.2 Tool Learning 7 Conclusion Lack of Reinforcement Learning Model Scale \useunder \ul AgentScaler: Towards General Agentic Intelligence via Environment Scaling Runnan Fang ∗ , Shihao Cai ∗ , Baixuan Li ∗ , Jialong Wu ∗ \faLeaf {}^{\textsuperscript{\faLeaf}} ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Guangyu Li, Wenbiao Yin, Xinyu Wang, Xiaobin Wang, Liangcai Su, Zhen Zhang, Shibin Wu, Zhengwei Tao, Yong Jiang ( ✉ ) {}^{(\textrm{…

**Method / approach.** methods fall into two categories. The first category follows a reverse paradigm, in which user queries are generated to match each assistant function call observed at every interaction turn (Yin et al., 2025 ) , though the resulting trajectories may exhibit limited realism. The second category follows a forward paradigm, which we refer to as simulated agent–human interplay (Chen et al., 2024a ; Liu et al., 2024b ; Prabhakar et al., 2025a ; Barres et al., 2025 ; Zeng et al., 2025 ) . Such generated trajectories, however, may lack naturalness. In this category, a high-level user intent is first formulated to necessitate agent interaction. Agentic data is then constructed in a top-down manner based on this intent through human–agent interplay. Yet, the environment is not scalable: the absence of automated environment construction hinders large-scale deployment and inevitably entails some degree of manual intervention. To address these challenges, we pursue the advancement of general…

**Results.** Experiments 4.1 Setup 4.2 Experimental Results Main Results Ablation Study 5 Analysis Our synthetic data approach enables efficient knowledge transfer and strong robustness and generalization. Long-horizon tool calling remains a fundamental challenge for agentic models. 6 Related Work 6.1 Tool-Use Environments 6.2 Tool Learning 7 Conclusion Lack of Reinforcement Learning Model Scale \useunder \ul AgentScaler: Towards General Agentic Intelligence via Environment Scaling Runnan Fang ∗ , Shihao Cai ∗ , Baixuan Li ∗ , Jialong Wu ∗ \faLeaf {}^{\textsuperscript{\faLeaf}} ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Guangyu Li, Wenbiao Yin, Xinyu Wang, Xiaobin Wang, Liangcai Su, Zhen Zhang, Shibin Wu, Zhengwei Tao, Yong Jiang ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Pengjun Xie, Fei Huang, Jingren Zhou Tongyi Lab , Alibaba Group Equal contributors. \faLeaf {}^{\textsuperscript{\faLeaf}} Ji…

**Conclusion.** Conclusion Lack of Reinforcement Learning Model Scale \useunder \ul AgentScaler: Towards General Agentic Intelligence via Environment Scaling Runnan Fang ∗ , Shihao Cai ∗ , Baixuan Li ∗ , Jialong Wu ∗ \faLeaf {}^{\textsuperscript{\faLeaf}} ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Guangyu Li, Wenbiao Yin, Xinyu Wang, Xiaobin Wang, Liangcai Su, Zhen Zhang, Shibin Wu, Zhengwei Tao, Yong Jiang ( ✉ ) {}^{(\textrm{{\char 0\relax}})} , Pengjun Xie, Fei Huang, Jingren Zhou Tongyi Lab , Alibaba Group Equal contributors. \faLeaf {}^{\textsuperscript{\faLeaf}} Jialong Wu (wujialongml@gmail.com) is project leader. ✉ {}^{\textrm{{\char 0\relax}}} yongjiang.yj@alibaba-inc.com Towards General Agentic Intelligence via Environm…

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.13311v1.md` · `raw/arxiv/2509.13311v1.fulltext.md`
