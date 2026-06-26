---
type: concept
tags: [agents, reasoning, inference-time, long-cot]
created: 2026-06-22
updated: 2026-06-22
census_count: 289
kind: domain
---

# Reasoning models (inference-time reasoning)

*Models trained to think before answering — long chain-of-thought, test-time compute scaling, and RL-on-reasoning. The substrate that made strong agents possible.*

## What it is
Models (o1/o3 and open successors like DeepSeek-R1, GLM-4.5, Kimi K2) that spend inference-time compute on extended reasoning before producing an answer, typically trained with RL on verifiable rewards ([[rlvr]]). Agents are, in large part, reasoning models run in a loop with tools and memory.

## Why it matters
The single biggest capability shift behind the 2025–26 agent surge. For the radar, the load-bearing question is **how much agentic capability comes from the base reasoning model vs the scaffold** — it determines whether you invest in better models or better orchestration. (The [[agentic-ai|"small models are enough for agents"]] argument is the counterweight.)

## What the evidence shows
**2025 foundations.** The year's most important — and most sobering — result: **RLVR mostly sharpens what the base model can already do** (better pass@1) while *shrinking* the set of solvable problems (worse pass@256 coverage); it rarely elicits genuinely new reasoning (→ [[2025-04-18-arxiv-2504-13837v5-does-reinforcement-learning-really-incentivize-reasoning-capacity-in]]). The reasoning-model paradigm then went **open and agentic**: GLM-4.5 (ARC — agentic/reasoning/coding, with science RL on GPQA-Diamond → [[2025-08-08-arxiv-2508-06471v1-glm-4-5-agentic-reasoning-and-coding-arc]]) and Kimi K2 (MuonClip optimizer + large-scale agentic data synthesis + joint RL → [[2025-07-28-arxiv-2507-20534v2-kimi-k2-open-agentic-intelligence]]) brought frontier reasoning to open weights. A safety thread ran alongside: monitoring a model's chain-of-thought catches reward-hacking — but training against the monitor teaches obfuscation (→ [[2025-03-14-arxiv-2503-11926v1-monitoring-reasoning-models-for-misbehavior-and-the-risks]]; see [[agent-security]]).
- The bridge to agents: reasoning + retrieval (Search-o1 → [[agentic-rag]]) and reasoning + tools ([[agentic-rl]]) are how a reasoning model becomes an agent.

## Relationships
- commentary: [[lilian-weng]] ("Why We Think" — the canonical explainer → [[2025-05-01-blog-weng-why-we-think]]), [[demis-hassabis]], [[jeff-dean]]
- verification asymmetry / RL framing: [[jason-wei]] → [[2025-07-15-blog-wei-asymmetry-of-verification]]
- debate: [[debate-llms-path-to-agi]] ([[yann-lecun]] vs [[sonya-huang]])
- substrate for [[agentic-ai]], [[agentic-rl]], [[deep-research-agents]]
- methods: [[chain-of-thought]], [[mcts]], [[rlvr]]
- exemplars: [[openai-o1]], [[openai-o3]], [[deepseek]], [[glm-45]], [[kimi-k2]]
- evaluated on [[aime]], [[gpqa]]
- explained by [[sebastian-raschka]] (RL-for-reasoning teardowns)
- produced by [[post-training]] (reasoning RL) on bases from [[pretraining]]; supply side [[frontier-model-training]]
- economic counterpart [[small-language-models]] (distilled small reasoners, test-time scaling)

## Key 2025 papers (citation-ranked)
- **852** · [[2025-04-18-arxiv-2504-13837v5-does-reinforcement-learning-really-incentivize-reasoning-capacity-in|Does Reinforcement Learning Really Incentivize Reasoning Capacity in LLMs Beyon...]]
- **429** · [[2025-01-09-arxiv-2501-05366v1-search-o1-agentic-search-enhanced-large-reasoning-models|Search-o1: Agentic Search-Enhanced Large Reasoning Models]]
- **358** · [[2025-08-08-arxiv-2508-06471v1-glm-4-5-agentic-reasoning-and-coding-arc|GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models]]
- **296** · [[2025-07-28-arxiv-2507-20534v2-kimi-k2-open-agentic-intelligence|Kimi K2: Open Agentic Intelligence]]
- **263** · [[2025-07-01-arxiv-2507-01006v6-glm-4-5v-and-glm-4-1v-thinking|GLM-4.5V and GLM-4.1V-Thinking: Towards Versatile Multimodal Reasoning with Sca...]]
- **243** · [[2025-03-14-arxiv-2503-11926v1-monitoring-reasoning-models-for-misbehavior-and-the-risks|Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation]]
- **169** · [[2025-09-24-arxiv-2509-20328v2-video-models-are-zero-shot-learners-and-reasoners|Video models are zero-shot learners and reasoners]]
- **167** · [[2025-04-28-arxiv-2504-19678v2-from-llm-reasoning-to-autonomous-ai-agents-a|From LLM Reasoning to Autonomous AI Agents: A Comprehensive Review]]
