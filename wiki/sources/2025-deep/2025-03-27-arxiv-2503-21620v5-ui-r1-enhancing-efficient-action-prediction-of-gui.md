---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning"
authors: Zhengxi Lu, Yuxiang Chai, Yaxuan Guo, Xi Yin et al.
url: https://arxiv.org/abs/2503.21620v5
date: 2025-03-27
citationCount: 122
influentialCitationCount: 13
velocity: 8.22
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning

**arXiv [2503.21620v5](https://arxiv.org/abs/2503.21620v5)** · 2025-03-27 · **122 citations** (13 influential · 8.22/mo) · Zhengxi Lu, Yuxiang Chai, Yaxuan Guo, Xi Yin et al.

## Abstract
The recent DeepSeek-R1 has showcased the emergence of reasoning capabilities in LLMs through reinforcement learning (RL) with rule-based rewards. Despite its success in language models, its application in multi-modal domains, particularly in graphic user interface (GUI) agent tasks, remains under-explored. To address this issue, we propose UI-R1, the first framework to explore how rule-based RL can enhance the reasoning capabilities of multimodal large language models (MLLMs) for GUI action prediction tasks. Specifically, UI-R1 introduces a novel rule-based action reward, enabling model optimization via policy-based algorithms such as Group Relative Policy Optimization (GRPO). For efficient training, we curate a small yet high-quality dataset of 136 challenging tasks, encompassing five common action types on mobile devices. Experimental results demonstrate that our proposed UI-R1-3B achieves significant improvements over the base model (i.e. Qwen2.5-VL-3B) on both in-domain (ID) and out-of-domain (OOD) tasks, with average accuracy gains of 22.1% on ScreenSpot, 6.0% on ScreenSpot-Pro, and 12.7% on ANDROIDCONTROL. Furthermore, UI-R1-3B delivers competitive performance compared to larger models (e.g., OS-Atlas-7B) trained via supervised fine-tuning (SFT) on 76K samples. We additionally develop an optimized version, UI-R1-E-3B, which significantly improves both grounding efficiency and accuracy. These results underscore the potential of rule-based reinforcement learning to advance GUI understanding and control, paving the way for future research in this domain. Code website: https://github.com/lll6gg/UI-R1.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 GUI Agents 2.2 Rule-Based Reinforcement Learning Efficient Reasoning. 3 Method 3.1 Preliminary 3.2 Rule-Based Action Rewards Action type reward. Coordinate accuracy reward. Format reward. 3.3 Fast Grounding DAST NOTHINK 3.4 Training Data Selection Quality. Difficulty. Diversity. 4 Experiments 4.1 GUI Grounding Capability Setting Analysis 4.2 Action Prediction Capability Setting Analysis 4.3 Key Factor Study Data Size Reasoning Length 4.4 Ablation Study Fast Grounding Reward Function Data Selection 5 Conclusion A Training A.1 Setting A.2 Dataset Distribution A.3 Visualization B Other Evaluation B.1 Reasoning C Other Ablation C.1 Training epoches C.2 Max Pixels D Case Study UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning Zhengxi Lu 1† , Yuxiang Chai 2† , Yaxuan Guo 1 , Xi Yin 1 , Liang Liu 1‡ , Hao Wang 1 , Han Xiao 2 , Shuai Ren 1 , Guanjing Xiong 1 , Hongsheng…

**Method / approach.** Method 3.1 Preliminary 3.2 Rule-Based Action Rewards Action type reward. Coordinate accuracy reward. Format reward. 3.3 Fast Grounding DAST NOTHINK 3.4 Training Data Selection Quality. Difficulty. Diversity. 4 Experiments 4.1 GUI Grounding Capability Setting Analysis 4.2 Action Prediction Capability Setting Analysis 4.3 Key Factor Study Data Size Reasoning Length 4.4 Ablation Study Fast Grounding Reward Function Data Selection 5 Conclusion A Training A.1 Setting A.2 Dataset Distribution A.3 Visualization B Other Evaluation B.1 Reasoning C Other Ablation C.1 Training epoches C.2 Max Pixels D Case Study UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning Zhengxi Lu 1† , Yuxiang Chai 2† , Yaxuan Guo 1 , Xi Yin 1 , Liang Liu 1‡ , Hao Wang 1 , Han Xiao 2 , Shuai Ren 1 , Guanjing Xiong 1 , Hongsheng Li 2 🖂 1 vivo AI…

**Results.** Experiments 4.1 GUI Grounding Capability Setting Analysis 4.2 Action Prediction Capability Setting Analysis 4.3 Key Factor Study Data Size Reasoning Length 4.4 Ablation Study Fast Grounding Reward Function Data Selection 5 Conclusion A Training A.1 Setting A.2 Dataset Distribution A.3 Visualization B Other Evaluation B.1 Reasoning C Other Ablation C.1 Training epoches C.2 Max Pixels D Case Study UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning Zhengxi Lu 1† , Yuxiang Chai 2† , Yaxuan Guo 1 , Xi Yin 1 , Liang Liu 1‡ , Hao Wang 1 , Han Xiao 2 , Shuai Ren 1 , Guanjing Xiong 1 , Hongsheng Li 2 🖂 1 vivo AI Lab 2 MMLab @ CUHK † Equal Contribution, ‡ Project Lead, 🖂 Corresponding Author {zhengxilu@zju.edu.cn} Abstract The recent DeepSeek-R1 has showcased the emergence of reasoning capabil…

**Conclusion.** Conclusion A Training A.1 Setting A.2 Dataset Distribution A.3 Visualization B Other Evaluation B.1 Reasoning C Other Ablation C.1 Training epoches C.2 Max Pixels D Case Study UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement Learning Zhengxi Lu 1† , Yuxiang Chai 2† , Yaxuan Guo 1 , Xi Yin 1 , Liang Liu 1‡ , Hao Wang 1 , Han Xiao 2 , Shuai Ren 1 , Guanjing Xiong 1 , Hongsheng Li 2 🖂 1 vivo AI Lab 2 MMLab @ CUHK † Equal Contribution, ‡ Project Lead, 🖂 Corresponding Author {zhengxilu@zju.edu.cn} Abstract The recent DeepSeek-R1 has showcased the emergence of reasoning capabilities in LLMs through reinforcement learning (RL) with rule-base…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[qwen]] · [[deepseek]]
- **Raw:** `raw/arxiv/2503.21620v5.md` · `raw/arxiv/2503.21620v5.fulltext.md`
