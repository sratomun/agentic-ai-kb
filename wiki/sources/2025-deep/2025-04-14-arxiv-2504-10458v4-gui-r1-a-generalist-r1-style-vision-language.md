---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents"
authors: Run Luo, Lu Wang, Wanwei He, Longze Chen et al.
url: https://arxiv.org/abs/2504.10458v4
date: 2025-04-14
citationCount: 218
influentialCitationCount: 29
velocity: 15.29
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents

**arXiv [2504.10458v4](https://arxiv.org/abs/2504.10458v4)** · 2025-04-14 · **218 citations** (29 influential · 15.29/mo) · Run Luo, Lu Wang, Wanwei He, Longze Chen et al.

## Abstract
Existing efforts in building Graphical User Interface (GUI) agents largely rely on the training paradigm of supervised fine-tuning on Large Vision-Language Models (LVLMs). However, this approach not only demands extensive amounts of training data but also struggles to effectively understand GUI screenshots and generalize to unseen interfaces. The issue significantly limits its application in real-world scenarios, especially for high-level tasks. Inspired by Reinforcement Fine-Tuning (RFT) in large reasoning models (e.g., DeepSeek-R1), which efficiently enhances the problem-solving capabilities of large language models in real-world settings, we propose \name, the first reinforcement learning framework designed to enhance the GUI capabilities of LVLMs in high-level real-world task scenarios, through unified action space rule modeling. By leveraging a small amount of carefully curated high-quality data across multiple platforms (including Windows, Linux, MacOS, Android, and Web) and employing policy optimization algorithms such as Group Relative Policy Optimization (GRPO) to update the model, \name achieves superior performance using only 0.02\% of the data (3K vs. 13M) compared to previous state-of-the-art methods like OS-Atlas across eight benchmarks spanning three different platforms (mobile, desktop, and web). These results demonstrate the immense potential of reinforcement learning based on unified action space rule modeling in improving the execution capabilities of LVLMs for real-world GUI agent tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 GUI Agents 2.2 Reinforcement Fine-Tuning 3 GUI-R1 Framework 3.1 Preliminaries 3.2 Verifiable Rewards in Unified Action Space 3.3 Training Data Curation 4 Experiments 4.1 Implementation Details 4.2 Experimental Results 4.3 Ablation Study 4.4 Visualization 5 Conclusion GUI-R1: A Generalist R1-Style Vision-Language Action Model For GUI Agents Run Luo 1,2 Lu Wang 3 Wanwei He 1,2 Longze Chen 1,2 Jiaming Li 1,2 Min Yang 1,2 Xiaobo Xia 3 1 Shenzhen Institute of Advanced Technology, Chinese Academy of Sciences 2 University of Chinese Academy of Sciences 3 National University of Singapore { r.luo@siat.ac.cn m.yang@siat.ac.cn xiaoboxia.uni@gmail.com } Abstract Existing efforts in building graphical user interface (GUI) agents largely rely on the training paradigm of supervised fine-tuning (SFT) on large vision-language models (LVLMs). However, this approach not only demands extensive amounts of training data but also struggles to effectively understand GUI screenshots and generalize to unseen interfaces. Th…

**Method / approach.** methods like OS-Atlas across eight benchmarks spanning three different platforms (mobile, desktop, and web). These results demonstrate the immense potential of reinforcement learning based on unified action space rule modeling in improving the execution capabilities of LVLMs for real-world GUI agent tasks. The codebase is available at https://github.com/ritzz-ai/GUI-R1.git . (a) Grounding capability. (b) Low-level task capability. (c) High-level task capability. Figure 1 : GUI-R1 achieves the best performance on eight evaluation datasets covering various platforms and task granularities, demonstrating the promising potential of RFT in GUI agent tasks. 1 Introduction Recent studies [ 1 ; 2 ; 3 ] have explored the use of large vision-language models (LVLMs) [ 4 ] to develop graphical user interface (GUI) agents capable of performing high-level complex tasks. These agents analyze the screen as a self-contained source of information for decision-making, without relyin…

**Results.** Experiments 4.1 Implementation Details 4.2 Experimental Results 4.3 Ablation Study 4.4 Visualization 5 Conclusion GUI-R1: A Generalist R1-Style Vision-Language Action Model For GUI Agents Run Luo 1,2 Lu Wang 3 Wanwei He 1,2 Longze Chen 1,2 Jiaming Li 1,2 Min Yang 1,2 Xiaobo Xia 3 1 Shenzhen Institute of Advanced Technology, Chinese Academy of Sciences 2 University of Chinese Academy of Sciences 3 National University of Singapore { r.luo@siat.ac.cn m.yang@siat.ac.cn xiaoboxia.uni@gmail.com } Abstract Existing efforts in building graphical user interface (GUI) agents largely rely on the training paradigm of supervised fine-tuning (SFT) on large vision-language models (LVLMs). However, this approach not only demands extensive amounts of training data but also struggles to effectively understand GUI screenshots and generalize to unseen interfaces. The issue significantly limits its application in real-world s…

**Conclusion.** Conclusion GUI-R1: A Generalist R1-Style Vision-Language Action Model For GUI Agents Run Luo 1,2 Lu Wang 3 Wanwei He 1,2 Longze Chen 1,2 Jiaming Li 1,2 Min Yang 1,2 Xiaobo Xia 3 1 Shenzhen Institute of Advanced Technology, Chinese Academy of Sciences 2 University of Chinese Academy of Sciences 3 National University of Singapore { r.luo@siat.ac.cn m.yang@siat.ac.cn xiaoboxia.uni@gmail.com } Abstract Existing efforts in building graphical user interface (GUI) agents largely rely on the training paradigm of supervised fine-tuning (SFT) on large vision-language models (LVLMs). However, this approach not only demands extensive amounts of training data but also struggles to effectively understand GUI screenshots and generalize…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[deepseek]]
- **Raw:** `raw/arxiv/2504.10458v4.md` · `raw/arxiv/2504.10458v4.fulltext.md`
