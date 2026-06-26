---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "UI-TARS: Pioneering Automated GUI Interaction with Native Agents"
authors: Yujia Qin, Yining Ye, Junjie Fang, Haoming Wang et al.
url: https://arxiv.org/abs/2501.12326v1
date: 2025-01-21
citationCount: 464
influentialCitationCount: 147
velocity: 27.32
ingested: 2026-06-22
tags: [computer-use-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# UI-TARS: Pioneering Automated GUI Interaction with Native Agents

**arXiv [2501.12326v1](https://arxiv.org/abs/2501.12326v1)** · 2025-01-21 · **464 citations** (147 influential · 27.32/mo) · Yujia Qin, Yining Ye, Junjie Fang, Haoming Wang et al.

**Significance:** Landmark native GUI agent — a foundation for the 2026 computer-use wave.

## Abstract
This paper introduces UI-TARS, a native GUI agent model that solely perceives the screenshots as input and performs human-like interactions (e.g., keyboard and mouse operations). Unlike prevailing agent frameworks that depend on heavily wrapped commercial models (e.g., GPT-4o) with expert-crafted prompts and workflows, UI-TARS is an end-to-end model that outperforms these sophisticated frameworks. Experiments demonstrate its superior performance: UI-TARS achieves SOTA performance in 10+ GUI agent benchmarks evaluating perception, grounding, and GUI task execution. Notably, in the OSWorld benchmark, UI-TARS achieves scores of 24.6 with 50 steps and 22.7 with 15 steps, outperforming Claude (22.0 and 14.9 respectively). In AndroidWorld, UI-TARS achieves 46.6, surpassing GPT-4o (34.5). UI-TARS incorporates several key innovations: (1) Enhanced Perception: leveraging a large-scale dataset of GUI screenshots for context-aware understanding of UI elements and precise captioning; (2) Unified Action Modeling, which standardizes actions into a unified space across platforms and achieves precise grounding and interaction through large-scale action traces; (3) System-2 Reasoning, which incorporates deliberate reasoning into multi-step decision making, involving multiple reasoning patterns such as task decomposition, reflection thinking, milestone recognition, etc. (4) Iterative Training with Reflective Online Traces, which addresses the data bottleneck by automatically collecting, filtering, and reflectively refining new interaction traces on hundreds of virtual machines. Through iterative training and reflection tuning, UI-TARS continuously learns from its mistakes and adapts to unforeseen situations with minimal human intervention. We also analyze the evolution path of GUI agents to guide the further development of this domain.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Evolution Path of GUI Agents 2.1 Rule-based Agents Stage 1: Rule-based Agents 2.2 From Modular Agent Framework to Native Agent Model Stage 2: Agent Framework Key Limitations of Agent Frameworks Stage 3: Native Agent Model 2.3 Active and Lifelong Agent (Prospect) Stage 4: Action and Lifelong Agent 3 Core Capabilities of Native Agent Model 3.1 Core Capabilities Perception Action Reasoning with System 1 2 Thinking Memory 3.2 Capability Evaluation Perception Evaluation Grounding Evaluation Offline Agent Capability Evaluation Online Agent Capability Evaluation 4 UI-TARS 4.1 Architecture Overview 4.2 Enhancing GUI Perception Screenshot Collection Element Description Dense Captioning State Transition Captioning Question Answering (QA) Set-of-Mark (SoM) 4.3 Unified Action Modeling and Grounding Unified Action Space Action Trace Collection Improving Grounding Ability 4.4 Infusing System-2 Reasoning Reasoning Enrichment with GUI Tutorials Reasoning Stimulation with Thought Augm…

**Method / approach.** methods have driven significant progress, they suffer from limitations such as platform-specific inconsistencies, verbosity, and limited scalability (Xu et al., 2024 ) . Textual-based methods often require system-level permissions to access underlying system information, such as HTML code, which further limits their applicability and generalizability across diverse environments. Another critical issue is that, many existing GUI systems follow an agent framework paradigm (Zhang et al., 2023 ; Wang et al., 2024a ; Wu et al., 2024a ; Zhang et al., 2024b ; Wang Liu, 2024 ; Xie et al., 2024 ) , where key functions are modularized across multiple components. These components often rely on specialized vision-language models (VLMs), e.g., GPT-4o (Hurst et al., 2024 ) , for understanding and reasoning (Zhang et al., 2024b ) , while grounding (Lu et al., 2024b ) or memory (Zhang et al., 2023 ) modules are implemented through additional tools or scripts. Although this modular architecture…

**Results.** Experiment Baseline 5.1 Perception Capability Evaluation 5.2 Grounding Capability Evaluation 5.3 Offline Agent Capability Evaluation 5.4 Online Agent Capability Evaluation 5.5 Comparing System 1 and System 2 Reasoning In-domain Evaluation Out-of-domain Evaluation 6 Conclusion A Case Study B Data Example UI-TARS : Pioneering Automated GUI Interaction with Native Agents Yujia Qin † , Yining Ye ∗♢ , Junjie Fang ∗ , Haoming Wang ∗ , Shihao Liang ∗ , Shizuo Tian ♢ , Junda Zhang, Jiahao Li, Yunxin Li, Shijue Huang, Wanjun Zhong, Kuanye Li, Jiale Yang, Yu Miao, Woyu Lin, Longxiang Liu, Xu Jiang, Qianli Ma, Jingyu Li, Xiaojun Xiao, Kai Cai, Chuang Li, Yaowei Zheng, Chaolin Jin, Chen Li, Xiao Zhou, Minchao Wang, Haoli Chen, Zhaojian Li, Haihua Yang, Haifeng Liu, Feng Lin, Tao Peng, Xin Liu, Guang Shi † ByteDance Seed, ♢ Tsinghua University {yujia.qin, shiguang.sg}@bytedance.com Indicates equal…

**Conclusion.** Conclusion A Case Study B Data Example UI-TARS : Pioneering Automated GUI Interaction with Native Agents Yujia Qin † , Yining Ye ∗♢ , Junjie Fang ∗ , Haoming Wang ∗ , Shihao Liang ∗ , Shizuo Tian ♢ , Junda Zhang, Jiahao Li, Yunxin Li, Shijue Huang, Wanjun Zhong, Kuanye Li, Jiale Yang, Yu Miao, Woyu Lin, Longxiang Liu, Xu Jiang, Qianli Ma, Jingyu Li, Xiaojun Xiao, Kai Cai, Chuang Li, Yaowei Zheng, Chaolin Jin, Chen Li, Xiao Zhou, Minchao Wang, Haoli Chen, Zhaojian Li, Haihua Yang, Haifeng Liu, Feng Lin, Tao Peng, Xin Liu, Guang Shi † ByteDance Seed, ♢ Tsinghua University {yujia.qin, shiguang.sg}@bytedance.com Indicates equal contribution. † Corresponding author. ♢ The work is done when interning at ByteDance…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[osworld]] · [[claude]] · [[gpt-5]] · [[ui-tars]]
- **Raw:** `raw/arxiv/2501.12326v1.md` · `raw/arxiv/2501.12326v1.fulltext.md`
