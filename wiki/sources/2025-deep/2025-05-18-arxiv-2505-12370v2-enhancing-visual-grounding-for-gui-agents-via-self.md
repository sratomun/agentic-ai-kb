---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning"
authors: Xinbin Yuan, Jian Zhang, Kaixin Li, Zhuoxuan Cai et al.
url: https://arxiv.org/abs/2505.12370v2
date: 2025-05-18
citationCount: 61
influentialCitationCount: 7
velocity: 4.64
ingested: 2026-06-22
tags: [computer-use-agents, self-evolving-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning

**arXiv [2505.12370v2](https://arxiv.org/abs/2505.12370v2)** · 2025-05-18 · **61 citations** (7 influential · 4.64/mo) · Xinbin Yuan, Jian Zhang, Kaixin Li, Zhuoxuan Cai et al.

## Abstract
Graphical User Interface (GUI) agents have made substantial strides in understanding and executing user instructions across diverse platforms. Yet, grounding these instructions to precise interface elements remains challenging, especially in complex, high-resolution, professional environments. Traditional supervised finetuning (SFT) methods often require large volumes of diverse data and exhibit weak generalization. To overcome these limitations, we introduce a reinforcement learning (RL) based framework that incorporates three core strategies: (1) seed data curation to ensure high quality training samples, (2) a dense policy gradient that provides continuous feedback based on prediction accuracy, and (3) a self evolutionary reinforcement finetuning mechanism that iteratively refines the model using attention maps. With only 3k training samples, our 7B-parameter model achieves state-of-the-art results among similarly sized models on three grounding benchmarks. Notably, it attains 47.3\% accuracy on the ScreenSpot-Pro dataset, outperforming much larger models, such as UI-TARS-72B, by a margin of 24.2\%. These findings underscore the effectiveness of RL-based approaches in enhancing GUI agent performance, particularly in high-resolution, complex environments.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 GUI Agents 2.2 Reinforcement Learning 3 Method 3.1 Seed Data Curation 3.2 Group Relative Policy Optimization with Dense Point Reward 3.3 Self-Evolutionary Reinforcement Fine-Tuning 4 Experiments 4.1 Implementation Details 4.2 Experimental Results 4.3 Ablation Study 5 Conclusions and Limitations A GRPO preliminary B More training details. C Attention visulization. D Hyper parameters Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning Xinbin Yuan 1,2 1 1 1 This work was done during Xinbin Yuan’s internship at vivo. Jian Zhang 2 3 3 3 Project lead. Kaixin Li 2 Zhuoxuan Cai 2 Lujian Yao 2 Jie Chen 2 Enguang Wang 2 Qibin Hou 1 2 2 2 Corresponding authors. Jinwei Chen 2 Peng-Tao Jiang 2 Bo Li 2 2 2 footnotemark: 2 1 VCIP, School of Computer Science, NKU 2 vivo Mobile Communication Co., Ltd yxb@mail.nankai.edu.cn, houqb@nankai.edu.cn, libra@vivo.com Project page: https://github.com/YXB-NKU/SE-GUI Abstract Graphical User Interface (GUI) agents have…

**Method / approach.** Method 3.1 Seed Data Curation 3.2 Group Relative Policy Optimization with Dense Point Reward 3.3 Self-Evolutionary Reinforcement Fine-Tuning 4 Experiments 4.1 Implementation Details 4.2 Experimental Results 4.3 Ablation Study 5 Conclusions and Limitations A GRPO preliminary B More training details. C Attention visulization. D Hyper parameters Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning Xinbin Yuan 1,2 1 1 1 This work was done during Xinbin Yuan’s internship at vivo. Jian Zhang 2 3 3 3 Project lead. Kaixin Li 2 Zhuoxuan Cai 2 Lujian Yao 2 Jie Chen 2 Enguang Wang 2 Qibin Hou 1 2 2 2 Corresponding authors. Jinwei Chen 2 Peng-Tao Jiang 2 Bo Li 2 2 2 footnotemark: 2 1 VCIP, School of Computer Science, NKU 2 vivo Mobile Communication Co., Ltd yxb@mail.nankai.edu.cn, houqb@nankai.edu.cn, libra@vivo.com Project page: https://github.com/YXB-NKU/SE-GUI Abstract Graphical User Interface (…

**Results.** Experiments 4.1 Implementation Details 4.2 Experimental Results 4.3 Ablation Study 5 Conclusions and Limitations A GRPO preliminary B More training details. C Attention visulization. D Hyper parameters Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning Xinbin Yuan 1,2 1 1 1 This work was done during Xinbin Yuan’s internship at vivo. Jian Zhang 2 3 3 3 Project lead. Kaixin Li 2 Zhuoxuan Cai 2 Lujian Yao 2 Jie Chen 2 Enguang Wang 2 Qibin Hou 1 2 2 2 Corresponding authors. Jinwei Chen 2 Peng-Tao Jiang 2 Bo Li 2 2 2 footnotemark: 2 1 VCIP, School of Computer Science, NKU 2 vivo Mobile Communication Co., Ltd yxb@mail.nankai.edu.cn, houqb@nankai.edu.cn, libra@vivo.com Project page: https://github.com/YXB-NKU/SE-GUI Abstract Graphical User Interface (GUI) agents have made substantial strides in understanding and executing user instructions across diverse…

**Conclusion.** Conclusions and Limitations A GRPO preliminary B More training details. C Attention visulization. D Hyper parameters Enhancing Visual Grounding for GUI Agents via Self-Evolutionary Reinforcement Learning Xinbin Yuan 1,2 1 1 1 This work was done during Xinbin Yuan’s internship at vivo. Jian Zhang 2 3 3 3 Project lead. Kaixin Li 2 Zhuoxuan Cai 2 Lujian Yao 2 Jie Chen 2 Enguang Wang 2 Qibin Hou 1 2 2 2 Corresponding authors. Jinwei Chen 2 Peng-Tao Jiang 2 Bo Li 2 2 2 footnotemark: 2 1 VCIP, School of Computer Science, NKU 2 vivo Mobile Communication Co., Ltd yxb@mail.nankai.edu.cn, houqb@nankai.edu.cn, libra@vivo.com Project page: https://github.com/YXB-NKU/SE-GUI Abstract Graphical User Interface (G…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.12370v2.md` · `raw/arxiv/2505.12370v2.fulltext.md`
