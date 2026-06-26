---
type: source
source_type: blog
title: "The State of Reinforcement Learning for LLM Reasoning"
author: Sebastian Raschka
outlet: Ahead of AI
url: https://magazine.sebastianraschka.com/p/the-state-of-llm-reasoning-model-training
resource: https://magazine.sebastianraschka.com/p/the-state-of-llm-reasoning-model-training
date: 2025-04-19
stake: Educator/author (Build a Large Language Model From Scratch); independent researcher (Raschka AI Research / RAIR Lab) — low commercial stake
ingested: 2026-06-22
tags: [perspective, agentic-rl, reasoning-models, grpo, ppo, rlvr, deepseek]
---

# The State of Reinforcement Learning for LLM Reasoning

**Blog** · Sebastian Raschka (Ahead of AI) · 2025-04-19 · [link](https://magazine.sebastianraschka.com/p/the-state-of-llm-reasoning-model-training)

**The take (attributed):** Raschka's definitive technical explainer of the **RLHF → PPO → GRPO → RLVR** lineage. His sharpest stance: **GRPO is an *efficiency* play, not magic** ("the key motivation here is to improve computational efficiency"), and he's openly skeptical that **RL is the sole cause of reasoning** — the "Aha moment" may be "inherited from pre-training."

**Stake:** Independent educator/author writing the from-scratch reasoning book — he implements these algorithms himself, so his read on PPO/GRPO mechanics is first-hand and unusually grounded. Low commercial stake.

## Argument
- **Macro thesis:** conventional scaling is plateauing (muted [[gpt-5|GPT-4.5]] and [[llama|Llama 4]] receptions "suggest we are approaching the limits of what scaling model size and data alone can achieve"); RL-for-reasoning is where gains now live ([[openai-o3|o3]] "used 10× more training compute compared to o1"). "I expect reasoning-focused post-training to become standard practice."
- **[[ppo|PPO]] (the workhorse):** conservative by design — clipped loss + KL penalty to the SFT reference + entropy bonus. The expensive part: PPO involves **four models** — policy, reward model, critic (value model), reference model — and the reward/critic are "typically the same size as the original model."
- **[[grpo|GRPO]] (the efficiency play):** "a variant of PPO." It **drops the critic** and instead "samples multiple answers from the policy model itself and uses their relative quality to compute the advantages." Repeated stance: "RLVR does not strictly require the GRPO algorithm"; GRPO "simply happens to be efficient and to perform well."
- **GRPO's flaws (recurring critique):** length bias ("GRPO divides the advantage by the length of the response... so the model learns to generate longer bad answers") and difficulty-level bias (std-dev normalization overweights low-variance questions). Endorses **Dr. GRPO** (removes both normalizations) and **DAPO** (clip-higher, dynamic sampling, token-level loss, overlong reward shaping).
- **[[rlvr|RLVR]] (the unlock):** "In contrast to standard RLHF, RLVR bypasses the need for a reward model" — binary correct/wrong from deterministic tools (calculators, compilers). DeepSeek-R1 = RLVR + GRPO, eliminating *two* expensive models. DeepSeek went rule-based because neural reward models "may suffer from reward hacking in the large-scale reinforcement learning process."
- **Is reasoning solely due to RL? (his most pointed stance — leans skeptical):** base models like Qwen2.5 "already show strong reasoning and even the 'Aha moment' without any RL"; his own V3-base-vs-R1 comparisons reinforce this. Settled verdict: "RL definitely turns simple base models into reasoning models. However, it's not the only way."
- **Long-incorrect-answers thesis:** verbose CoT is partly a training artifact — with a negative reward, "longer responses can dilute the penalty per individual token." (Honest caveat he quotes: this PPO analysis is "not applicable to GRPO.")
- **Skeptic's coda ("A Sober Look"):** many reported RL gains "might just be noise"; AIME24 is so unstable "just changing a random seed can shift scores by several percentage points." Benefits "have been overstated and better evaluation standards are needed." (Feeds [[agent-evaluation]].)

## Why it matters / where it cuts
The radar's best from-first-principles account of the [[agentic-rl|RL-for-LLMs]] stack that underpins every modern reasoning/agent model — the [[ppo|PPO]]/[[grpo|GRPO]]/[[rlvr|RLVR]] vocabulary, in his own words. Notably *more skeptical* than the field consensus: he treats GRPO as a memory optimization (not a reasoning breakthrough) and doubts RL is the sole source of reasoning — a useful counterweight to RL-triumphalism. Pairs with [[nathan-lambert]]'s "reasoning comes from scaled RL, not search" — they agree RL is real but Raschka stresses the pre-training contribution more.

## Graph
- **Author:** [[sebastian-raschka]]
- **Concepts:** [[agentic-rl]] · [[reasoning-models]] · [[agent-evaluation]]
- **Entities:** [[grpo]] · [[ppo]] · [[rlvr]] · [[deepseek]] · [[openai-o3]] · [[qwen]]
- **Raw:** `raw/blogs/2025-04-19-sebastian-raschka-state-of-rl-for-llm-reasoning.md`
