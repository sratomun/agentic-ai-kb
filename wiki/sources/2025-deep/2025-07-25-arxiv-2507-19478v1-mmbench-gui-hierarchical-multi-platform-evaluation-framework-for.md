---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MMBench-GUI: Hierarchical Multi-Platform Evaluation Framework for GUI Agents"
authors: Xuehui Wang, Zhenyu Wu, JingJing Xie, Zichen Ding et al.
url: https://arxiv.org/abs/2507.19478v1
date: 2025-07-25
citationCount: 46
influentialCitationCount: 8
velocity: 4.22
ingested: 2026-06-22
tags: [computer-use-agents, agent-reliability, agent-skills, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# MMBench-GUI: Hierarchical Multi-Platform Evaluation Framework for GUI Agents

**arXiv [2507.19478v1](https://arxiv.org/abs/2507.19478v1)** · 2025-07-25 · **46 citations** (8 influential · 4.22/mo) · Xuehui Wang, Zhenyu Wu, JingJing Xie, Zichen Ding et al.

## Abstract
We introduce MMBench-GUI, a hierarchical benchmark for evaluating GUI automation agents across Windows, macOS, Linux, iOS, Android, and Web platforms. It comprises four levels: GUI Content Understanding, Element Grounding, Task Automation, and Task Collaboration, covering essential skills for GUI agents. In addition, we propose a novel Efficiency-Quality Area (EQA) metric to assess GUI agent execution efficiency in online automation scenarios. Through MMBench-GUI, we identify accurate visual grounding as a critical determinant of overall task success, emphasizing the substantial benefits of modular frameworks that integrate specialized grounding modules. Furthermore, to achieve reliable GUI automation, an agent requires strong task planning and cross-platform generalization abilities, with long-context memory, a broad action space, and long-term reasoning playing a critical role. More important, task efficiency remains a critically underexplored dimension, and all models suffer from substantial inefficiencies, with excessive redundant steps even when tasks are ultimately completed. The integration of precise localization, effective planning, and early stopping strategies is indispensable to enable truly efficient and scalable GUI automation. Our benchmark code, evaluation data, and running environment will be publicly available at https://github.com/open-compass/MMBench-GUI.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related works 3 MMBench-GUI 3.1 Hierarchical Evaluation 3.2 L1-GUI Content Understanding 3.3 Level 2: GUI Element Grounding 3.4 Level 3: GUI Task Automation 3.5 Level 4: GUI Task Collaboration 3.6 Benchmark Statistics 4 Benchmarking GUI Agent Baselines 4.1 Benchmarking details 4.2 Benchmark results on L1-GUI Content Understanding 4.3 Benchmark results on L2-GUI Element Grounding 4.4 Benchmark results on L3-GUI Task Automation and L4-GUI Task Collaboration 5 Analysis and discussion 6 Conclusion MMBench-GUI: Hierarchical Multi-Platform Evaluation Framework for GUI Agents Xuehui Wang 2,1∗ , Zhenyu Wu 2,1∗ , JingJing Xie 3,1∗ , Zichen Ding 1∗ , Bowen Yang 4,1∗ , Zehao Li 4,1∗ , Zhaoyang Liu 5,1∗ , Qingyun Li 6,1 , Xuan Dong 7 , Zhe Chen 8,1 , Weiyun Wang 9,1 , Xiangyu Zhao 2,1 , Jixuan Chen 8,1 , Haodong Duan 1 , Tianbao Xie 10 , Chenyu Yang 1 , Shiqian Su 7 , Yue Yu 7 , Yuan Huang, Yiqian Liu, Xiao Zhang, Yanting Zhang 11 Xiangyu Yue 12 , Weijie Su 1 , Xizhou Zhu 7 , Wei Shen 2 🖂 , Jifeng Dai 7 , Wenhai Wang 12,1 🖂 1 Shan…

**Method / approach.** approaches benefit from state-of-the-art components but face challenges in system-level alignment Cheng et al. ( 2024 ); Gou et al. ( 2024 ) . In contrast, the native agent paradigm aligns capabilities more naturally during training (Wu et al., 2024b ; Xu et al., 2024b ; Qin et al., 2025 ) . Both paradigms can use screenshots (Niu et al., 2024 ; Liu et al., 2024a ) , accessibility trees (A11y Trees) (Gao et al., 2023 ) , and HTML pages (Furuta et al., 2023 ; Deng et al., 2023b ) as input. However, A11y Trees and HTML codes vary across platforms, are prone to noise, and may cause excessive token length (Zheng et al., 2024 ; Hong et al., 2024 ; Cheng et al., 2024 ) . Generally, in this work, we focus exclusively on the screenshot-only setting and propose a hierarchical, multi-platform benchmark to evaluate these vision-only native agents. GUI Benchmarks. Effectively GUIs requires a sophisticated grasp of intertwined visual and textual cues, yet this complex domain remains large…

**Results.** Evaluation Framework for GUI Agents 1 Introduction 2 Related works 3 MMBench-GUI 3.1 Hierarchical Evaluation 3.2 L1-GUI Content Understanding 3.3 Level 2: GUI Element Grounding 3.4 Level 3: GUI Task Automation 3.5 Level 4: GUI Task Collaboration 3.6 Benchmark Statistics 4 Benchmarking GUI Agent Baselines 4.1 Benchmarking details 4.2 Benchmark results on L1-GUI Content Understanding 4.3 Benchmark results on L2-GUI Element Grounding 4.4 Benchmark results on L3-GUI Task Automation and L4-GUI Task Collaboration 5 Analysis and discussion 6 Conclusion MMBench-GUI: Hierarchical Multi-Platform Evaluation Framework for GUI Agents Xuehui Wang 2,1∗ , Zhenyu Wu 2,1∗ , JingJing Xie 3,1∗ , Zichen Ding 1∗ , Bowen Yang 4,1∗ , Zehao Li 4,1∗ , Zhaoyang Liu 5,1∗ , Qingyun Li 6,1 , Xuan Dong 7 , Zhe Chen 8,1 , Weiyun Wang 9,1 , Xiangyu Zhao 2,1 , Jixuan Chen 8,1 , Haodong Duan 1 , Tianbao Xie 10 , Chenyu Yang…

**Conclusion.** Conclusion MMBench-GUI: Hierarchical Multi-Platform Evaluation Framework for GUI Agents Xuehui Wang 2,1∗ , Zhenyu Wu 2,1∗ , JingJing Xie 3,1∗ , Zichen Ding 1∗ , Bowen Yang 4,1∗ , Zehao Li 4,1∗ , Zhaoyang Liu 5,1∗ , Qingyun Li 6,1 , Xuan Dong 7 , Zhe Chen 8,1 , Weiyun Wang 9,1 , Xiangyu Zhao 2,1 , Jixuan Chen 8,1 , Haodong Duan 1 , Tianbao Xie 10 , Chenyu Yang 1 , Shiqian Su 7 , Yue Yu 7 , Yuan Huang, Yiqian Liu, Xiao Zhang, Yanting Zhang 11 Xiangyu Yue 12 , Weijie Su 1 , Xizhou Zhu 7 , Wei Shen 2 🖂 , Jifeng Dai 7 , Wenhai Wang 12,1 🖂 1 Shanghai AI Laboratory, 2 Shanghai Jiao Tong University, 3 Xiamen University, 4 University of Science and Technology of China, 5 The Hong Kong University of Science and Technology, 6 Harbi…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2507.19478v1.md` · `raw/arxiv/2507.19478v1.fulltext.md`
