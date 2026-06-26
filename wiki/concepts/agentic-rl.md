---
type: concept
tags: [agents, reinforcement-learning, tool-use, training]
created: 2026-06-21
updated: 2026-06-22
source_count: 5
---

# Agentic RL

*Reinforcement learning for agents that interleave reasoning with tool execution — and the specific pathologies of training in that setting.*

## What it is
The training paradigm behind capable agents: RL (typically with verifiable rewards) over multi-turn trajectories that mix reasoning steps and tool calls. It spans reward design, rollout strategy, and credit assignment across long, sparse-reward episodes. The field has moved past "just apply [[grpo|GRPO]]" toward diagnosing why long-horizon, tool-integrated training is hard.

## Why it matters
The practical levers here are **cost and reliability, not just accuracy**: teaching agents to skip unnecessary tool calls (18–25% fewer), to recover from the one irrecoverable step that dooms a trajectory, and to treat safety as a graded reward rather than a refusal. If you're funding agent training or choosing a post-training recipe, these are the knobs that move the bill and the failure rate.

## What the evidence shows
**2025 foundations.** RLVR ([[rlvr]] — RL with verifiable rewards) became the default recipe, but the year's most-cited result is a caution: RLVR mostly *sharpens* what the base model can already do (better pass@1) while **shrinking the reasoning boundary** (worse pass@256 coverage), rarely eliciting genuinely new reasoning (→ [[2025-04-18-arxiv-2504-13837v5-does-reinforcement-learning-really-incentivize-reasoning-capacity-in]]). On tool use, **ReTool** showed RL with real-time code execution reaches **67% on AIME vs 40% for text-only RL at far fewer steps** (→ [[2025-04-15-arxiv-2504-11536v2-retool-reinforcement-learning-for-strategic-tool-use-in]]; cf. [[tool-use]]), and **ToolRL** established that *reward design is the lever* (+17% over base, +15% over SFT) (→ [[2025-04-16-arxiv-2504-13958v1-toolrl-reward-is-all-tool-learning-needs]]). The hard problem — credit assignment over long, sparse-reward trajectories — got **GiGPO**'s critic-free step-level credit (+12% ALFWorld, +9% WebShop over [[grpo|GRPO]] → [[2025-05-16-arxiv-2505-10978v3-group-in-group-policy-optimization-for-llm-agent]]) and **RAGEN/StarPO**, which named the "Echo Trap" instability of multi-turn agent RL (→ [[2025-04-24-arxiv-2504-20073v2-ragen-understanding-self-evolution-in-llm-agents-via]]).

**2026 developments.** Work is now fixing specific pathologies: reasoning and tool-use *interfere* when trained in one parameter set — decoupling via separate LoRA (DART) beats joint baselines and nears a 2-agent upper bound (→ [[2026-02-01-arxiv-2602-00994v2-reasoning-vs-tooluse-interference-dart]]); **"tool abuse" is real and fixable** — EAPO cuts tool calls 18–25% while improving accuracy 7–10% vs GRPO (→ [[2026-06-01-arxiv-2606-02132v2-eapo-learning-when-not-to-act]]; cf. [[eapo]]); sparse-reward credit assignment improves by localizing the first irrecoverable step (ELPO → [[2026-02-10-arxiv-2602-09598v1-elpo-error-localized-policy-optimization]]) and oracle-preserving synthetic environments (COVERT → [[2026-04-10-arxiv-2604-09813v1-covert-verifiable-tooluse-data-synthesis]]); and safety becomes a graded rubric reward over whole trajectories (RUBAS → [[2026-06-02-arxiv-2606-04051v1-rubas-rubric-based-rl-agent-safety]]).

## Includes (sub-themes folded here)
Folds in: **RL training infrastructure** — rollout strategies, reward design, multi-turn/agentic RL pipelines (~1,800 papers touch this).

## Relationships
- perspective: [[nathan-lambert]] — long-horizon is scaffolded, not learned ([[2025-06-09-blog-lambert-what-comes-next-rl]])
- cross-refs (methods/benchmarks/models): [[rlvr]] · [[rlhf]] · [[mcts]] · [[chain-of-thought]] · [[ppo]] · [[dpo]]
- methods/entities: [[grpo]], [[dart]], [[eapo]], [[rubas]]
- benchmarks: [[bfcl]]
- feeds: [[self-evolving-agents]], [[agent-security]]
- a training approach for [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **852** · [[2025-04-18-arxiv-2504-13837v5-does-reinforcement-learning-really-incentivize-reasoning-capacity-in|Does Reinforcement Learning Really Incentivize Reasoning Capacity in LLMs Beyon...]]
- **309** · [[2025-04-15-arxiv-2504-11536v2-retool-reinforcement-learning-for-strategic-tool-use-in|ReTool: Reinforcement Learning for Strategic Tool Use in LLMs]]
- **280** · [[2025-04-16-arxiv-2504-13958v1-toolrl-reward-is-all-tool-learning-needs|ToolRL: Reward is All Tool Learning Needs]]
- **268** · [[2025-05-16-arxiv-2505-10978v3-group-in-group-policy-optimization-for-llm-agent|Group-in-Group Policy Optimization for LLM Agent Training]]
- **236** · [[2025-04-24-arxiv-2504-20073v2-ragen-understanding-self-evolution-in-llm-agents-via|RAGEN: Understanding Self-Evolution in LLM Agents via Multi-Turn Reinforcement ...]]
- **220** · [[2025-04-04-arxiv-2504-03160v4-deepresearcher-scaling-deep-research-via-reinforcement-learning-in|DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world ...]]
- **218** · [[2025-04-14-arxiv-2504-10458v4-gui-r1-a-generalist-r1-style-vision-language|GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents]]
- **166** · [[2025-07-03-arxiv-2507-02259v1-memagent-reshaping-long-context-llm-with-multi-conv|MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent]]
