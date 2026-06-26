---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation"
authors: Yuanhang Zhang, Yifu Yuan, Prajwal Gurunath, Ishita Gupta et al.
url: https://arxiv.org/abs/2505.06776v2
date: 2025-05-10
citationCount: 75
influentialCitationCount: 10
velocity: 5.6
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation

**arXiv [2505.06776v2](https://arxiv.org/abs/2505.06776v2)** · 2025-05-10 · **75 citations** (10 influential · 5.6/mo) · Yuanhang Zhang, Yifu Yuan, Prajwal Gurunath, Ishita Gupta et al.

## Abstract
Humanoid loco-manipulation holds transformative potential for daily service and industrial tasks, yet achieving precise, robust whole-body control with 3D end-effector force interaction remains a major challenge. Prior approaches are often limited to lightweight tasks or quadrupedal/wheeled platforms. To overcome these limitations, we propose FALCON, a dual-agent reinforcement-learning-based framework for robust force-adaptive humanoid loco-manipulation. FALCON decomposes whole-body control into two specialized agents: (1) a lower-body agent ensuring stable locomotion under external force disturbances, and (2) an upper-body agent precisely tracking end-effector positions with implicit adaptive force compensation. These two agents are jointly trained in simulation with a force curriculum that progressively escalates the magnitude of external force exerted on the end effector while respecting torque limits. Experiments demonstrate that, compared to the baselines, FALCON achieves 2x more accurate upper-body joint tracking, while maintaining robust locomotion under force disturbances and achieving faster training convergence. Moreover, FALCON enables policy training without embodiment-specific reward or curriculum tuning. Using the same training setup, we obtain policies that are deployed across multiple humanoids, enabling forceful loco-manipulation tasks such as transporting payloads (0-20N force), cart-pulling (0-100N), and door-opening (0-40N) in the real world.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Humanoid Loco-Manipulation 2.2 Forceful Interaction in Legged Robots 3 FALCON : Force-Adaptive Humanoid Loco-Manipulation 3.1 Dual-Agent Learning Framework 3.2 Torque-Limit-Aware 3D Force Curriculum Torque-Aware Force Computation: Progressive Force Curriculum: Position Randomization of the Applied Force: 4 Simulation and Real-World Experiments 4.1 Evaluation Criterion 4.2 Baselines 4.3 Simulation Results Loco-Manipulation Performance: Torque-Limit-Aware Force Curriculum Exploration and Learning: 4.4 Real-World Quantatitive Tracking Results 4.5 Real-World Deployment with Teleoperation 4.6 Real-World Deployment with Autonomy 5 Conclusion 6 Limitations A Appendix A.1 Reward Terms A.2 Domain Randomization A.3 Lower-RL-Upper-IK with Force Estimator A.4 Force Measurement A.5 Autonomy Pipeline A.5.1 Perception - Pose Estimation A.5.2 Motion Capture System A.6 Hardware Limits in Real-World Deployment FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation Yuanha…

**Method / approach.** methods by 100% while maintaining robust locomotion performance. • To facilitate the efficient RL training, we design a 3D force curriculum with progressive force application while ensuring joint torque feasibility and maximizing its force-adaptive capability. • We validate FALCON on two different humanoid platforms (Unitree G1, Booster T1), achieving strong cross-platform generalization with minimal tuning overhead. 2 Related Works 2.1 Humanoid Loco-Manipulation Humanoid loco-manipulation remains a challenging control problem in robotics. While traditional model-based methods (e.g., simplified dynamics models and MPC) [ dantec2021whole , sombolestan2024adaptive , li2023dynamic , murooka2021humanoid , bouyarmane2018quadratic , di2018dynamic , kajita2003biped , xue2024full ] offer real-time planning, their reliance on manual design limits flexibility and generalizability. In contrast, learning-based methods—particularly sim-to-real RL—have demonstrated promisin…

**Results.** Experiments 4.1 Evaluation Criterion 4.2 Baselines 4.3 Simulation Results Loco-Manipulation Performance: Torque-Limit-Aware Force Curriculum Exploration and Learning: 4.4 Real-World Quantatitive Tracking Results 4.5 Real-World Deployment with Teleoperation 4.6 Real-World Deployment with Autonomy 5 Conclusion 6 Limitations A Appendix A.1 Reward Terms A.2 Domain Randomization A.3 Lower-RL-Upper-IK with Force Estimator A.4 Force Measurement A.5 Autonomy Pipeline A.5.1 Perception - Pose Estimation A.5.2 Motion Capture System A.6 Hardware Limits in Real-World Deployment FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation Yuanhang Zhang 1 {}^{\textnormal{1}} , Yifu Yuan 1 {}^{\textnormal{1}} , Prajwal Gurunath 1 {}^{\textnormal{1}} , Ishita Gupta 1 {}^{\textnormal{1}} , Shayegan Omidshafiei 2 {}^{\textnormal{2}} Ali-akbar Agha-mohammadi 2 {}^{\textnormal{2}} , Marcell Va…

**Conclusion.** Conclusion 6 Limitations A Appendix A.1 Reward Terms A.2 Domain Randomization A.3 Lower-RL-Upper-IK with Force Estimator A.4 Force Measurement A.5 Autonomy Pipeline A.5.1 Perception - Pose Estimation A.5.2 Motion Capture System A.6 Hardware Limits in Real-World Deployment FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation Yuanhang Zhang 1 {}^{\textnormal{1}} , Yifu Yuan 1 {}^{\textnormal{1}} , Prajwal Gurunath 1 {}^{\textnormal{1}} , Ishita Gupta 1 {}^{\textnormal{1}} , Shayegan Omidshafiei 2 {}^{\textnormal{2}} Ali-akbar Agha-mohammadi 2 {}^{\textnormal{2}} , Marcell Vazquez-Chanlatte 3 {}^{\textnormal{3}} , Liam Pedersen 3 {}^{\textnormal{3}} Tairan He 1 {}^{\textnormal{1}} , Guanya Shi 1 {}…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.06776v2.md` · `raw/arxiv/2505.06776v2.fulltext.md`
