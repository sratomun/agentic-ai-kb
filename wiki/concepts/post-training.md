---
type: concept
tags: [agents, frontier-models, post-training, alignment]
created: 2026-06-22
updated: 2026-06-22
kind: hub
---

# Post-training

*Everything done to a base model after pre-training to make it useful, steerable, and aligned: supervised fine-tuning → preference optimization → reinforcement learning. The stage where most of 2025–26's capability gains landed.*

## What it is
The recipe that turns a raw base model into a product. The canonical pipeline is three moves: [[sft|supervised fine-tuning]] on high-quality demonstrations, preference optimization ([[rlhf]], [[dpo]]) against a [[reward-modeling|reward model]] or AI feedback ([[constitutional-ai]]), and reinforcement learning ([[ppo]], [[grpo]], [[rlvr]]) — increasingly RL on verifiable rewards for reasoning. This hub aggregates the method nodes the wiki already holds; it's the connective tissue that makes them one story rather than scattered techniques.

## Why it matters
Post-training is where the marginal dollar of compute now goes, because pre-training scaling is flattening and this is where reasoning, tool-use, and alignment are actually installed. For the exec the key nuance is the ceiling: RL post-training mostly *sharpens* what the base model can already do (better pass@1) rather than creating new capability — so the base model still caps you, but the recipe is what separates a usable frontier model from an inert one. The recipe is also the most *transferable* part of the stack: DeepSeek-R1 made a frontier-grade post-training process legible enough to copy.

## What the evidence shows
**Foundations.** The SFT → reward-model → RLHF pipeline was defined by InstructGPT (arXiv:2203.02155). The open blueprint is Tülu 3, which documented a full open post-training recipe combining SFT, DPO, and RLVR (arXiv:2411.15124); Llama 2/3 (arXiv:2307.09288, arXiv:2407.21783) and DeepSeek-R1 (arXiv:2501.12948) are the other reference recipes. The four post-training routes are dissected in [[2025-02-05-blog-raschka-understanding-reasoning-llms]], and the R1 recipe in [[2025-01-21-blog-lambert-deepseek-r1-recipe]].

**Recent developments.** RL post-training is now discussed as its own scaling regime → [[2025-10-20-blog-lambert-how-to-scale-rl]], [[2025-06-09-blog-lambert-what-comes-next-rl]]; the taxonomy of next-gen reasoners is in [[2025-06-04-blog-lambert-taxonomy-next-gen-reasoners]]. Verification-centric framing (rewards are easy to check, hard to fake) from [[2025-07-15-blog-wei-asymmetry-of-verification]].

## Includes (method nodes aggregated here)
[[sft]], [[reward-modeling]], [[rlhf]], [[dpo]], [[ppo]], [[grpo]], [[rlvr]], [[constitutional-ai]], [[chain-of-thought]].

## Relationships
- stage of [[frontier-model-training]]; consumes base models from [[pretraining]]
- produces [[reasoning-models]]; method overlap with [[agentic-rl]]
- methods: [[sft]], [[rlhf]], [[dpo]], [[ppo]], [[grpo]], [[rlvr]], [[reward-modeling]], [[constitutional-ai]]
- alignment angle links [[agent-security]], [[constitutional-ai]]
- specializes [[small-language-models]] (LoRA/QLoRA/RL agent specialists)
- on-device fine-tuning branch: [[on-device-agents]]
- explained by [[sebastian-raschka]], [[nathan-lambert]], [[jason-wei]]

## Key papers (full-text ingested)
- [[2022-03-04-arxiv-2203-02155-instructgpt|InstructGPT]] — 3-step SFT→RM→PPO; 1.3B aligned preferred over 175B GPT-3
- [[2024-11-22-arxiv-2411-15124-tulu-3|Tülu 3]] — open recipe; 8B SFT→DPO→RLVR lifts GSM8K 76→88%
- [[2023-07-18-arxiv-2307-09288-llama-2|Llama 2]] — RLHF with two reward models (helpful + safe); rejection sampling + PPO
- [[2026-06-22-arxiv-2407-21783-llama-3-herd|Llama 3 Herd]] — SFT + DPO + rejection sampling at frontier scale
- [[2026-06-22-arxiv-2501-12948-deepseek-r1|DeepSeek-R1]] — multi-stage RL recipe; distillation beats small-model RL
