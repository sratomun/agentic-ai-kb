---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Survey: Learning Embodied Intelligence from Physical Simulators and World Models"
authors: Xiaoxiao Long, Qingrui Zhao, Kaiwen Zhang, Zihao Zhang et al.
url: https://arxiv.org/abs/2507.00917v3
date: 2025-07-01
citationCount: 47
influentialCitationCount: 3
velocity: 4.02
ingested: 2026-06-22
tags: [coding-agents, embodied-agents, arxiv, 2025, cited]
---

# A Survey: Learning Embodied Intelligence from Physical Simulators and World Models

**arXiv [2507.00917v3](https://arxiv.org/abs/2507.00917v3)** · 2025-07-01 · **47 citations** (3 influential · 4.02/mo) · Xiaoxiao Long, Qingrui Zhao, Kaiwen Zhang, Zihao Zhang et al.

## Abstract
The pursuit of artificial general intelligence (AGI) has placed embodied intelligence at the forefront of robotics research. Embodied intelligence focuses on agents capable of perceiving, reasoning, and acting within the physical world. Achieving robust embodied intelligence requires not only advanced perception and control, but also the ability to ground abstract cognition in real-world interactions. Two foundational technologies, physical simulators and world models, have emerged as critical enablers in this quest. Physical simulators provide controlled, high-fidelity environments for training and evaluating robotic agents, allowing safe and efficient development of complex behaviors. In contrast, world models empower robots with internal representations of their surroundings, enabling predictive planning and adaptive decision-making beyond direct sensory input. This survey systematically reviews recent advances in learning embodied AI through the integration of physical simulators and world models. We analyze their complementary roles in enhancing autonomy, adaptability, and generalization in intelligent robots, and discuss the interplay between external simulation and internal modeling in bridging the gap between simulated training and real-world deployment. By synthesizing current progress and identifying open challenges, this survey aims to provide a comprehensive perspective on the path toward more capable and generalizable embodied AI systems. We also maintain an active repository that contains up-to-date literature and open-source projects at https://github.com/NJU3DV-LoongGroup/Embodied-World-Models-Survey.

## From the paper (full-text excerpts)
**Introduction.** Introduction 1.1 Overview 1.2 Scope and Contributions 1.3 Structure 2 Levels of Intelligent Robot 2.1 Level Criteria 2.2 Level Factors 2.3 Classification Levels 2.3.1 IR-L0: Basic Execution Level 2.3.2 IR-L1: Programmatic Response Level 2.3.3 IR-L2: Basic Perception and Adaptation Level 2.3.4 IR-L3: Humanoid Cognition and Collaboration Level 2.3.5 IR-L4: Fully Autonomous Level 3 Robotic Mobility, Dexterity and Interaction 3.1 Related Robotic Techniques 3.1.1 Model Predictive Control, MPC 3.1.2 Whole-Body Control, WBC 3.1.3 Reinforcement Learning 3.1.4 Imitation Learning 3.1.5 Visual-Language-Action Models, VLA 3.2 Robotic Locomotion 3.2.1 Legged Locomotion 3.2.2 Fall Protection and Recovery 3.3 Robotic Manipulation 3.3.1 Unimanual Manipulation Task 3.3.2 Bimanual Manipulation Task 3.3.3 Whole-Body Manipulation Control 3.3.4 Foundation Models in Humanoid Robot Manipulation 3.4 Human-Robot Interaction 3.4.1 Cognitive Collaboration: Understanding and Aligning with Human Cognition 3.4.2 Physical Reliability…

**Method / approach.** Method) simulation 4.2.7 Differentiable physics 4.3 Rendering Capabilities 4.3.1 Rendering Engine 4.3.2 Ray Tracing 4.3.3 Physically-based Rendering 4.3.4 Parallel Rendering 4.4 Sensor and Joint Component Types 4.5 Discussions and Future Perspectives 4.5.1 Advantages of Simulators 4.5.2 Challenges of Simulators 4.5.3 Future Perspectives 5 World Models 5.1 Representative Architectures of World Models 5.2 Core Roles of World Models 5.2.1 World Models as Neural Simulator 5.2.2 World Models as Dynamic Models 5.2.3 World Models as Reward Models 6 World Models for Intelligent Agents 6.1 World Models for Autonomous Driving 6.1.1 WMs as Neural Simulators for Autonomous Driving 6.1.2 WMs as Dynamic Models for Autonomous Driving 6.1.3 WMs as Reward Models for Autonomous Driving 6.1.4 Technical Trends and Implications 6.2 World Models for Articulated Robots 6.2.1 WMs as Neural Simulators for Articulated Robots 6.2.2 WMs as…

**Results.** experimentation. Unlike simulators, world models offer internal representations of the environment, enabling robots to autonomously simulate, predict, and plan actions within their cognitive framework. Following NVIDIA’s definition, world models are ”generative AI models that understand the dynamics of the real world, including physics and spatial properties” [ 17 ] . This concept gained significant attention with Ha and Schmidhuber’s seminal work [ 18 ] , which demonstrated how agents could learn compact environmental representations for internal planning. The synergy between simulators and world models enhances robots’ autonomy, adaptability, and task performance across diverse scenarios. This paper will explore the interplay between robot control algorithms, simulators, and world models. By examining how simulators provide a structured, external environment for training and how world models create internal representations for m…

**Conclusion.** Conclusion A Survey: Learning Embodied Intelligence from Physical Simulators and World Models Xiaoxiao Long ∗ , Qingrui Zhao ∗ , Kaiwen Zhang ∗ , Zihao Zhang ∗ , Dingrui Wang ∗ , Yumeng Liu ∗ , Zhengjie Shu ∗ , Yi Lu ∗ , Shouzheng Wang ∗ , Xinzhe Wei ∗ , Wei Li, Wei Yin, Yao Yao, Jia Pan, Qiu Shen, Ruigang Yang, Xun Cao † , Qionghai Dai ∗ indicates equal contributions. † indicates corresponding authors. Xiaoxiao Long, Qingrui Zhao, Yi Lu, Yao Yao, Qiu Shen, Wei Li and Xun Cao are with the Nanjing University (e-mail: caoxun@nju.edu.cn). Yumeng Liu, Zhengjie Shu and Jia Pan are with the University of Hong Kong. Shouzheng Wang is with the Central South University. Wei Yin is with the Horizon Robotics. Zihao Zhang and Xinzhe Wei are w…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[embodied-agents|Embodied agents]]
- **Raw:** `raw/arxiv/2507.00917v3.md` · `raw/arxiv/2507.00917v3.fulltext.md`
