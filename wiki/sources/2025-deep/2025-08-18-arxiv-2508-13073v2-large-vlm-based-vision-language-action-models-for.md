---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Large VLM-based Vision-Language-Action Models for Robotic Manipulation: A Survey"
authors: Rui Shao, Wei Li, Lingsen Zhang, Renshan Zhang et al.
url: https://arxiv.org/abs/2508.13073v2
date: 2025-08-18
citationCount: 68
influentialCitationCount: 2
velocity: 6.72
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agent-memory, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# Large VLM-based Vision-Language-Action Models for Robotic Manipulation: A Survey

**arXiv [2508.13073v2](https://arxiv.org/abs/2508.13073v2)** · 2025-08-18 · **68 citations** (2 influential · 6.72/mo) · Rui Shao, Wei Li, Lingsen Zhang, Renshan Zhang et al.

## Abstract
Robotic manipulation, a key frontier in robotics and embodied AI, requires precise motor control and multimodal understanding, yet traditional rule-based methods fail to scale or generalize in unstructured, novel environments. In recent years, Vision-Language-Action (VLA) models, built upon Large Vision-Language Models (VLMs) pretrained on vast image-text datasets, have emerged as a transformative paradigm. This survey provides the first systematic, taxonomy-oriented review of large VLM-based VLA models for robotic manipulation. We begin by clearly defining large VLM-based VLA models and delineating two principal architectural paradigms: (1) monolithic models, encompassing single-system and dual-system designs with differing levels of integration; and (2) hierarchical models, which explicitly decouple planning from execution via interpretable intermediate representations. Building on this foundation, we present an in-depth examination of large VLM-based VLA models: (1) integration with advanced domains, including reinforcement learning, training-free optimization, learning from human videos, and world model integration; (2) synthesis of distinctive characteristics, consolidating architectural traits, operational strengths, and the datasets and benchmarks that support their development; (3) identification of promising directions, including memory mechanisms, 4D perception, efficient adaptation, multi-agent cooperation, and other emerging capabilities. This survey consolidates recent advances to resolve inconsistencies in existing taxonomies, mitigate research fragmentation, and fill a critical gap through the systematic integration of studies at the intersection of large VLMs and robotic manipulation. We provide a regularly updated project page to document ongoing progress: https://github.com/JiuTian-VL/Large-VLM-based-VLA-for-Robotic-Manipulation

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background 2.1 Evolution of Vision-Language Models 2.2 Advancements in Robotic Manipulation 2.3 Relevant Surveys 3 Monolithic Models 3.1 Single-system Models 3.1.1 Classic Paradigm: Autoregressive Decoding 3.1.2 Model Performance Enhancement 3.1.3 Inference Efficiency Optimization 3.2 Dual-system Models 3.2.1 Cascade-based Methods 3.2.2 Parallel-based Methods 4 Hierarchical Models 4.1 Planner-Only 4.1.1 Program-based Methods 4.1.2 Keypoint-based Methods 4.1.3 Subtask-based Methods 4.2 Planner+Policy 4.2.1 Keypoint-based Methods 4.2.2 Subtask-based Methods 4.3 Comparison: Monolithic vs. Hierarchical 5 Other Advanced Field 5.1 Reinforcement Learning-based Methods 5.2 Training-Free Methods 5.3 Learning from Human Videos 5.4 World Model-based VLA 6 Characteristics of VLA Models 6.1 Multimodal Fusion 6.2 Instruction Following 6.3 Multi-Dimensional Generalization 7 Datasets and Benchmarks 7.1 Real-world Robot Datasets 7.2 Simulation Datasets and Benchmarks 7.3 Human Behavior Datas…

**Method / approach.** Methods 3.2.2 Parallel-based Methods 4 Hierarchical Models 4.1 Planner-Only 4.1.1 Program-based Methods 4.1.2 Keypoint-based Methods 4.1.3 Subtask-based Methods 4.2 Planner+Policy 4.2.1 Keypoint-based Methods 4.2.2 Subtask-based Methods 4.3 Comparison: Monolithic vs. Hierarchical 5 Other Advanced Field 5.1 Reinforcement Learning-based Methods 5.2 Training-Free Methods 5.3 Learning from Human Videos 5.4 World Model-based VLA 6 Characteristics of VLA Models 6.1 Multimodal Fusion 6.2 Instruction Following 6.3 Multi-Dimensional Generalization 7 Datasets and Benchmarks 7.1 Real-world Robot Datasets 7.2 Simulation Datasets and Benchmarks 7.3 Human Behavior Datasets 7.4 Embodied Datasets and Benchmarks 8 Future Directions 9 Conclusion Large VLM-based Vision-Language-Action Models for Robotic Manipulation: A Survey Rui Shao, Wei Li, Lingsen Zhang, Renshan Zhang, Zhiyang Liu, Ran Chen, Liqiang Nie Rui Shao, Wei Li, Lin…

**Results.** Empirically, RT-2 shows a dramatically stronger semantic understanding ability. Compared to RT-1 [ 83 ] , RT-2 [ 27 ] generalizes to novel objects and unseen instructions (e.g., placing an object on a particular number) and can perform basic reasoning (choosing the smallest or closest object). In other words, the large-scale vision-language pretraining imbues the robotic policy with real-world knowledge and stronger language grounding that earlier models lack. Following RT-2’s demonstration of how Internet-scale VLM pretraining can boost robotic control, more VLA models have emerged. For example, π 0 \pi_{0} [ 29 ] adopts a flow-matching architecture on top of a pretrained VLM, trained on diverse dexterous robot datasets, which yields strong zero-shot generalization and easy adaptation to new tasks via fine-tuning. In addition, OpenVLA [ 26 ] has been released as a 7B open-source VLA model pretrained on approximately 970k real-w…

**Conclusion.** Conclusion Large VLM-based Vision-Language-Action Models for Robotic Manipulation: A Survey Rui Shao, Wei Li, Lingsen Zhang, Renshan Zhang, Zhiyang Liu, Ran Chen, Liqiang Nie Rui Shao, Wei Li, Lingsen Zhang, Renshan Zhang, Zhiyang Liu, Ran Chen and Liqiang Nie are with the School of Computer Science and Technology, Harbin Institute of Technology (Shenzhen), China, 518055 (e-mail: shaorui@hit.edu.cn, {liwei2024, zls030726, zhangrenshan, 25s151095, 220310324}@stu.hit.edu.cn, nieliqiang@gmail.com). Abstract Robotic manipulation, as a critical frontier in robotics and embodied AI, demands precise motor control and integrated understanding of visual and semantic cues in dynamic environments. Traditional approaches, grounded in predefi…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[vla]]
- **Raw:** `raw/arxiv/2508.13073v2.md` · `raw/arxiv/2508.13073v2.fulltext.md`
