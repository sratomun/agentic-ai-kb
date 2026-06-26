---
type: source
source_type: blog
title: "Understanding Reasoning LLMs"
author: Sebastian Raschka
outlet: Ahead of AI
url: https://magazine.sebastianraschka.com/p/understanding-reasoning-llms
resource: https://magazine.sebastianraschka.com/p/understanding-reasoning-llms
date: 2025-02-05
stake: Educator/author (Build a Large Language Model From Scratch); independent researcher (Raschka AI Research / RAIR Lab) — low commercial stake
ingested: 2026-06-22
tags: [perspective, reasoning-models, agentic-rl, deepseek]
---

# Understanding Reasoning LLMs

**Blog** · Sebastian Raschka (Ahead of AI) · 2025-02-05 · [link](https://magazine.sebastianraschka.com/p/understanding-reasoning-llms)

**The take (attributed):** Raschka argues there are exactly **four ways** to build/improve a reasoning model — inference-time scaling, pure RL, SFT+RL, and SFT/distillation — and that **reasoning is a *specialization*, not a universal upgrade**: "using reasoning models for everything can be inefficient and expensive."

**Stake:** Independent educator/author — low commercial stake. He's selling books (LLMs From Scratch), not a model or a fund, so his framing is pedagogical rather than promotional. Weight his technical breakdowns heavily; the value judgments ("right tool for the task") are his teaching philosophy.

## Argument
- **Definition (narrow on purpose):** reasoning = "answering questions that require complex, multi-step generation with intermediate steps." Factual lookups ("capital of France") explicitly don't count. Reasoning models are "more expensive to use, more verbose, and sometimes more prone to errors due to 'overthinking.'"
- **The [[deepseek|DeepSeek R1]] pipeline as blueprint** — three variants: R1-Zero (pure RL, no SFT — "cold start"), R1 (flagship, SFT+RL), R1-Distill (SFT on R1 outputs into Qwen/Llama).
- **The "Aha moment" is his personal highlight:** R1-Zero developed reasoning from *pure RL* with only two rewards — an accuracy reward (LeetCode compiler / deterministic math checks) and a format reward (LLM judge for `<think>` tags). "DeepSeek was the first to demonstrate (or at least publish) this approach."
- **His practical recommendation:** "in practical model development, RL + SFT is the preferred approach as it leads to stronger reasoning models." R1's pipeline: cold-start SFT data → instruction tuning → RL (with language-consistency reward) → 600K CoT + 200K knowledge SFT → final SFT+RL.
- **Distillation — useful but limited:** "distillation does not drive innovation or produce the next generation of reasoning models. For instance, distillation always depends on an existing, stronger model." Empirical: "distillation is far more effective than pure RL for smaller models."
- **On o1/o3 (flagged as suspicion):** o1 likely uses RL+SFT *plus* inference-time scaling, on a weaker base than R1, "which explains why DeepSeek-R1 performs so well while remaining relatively cheap at inference time." Next frontier: combine RL+SFT with inference-time scaling.
- **Pushes back on the cost narrative:** the "~$6 million" figure conflates V3 and R1; DeepSeek "never disclosed the exact GPU hours or development cost for R1, so any cost estimates remain pure speculation."
- **Budget optimism:** Sky-T1 (32B, 17K SFT samples, ~$450, "roughly on par with o1"); TinyZero (3B, pure-RL R1-Zero replication, <$30, shows "emergent self-verification"); journey learning (training on *incorrect* solution paths too).

## Why it matters / where it cuts
This is the radar's cleanest pedagogical map of *how reasoning models are actually built* — the foundation for [[reasoning-models]] and the [[agentic-rl]] training stack. His "right tool for the task" stance is the practitioner counter to reasoning-everywhere hype, and his cost-narrative skepticism is a useful corrective to the DeepSeek-panic coverage. Sets up his deeper [[2025-04-19-blog-raschka-state-of-rl-for-llm-reasoning|GRPO/PPO state-of-RL post]].

## Graph
- **Author:** [[sebastian-raschka]]
- **Concepts:** [[reasoning-models]] · [[agentic-rl]]
- **Entities:** [[deepseek]] · [[rlvr]] · [[qwen]] · [[llama]]
- **Raw:** `raw/blogs/2025-02-05-sebastian-raschka-understanding-reasoning-llms.md`
