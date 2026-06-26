---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Universal Actions for Enhanced Embodied Foundation Models"
authors: Jinliang Zheng, Jianxiong Li, Dongxiu Liu, Yinan Zheng et al.
url: https://arxiv.org/abs/2501.10105v2
date: 2025-01-17
citationCount: 81
influentialCitationCount: 6
velocity: 4.73
ingested: 2026-06-22
tags: [embodied-agents, arxiv, 2025, cited]
---

# Universal Actions for Enhanced Embodied Foundation Models

**arXiv [2501.10105v2](https://arxiv.org/abs/2501.10105v2)** · 2025-01-17 · **81 citations** (6 influential · 4.73/mo) · Jinliang Zheng, Jianxiong Li, Dongxiu Liu, Yinan Zheng et al.

## Abstract
Training on diverse, internet-scale data is a key factor in the success of recent large foundation models. Yet, using the same recipe for building embodied agents has faced noticeable difficulties. Despite the availability of many crowd-sourced embodied datasets, their action spaces often exhibit significant heterogeneity due to distinct physical embodiment and control interfaces for different robots, causing substantial challenges in developing embodied foundation models using cross-domain data. In this paper, we introduce UniAct, a new embodied foundation modeling framework operating in a Universal Action Space. Our learned universal actions capture the generic atomic behaviors across diverse robots by exploiting their shared structural features, and enable enhanced cross-domain data utilization and cross-embodiment generalizations by eliminating the notorious heterogeneity. The universal actions can be efficiently translated back to heterogeneous actionable commands by simply adding embodiment-specific details, from which fast adaptation to new robots becomes simple and straightforward. Our 0.5B instantiation of UniAct outperforms 14X larger SOTA embodied foundation models in extensive evaluations on various real-world and simulation robots, showcasing exceptional cross-embodiment control and adaptation capability, highlighting the crucial benefit of adopting universal actions. Project page: https://github.com/2toinf/UniAct

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 The UniAct Framework 3.1 Universal Action Space 3.2 Universal Action Extraction 3.3 Heterogeneous Decoding 3.4 Training Procedure 4 Experiments 4.1 Experiments Setup 4.2 Main Results 4.3 Fast Adaptation to New Embodiment 4.4 Fast Adaptation to New Decoder Head 4.5 In-depth Analysis of Universal Actions 5 Conclusion 6 Acknowledgment A Training Details B Evaluation Setups B.1 WidowX Robot in Real World B.2 Franka Robot in Simulation B.3 Fast adaptation to AIRBOT B.4 Fast adaptation to Bi-manual AIRBOT C More Related Works D Limitations and Future Works Universal Actions for Enhanced Embodied Foundation Models Jinliang Zheng 1 1 1 Equal contribution 1,2,5 , Jianxiong Li 1 1 1 Equal contribution 2 2 2 Project Lead 1 , Dongxiu Liu 1 1 1 Equal contribution 4,1 , Yinan Zheng 1 , Zhihao Wang 3,1 , Zhonghong Ou 4 , Yu Liu 2 , Jingjing Liu 1 , Ya-Qin Zhang 1 , Xianyuan Zhan 3 3 3 Corresponding author 1,5,6 1 AIR, Tsinghua University, 2 Sensetime Research, 3 Peking University 4 Beiji…

**Method / approach.** methods can enhance sample efficiency for specific robots on a narrow set of tasks, they suffer from serious performance bottlenecks towards building a generalist embodied agent [ 56 , 19 , 7 ] , as the action data gathered from any single robot platform is far less comprehensive than crowed-sourced data collected globally [ 49 , 30 , 20 ] . Some recent works leverage the abundant heterogeneous action labels to develop generalist robot policies for cross-embodiment control. RT-X series [ 49 ] , Octo [ 61 ] and OpenVLA [ 31 ] leverage data from different 7-DoF robots to enhance generalization over the one trained on single robot source. Step further, CrossFormer [ 17 ] , RDT [ 41 ] , π 0 subscript 𝜋 0 \pi_{0} italic_π start_POSTSUBSCRIPT 0 end_POSTSUBSCRIPT [ 8 ] and Yang et al. [ 68 ] explore the data from robots with totally distinct mechanical structures, such as those in manipulation and navigation, and from single-arm versus bi-manual systems. However, existing work…

**Results.** Experiments 4.1 Experiments Setup 4.2 Main Results 4.3 Fast Adaptation to New Embodiment 4.4 Fast Adaptation to New Decoder Head 4.5 In-depth Analysis of Universal Actions 5 Conclusion 6 Acknowledgment A Training Details B Evaluation Setups B.1 WidowX Robot in Real World B.2 Franka Robot in Simulation B.3 Fast adaptation to AIRBOT B.4 Fast adaptation to Bi-manual AIRBOT C More Related Works D Limitations and Future Works Universal Actions for Enhanced Embodied Foundation Models Jinliang Zheng 1 1 1 Equal contribution 1,2,5 , Jianxiong Li 1 1 1 Equal contribution 2 2 2 Project Lead 1 , Dongxiu Liu 1 1 1 Equal contribution 4,1 , Yinan Zheng 1 , Zhihao Wang 3,1 , Zhonghong Ou 4 , Yu Liu 2 , Jingjing Liu 1 , Ya-Qin Zhang 1 , Xianyuan Zhan 3 3 3 Corresponding author 1,5,6 1 AIR, Tsinghua University, 2 Sensetime Research, 3 Peking University 4 Beijing University of Posts and Tele…

**Conclusion.** Conclusion 6 Acknowledgment A Training Details B Evaluation Setups B.1 WidowX Robot in Real World B.2 Franka Robot in Simulation B.3 Fast adaptation to AIRBOT B.4 Fast adaptation to Bi-manual AIRBOT C More Related Works D Limitations and Future Works Universal Actions for Enhanced Embodied Foundation Models Jinliang Zheng 1 1 1 Equal contribution 1,2,5 , Jianxiong Li 1 1 1 Equal contribution 2 2 2 Project Lead 1 , Dongxiu Liu 1 1 1 Equal contribution 4,1 , Yinan Zheng 1 , Zhihao Wang 3,1 , Zhonghong Ou 4 , Yu Liu 2 , Jingjing Liu 1 , Ya-Qin Zhang 1 , Xianyuan Zhan 3 3 3 Corresponding author 1,5,6 1 AIR, Tsinghua University, 2 Sensetime Research, 3 Peking University 4 Beijing University of Pos…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]]
- **Raw:** `raw/arxiv/2501.10105v2.md` · `raw/arxiv/2501.10105v2.fulltext.md`
