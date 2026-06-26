---
type: entity
entity_type: model
tags: [agents, model]
created: 2026-06-21
updated: 2026-06-22
census_count: 134
---

# DeepSeek

*Open-weight LLM family notable for strong reasoning at low cost — the most-used RL post-training base in 2025–26 agent research.*

## What it is
DeepSeek is a family of open-weight LLMs from the Chinese lab DeepSeek, noted for strong reasoning performance at competitive cost. The R1 recipe (GRPO + verifiable rewards) made it the de-facto base model for agentic RL research. Mentioned in ~134 of 2026 H1 census papers.

## Why it matters
DeepSeek demonstrated that frontier-level reasoning doesn't require a closed lab's training budget — reshaping the economics of enterprise AI deployment. Its RL recipe is now the standard starting point for teams training task-specific agents.

## Relationships
- base for [[agentic-rl]], [[tool-use]]
- exemplifies [[mixture-of-experts]], [[distillation]], [[post-training]] (the R1 recipe)
- R1-Distill (1.5–8B) is a flagship [[small-language-models]] family; R1-Distill-Qwen-7B beats GPT-4o/Claude-3.5 on reasoning

## Cited by (2025 deep notes)
- **309** · [[2025-04-15-arxiv-2504-11536v2-retool-reinforcement-learning-for-strategic-tool-use-in|ReTool: Reinforcement Learning for Strategic Tool Use in LLMs]]
- **279** · [[2025-04-30-arxiv-2504-21776v2-webthinker-empowering-large-reasoning-models-with-deep-research|WebThinker: Empowering Large Reasoning Models with Deep Research Capability]]
- **218** · [[2025-04-14-arxiv-2504-10458v4-gui-r1-a-generalist-r1-style-vision-language|GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents]]
- **143** · [[2025-03-11-arxiv-2503-08679v6-chain-of-thought-reasoning-in-the-wild-is|Chain-of-Thought Reasoning In The Wild Is Not Always Faithful]]
- **132** · [[2025-03-27-arxiv-2503-21614v2-a-survey-of-efficient-reasoning-for-large-reasoning|A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimo...]]
- **122** · [[2025-03-27-arxiv-2503-21620v5-ui-r1-enhancing-efficient-action-prediction-of-gui|UI-R1: Enhancing Efficient Action Prediction of GUI Agents by Reinforcement L...]]
- **113** · [[2025-02-07-arxiv-2502-04644v2-agentic-reasoning-a-streamlined-framework-for-enhancing-llm|Agentic Reasoning: A Streamlined Framework for Enhancing LLM Reasoning with A...]]
- **112** · [[2025-04-12-arxiv-2504-09037v4-a-survey-of-frontiers-in-llm-reasoning-inference|A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason...]]
