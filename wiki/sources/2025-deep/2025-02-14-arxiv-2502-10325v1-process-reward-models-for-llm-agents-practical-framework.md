---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Process Reward Models for LLM Agents: Practical Framework and Directions"
authors: Sanjiban Choudhury
url: https://arxiv.org/abs/2502.10325v1
date: 2025-02-14
citationCount: 66
influentialCitationCount: 4
velocity: 4.08
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Process Reward Models for LLM Agents: Practical Framework and Directions

**arXiv [2502.10325v1](https://arxiv.org/abs/2502.10325v1)** · 2025-02-14 · **66 citations** (4 influential · 4.08/mo) · Sanjiban Choudhury

## Abstract
We introduce Agent Process Reward Models (AgentPRM), a simple and scalable framework for training LLM agents to continually improve through interactions. AgentPRM follows a lightweight actor-critic paradigm, using Monte Carlo rollouts to compute reward targets and optimize policies. It requires minimal modifications to existing RLHF pipelines, making it easy to integrate at scale. Beyond AgentPRM, we propose InversePRM, which learns process rewards directly from demonstrations without explicit outcome supervision. We also explore key challenges and opportunities, including exploration, process reward shaping, and model-predictive reasoning. We evaluate on ALFWorld benchmark, show that small 3B models trained with AgentPRM and InversePRM outperform strong GPT-4o baselines, and analyze test-time scaling, reward hacking, and more. Our code is available at: https://github.com/sanjibanc/agent_prm.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Agent Process Reward Models: A Simple Framework 2.1 Formulation Agent Process Reward Models. Distinction from Reasoning Tasks. 2.2 Approach Stage 1: Rollout and Compute Target. Stage 2: Train Process Reward Model. Stage 3: Train Policy via RL. Inference. 2.3 Experiments Setup. Overall Results. Training Curves. Test-time Scaling. Question: Can we measure and mitigate reward hacking? Question: Can we train PRMs on relative vs absolute losses? 3 Inverse Process Reward Models 3.1 Formulation IRL via PRMs. 3.2 Approach Stage 1: Create Positive / Negative Transitions. Stage 2: Training Process Reward Model. Stage 3: Train Policy via RL. 3.3 Experiments Setup. Overall Results. Training Curves. Test-time Scaling. 4 Challenges and Opportunities 4.1 Exploration Strategy 1: Reset Distribution. Strategy 2: Steered Exploration. Strategy 3: Post-hoc Rationalization. 4.2 Process Reward Shaping Strategy 1: Initialize with IL, then do RL. Strategy 2: Process Reward Shaping. 4.3 Model-…

**Method / approach.** method for training process reward models, and InversePRM (Sec. 3 ), which learns PRMs directly from demonstrations. Our implementation is a light-weight Gym wrapper around OpenInstruct 1 1 1 https://github.com/allenai/open-instruct [ 13 ] , making it easy to integrate with existing RLHF pipelines. 2. Evaluation and Analysis. We evaluate on a text game benchmark ALFWorld [ 15 ] and find: • AgentPRM enables small (3B) models to outperform strong GPT-4o baselines. We analyze training curves, test-time scaling, reward hacking, and absolute v/s relative loss (Sec. 2.3 ). • InversePRM achieves near expert performance in a single iteration, significantly outperforming SFT and being more sample-efficient than AgentPRM (Sec. 3.3 ). 3. Challenges and Opportunities. We discuss challenges and new research opportunities in: • Exploration : We explore resets and steered exploration to accelerate training (Sec. 4.1 ). • Process Reward Shaping : We us…

**Results.** Experiments Setup. Overall Results. Training Curves. Test-time Scaling. Question: Can we measure and mitigate reward hacking? Question: Can we train PRMs on relative vs absolute losses? 3 Inverse Process Reward Models 3.1 Formulation IRL via PRMs. 3.2 Approach Stage 1: Create Positive / Negative Transitions. Stage 2: Training Process Reward Model. Stage 3: Train Policy via RL. 3.3 Experiments Setup. Overall Results. Training Curves. Test-time Scaling. 4 Challenges and Opportunities 4.1 Exploration Strategy 1: Reset Distribution. Strategy 2: Steered Exploration. Strategy 3: Post-hoc Rationalization. 4.2 Process Reward Shaping Strategy 1: Initialize with IL, then do RL. Strategy 2: Process Reward Shaping. 4.3 Model-Predictive Reasoning Strategy: Deliberative Reasoning with a Learned World Model. 5 Related Work 6 Conclusion Process Reward Models for LLM A…

**Conclusion.** Conclusion Process Reward Models for LLM Agents: Practical Framework and Directions Sanjiban Choudhury Cornell University sanjibanc@cornell.edu Abstract We introduce Agent Process Reward Models ( AgentPRM ), a simple and scalable framework for training LLM agents to continually improve through interactions. AgentPRM follows a lightweight actor-critic paradigm, using Monte Carlo rollouts to compute reward targets and optimize policies. It requires minimal modifications to existing RLHF pipelines, making it easy to integrate at scale. Beyond AgentPRM , we propose InversePRM , which learns process rewards directly from demonstrations without explicit outcome supervision. We also explore key challenges and opportunities, includ…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[alfworld]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2502.10325v1.md` · `raw/arxiv/2502.10325v1.fulltext.md`
