---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft"
authors: Junliang Guo, Yang Ye, Tianyu He, Haoyu Wu et al.
url: https://arxiv.org/abs/2504.08388v1
date: 2025-04-11
citationCount: 64
influentialCitationCount: 8
velocity: 4.46
ingested: 2026-06-22
tags: [agentic-ai, arxiv, 2025, cited]
---

# MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft

**arXiv [2504.08388v1](https://arxiv.org/abs/2504.08388v1)** · 2025-04-11 · **64 citations** (8 influential · 4.46/mo) · Junliang Guo, Yang Ye, Tianyu He, Haoyu Wu et al.

## Abstract
World modeling is a crucial task for enabling intelligent agents to effectively interact with humans and operate in dynamic environments. In this work, we propose MineWorld, a real-time interactive world model on Minecraft, an open-ended sandbox game which has been utilized as a common testbed for world modeling. MineWorld is driven by a visual-action autoregressive Transformer, which takes paired game scenes and corresponding actions as input, and generates consequent new scenes following the actions. Specifically, by transforming visual game scenes and actions into discrete token ids with an image tokenizer and an action tokenizer correspondingly, we consist the model input with the concatenation of the two kinds of ids interleaved. The model is then trained with next token prediction to learn rich representations of game states as well as the conditions between states and actions simultaneously. In inference, we develop a novel parallel decoding algorithm that predicts the spatial redundant tokens in each frame at the same time, letting models in different scales generate $4$ to $7$ frames per second and enabling real-time interactions with game players. In evaluation, we propose new metrics to assess not only visual quality but also the action following capacity when generating new scenes, which is crucial for a world model. Our comprehensive evaluation shows the efficacy of MineWorld, outperforming SoTA open-sourced diffusion based world models significantly. The code and model have been released.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Framework 2.1 Overview 2.2 Architectures Tokenizers Transformer Decoder 2.3 Parallel Decoding Real-Time Interactive World Model Discussion with Related Works 3 Evaluation 3.1 Dataset Construction and Preprocessing 3.2 Evaluation Metrics Discrete Action Classification Camera Movement. 3.3 Implementation Details 4 Experiments 4.1 Main Results 4.2 Analysis The Effect of Parallel Decoding The Metrics on Controllability 4.3 Case Study General Capability Controllability Serve as an Agent 5 Conclusion and Limitations Limitations A Minecraft Action Space A.1 Details of Action Following Metric A.2 Task-Specific Action Accuracy B Model Configurations C More Results C.1 Reconstruction Results of Visual Tokenizer MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft Junliang Guo ∗ , Yang Ye ∗ , Tianyu He ∗ , Haoyu Wu ∗ , Yushu Jiang, Tim Pearce, Jiang Bian ∗ Equal contribution. Correspondence to Junliang Guo. Microsoft Research {junliangguo,v-yan…

**Method / approach.** method exploits the dependencies between spatially adjacent tokens, allowing certain token groups to be predicted in parallel. This optimization results in over a more than 3 × 3\times 3 × speedup compared to standard autoregressive decoding, without sacreficing the quality of results. Equipped with this decoding algorithm, MineWorld is able to generate 4 4 4 4 to 7 7 7 7 frames in one second, making the real-time interaction between human and world model feasible. In addition, to assess the controllability of MineWorld, we propose new evaluation metrics that extend beyond conventional video quality assessments. We first transform the actions in Minecraft to discrete tokens in one vocabulary. Then, after output videos are generated conditioned on previous frames and actions, we utilize an inverse dynamic model (IDM) (Baker et al., 2022 ) to predict an action between consecutive generated frames. This predicted action can be treated as the executed action according to generated vid…

**Results.** Experiments 4.1 Main Results 4.2 Analysis The Effect of Parallel Decoding The Metrics on Controllability 4.3 Case Study General Capability Controllability Serve as an Agent 5 Conclusion and Limitations Limitations A Minecraft Action Space A.1 Details of Action Following Metric A.2 Task-Specific Action Accuracy B Model Configurations C More Results C.1 Reconstruction Results of Visual Tokenizer MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft Junliang Guo ∗ , Yang Ye ∗ , Tianyu He ∗ , Haoyu Wu ∗ , Yushu Jiang, Tim Pearce, Jiang Bian ∗ Equal contribution. Correspondence to Junliang Guo. Microsoft Research {junliangguo,v-yangye,tianyuhe, v-haoywu}@microsoft.com Abstract World modeling is a crucial task for enabling intelligent agents to effectively interact with humans and operate in dynamic environments. In this work, we propose MineWorld, a r…

**Conclusion.** Conclusion and Limitations Limitations A Minecraft Action Space A.1 Details of Action Following Metric A.2 Task-Specific Action Accuracy B Model Configurations C More Results C.1 Reconstruction Results of Visual Tokenizer MineWorld: a Real-Time and Open-Source Interactive World Model on Minecraft Junliang Guo ∗ , Yang Ye ∗ , Tianyu He ∗ , Haoyu Wu ∗ , Yushu Jiang, Tim Pearce, Jiang Bian ∗ Equal contribution. Correspondence to Junliang Guo. Microsoft Research {junliangguo,v-yangye,tianyuhe, v-haoywu}@microsoft.com Abstract World modeling is a crucial task for enabling intelligent agents to effectively interact with humans and operate in dynamic environments. In this work, we propose MineWorld, a real…

## Graph
- **Concepts:** [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.08388v1.md` · `raw/arxiv/2504.08388v1.fulltext.md`
