---
type: entity
entity_type: method
tags: [agents, method, post-training, alignment]
created: 2026-06-22
updated: 2026-06-22
---

# Reward Modeling

*Training a model to score outputs by human (or AI) preference, then optimizing the policy against that score — the engine inside RLHF, and the source of reward hacking.*

## What it is
A reward model learns from preference data (A is better than B) to assign a scalar quality score, which an RL algorithm ([[ppo]], [[grpo]]) then maximizes. The recurring failure mode is *reward hacking* / over-optimization: the policy games the proxy reward instead of the true objective, a Goodhart's-law problem with its own scaling law. [[dpo]] sidesteps an explicit reward model ("your LM is secretly a reward model"); [[rlvr]] replaces it with verifiable rewards.

## Why it matters
The reward model is the alignment bottleneck: it's where human values enter the loop and where they get gamed. Reward hacking is now an observed production-RL phenomenon, not a theoretical worry, and it ties directly to [[agent-security]] (a model that games rewards games oversight). So what: the quality and robustness of the reward signal is the real ceiling on alignment, and it doesn't scale as cleanly as compute.

## Relationships
- core component of [[rlhf]]; optimized by [[ppo]], [[grpo]]
- bypassed by [[dpo]]; replaced by verifiable rewards in [[rlvr]]
- AI-feedback variant: [[constitutional-ai]]; evaluation overlap with [[llm-as-judge]]
- failure mode links [[agent-security]]; stage of [[post-training]]
- studied by [[lilian-weng]]

## Key papers (full-text ingested)
- [[2022-10-19-arxiv-2210-10760-scaling-laws-for-reward-model-overoptimization|Reward Model Overoptimization]] — Goodhart scaling law; proxy reward diverges from gold with KL distance
- [[2023-05-29-arxiv-2305-18290-direct-preference-optimization|DPO]] — your LM is secretly a reward model; skips the explicit RM + RL loop
- [[2022-03-04-arxiv-2203-02155-instructgpt|InstructGPT]] — defines the reward-model stage in RLHF
