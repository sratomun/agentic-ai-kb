---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WoW: Towards a World omniscient World model Through Embodied Interaction"
authors: Xiaowei Chi, Peidong Jia, Chun-Kai Fan, Xiaozhu Ju et al.
url: https://arxiv.org/abs/2509.22642v2
date: 2025-09-26
citationCount: 47
influentialCitationCount: 7
velocity: 5.32
ingested: 2026-06-22
tags: [embodied-agents, science-agents, agent-evaluation, arxiv, 2025, cited]
---

# WoW: Towards a World omniscient World model Through Embodied Interaction

**arXiv [2509.22642v2](https://arxiv.org/abs/2509.22642v2)** · 2025-09-26 · **47 citations** (7 influential · 5.32/mo) · Xiaowei Chi, Peidong Jia, Chun-Kai Fan, Xiaozhu Ju et al.

## Abstract
Humans develop an understanding of intuitive physics through active interaction with the world. This approach is in stark contrast to current video models, such as Sora, which rely on passive observation and therefore struggle with grasping physical causality. This observation leads to our central hypothesis: authentic physical intuition of the world model must be grounded in extensive, causally rich interactions with the real world. To test this hypothesis, we present WoW, a 14-billion-parameter generative world model trained on 2 million robot interaction trajectories. Our findings reveal that the model's understanding of physics is a probabilistic distribution of plausible outcomes, leading to stochastic instabilities and physical hallucinations. Furthermore, we demonstrate that this emergent capability can be actively constrained toward physical realism by SOPHIA, where vision-language model agents evaluate the DiT-generated output and guide its refinement by iteratively evolving the language instructions. In addition, a co-trained Inverse Dynamics Model translates these refined plans into executable robotic actions, thus closing the imagination-to-action loop. We establish WoWBench, a new benchmark focused on physical consistency and causal reasoning in video, where WoW achieves state-of-the-art performance in both human and autonomous evaluation, demonstrating strong ability in physical causality, collision dynamics, and object permanence. Our work provides systematic evidence that large-scale, real-world interaction is a cornerstone for developing physical intuition in AI. Models, data, and benchmarks will be open-sourced.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Rethinking World Model: Towards A World-Omniscient Intelligent 2.1 Definition of a World Model 2.2 Evolution of World Models: Representation and Modality 2.3 Embodied World Modeling 2.4 Emergency, Toward a Generative Physical Engine 2.5 The Cognitive Science Connection: World Model in Mind 3 WoW World Model 4 Self-Optimizing Framework 4.1 Foundation Video Generation World Model 4.1.1 Pretrain Data Preparation Collection. Filtering. Caption Refinement. Rebalancing. 4.1.2 Diffusion-Based Video Generation 4.2 Solver-Critic Video Generation Agents 4.2.1 Framework Overview 4.2.2 Refiner Agent in World Model 4.2.3 Dynamic Critic Model Team 4.2.4 Closed-Loop Generative Workflow 4.2.5 Discussion: The Prover-Verifier Paradigm for Generative World Models 4.3 Flow-Mask Inverse Dynamics Model Task Formulation 5 WoWBench: A Multi-faceted Benchmark for Embodied World Models 5.1 Core Evaluation Dimensions Perception Understanding Predictive Reasoning Decision-making and Planning Generalized Execution 5…

**Method / approach.** methods and proposed WoW across 4 core metrics and 20 associated tasks. • Postraining Application Discussion. We demonstrate that WoW is more than a generator, showcasing its versatility across a range of downstream applications. These applications include synthesizing novel views, generating trajectory-guided videos, producing action-conditioned videos for robot manipulation, enhancing visual style transfer and improving VLM task planning at test-time. • A Scaling Analysis and Open-Source Models. We perform a systematic scaling analysis of our architecture up to 14B parameters, uncovering nascent capabilities and potential precursors to emergence in physical reasoning. This provides strong empirical evidence for the scaling hypothesis in this domain. We will release all trained model checkpoints to provide a foundation for future research in the embodied world model. 2 Rethinking World Model: Towards A World-Omniscient Intelligent The idea that intelligent agents…

**Results.** Experiment: Evaluating Generative World Models 6.1 Training Data 6.2 Model Comparsion Experiment 6.3 Qualitative Experiment 6.4 Generalization Discussion 6.4.1 Visual Evaluation 6.4.2 Quantity Evaluation 6.5 Real World Robot Manipulation 7 Case Study: Advanced Reasoning and Generalization 7.1 Counterfactual Reasoning and replanning 7.2 Tool-Use Generalization via Iterative Prompt Refinement 7.3 Physical and Logical Constitutionality 8 Foundation Model For Application Post-Training 8.1 Novel-View Synthesis and Generation 8.2 Spatial-Aware Trajectory-Guided Video Generation Trajectory-Conditioned Video Synthesis 8.3 Action-to-Video Generation for Robot Manipulation Definition. 8.4 Visual Style Transfer Enhancement Embodiment. Object. Background. Multi-condition Mixture. 8.5 Test-Time Scaling for VLM task planning Task Setting. Quality Comparison. Experiment…

**Conclusion.** Conclusion and Future Work WoW: Towards a World-omniscient World-model Through Embodied Interaction Xiaowei Chi 1,2,3, † , Peidong Jia 1,2, † , Chun-Kai Fan 1,2, † , Xiaozhu Ju 1, † , Weishi Mi 1, † , Zhiyuan Qin 1, † , Kevin Zhang 2 , Wanxin Tian 1 , Kuangzhi Ge 2 , Hao Li 1 , Zezhong Qian 1,2 , Anthony Chen 2 , Qiang Zhou 1,2 , Yueru Jia 2 , Jiaming Liu 2 , Yong Dai 1 , Qingpo Wuwu 2 , Chengyu Bai 2 , Yu-Kai Wang 2 , Ying Li 2 , Lizhang Chen 1,2 , Yong Bao 1 , Zhiyuan Jiang 1 , Jiacheng Zhu 1 , Kai Tang 2 , Ruichuan An 2 , Yulin Luo 2 , Qiuxuan Feng 1,2 , Siyuan Zhou 3 , Chi-min Chan 3 , Chengkai Hou 1,2 , Wei Xue 3 , Sirui Han 3 , Yike Guo 3 , Shanghang Zhang 2,✉ , Jian Tang 1,✉ 1 Beijing Innovation Center of Humanoid Ro…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[science-agents|Science agents]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2509.22642v2.md` · `raw/arxiv/2509.22642v2.fulltext.md`
