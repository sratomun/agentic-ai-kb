---
type: source
source_type: blog
title: "The State Of LLMs 2025: Progress, Problems, and Predictions"
author: Sebastian Raschka
outlet: Ahead of AI
url: https://magazine.sebastianraschka.com/p/state-of-llms-2025
resource: https://magazine.sebastianraschka.com/p/state-of-llms-2025
date: 2025-12-30
stake: Educator/author (Build a Large Language Model From Scratch); independent researcher (Raschka AI Research / RAIR Lab) — low commercial stake
ingested: 2026-06-22
tags: [perspective, reasoning-models, agentic-rl, rlvr, grpo, tool-use, agent-protocols]
---

# The State Of LLMs 2025: Progress, Problems, and Predictions

**Blog** · Sebastian Raschka (Ahead of AI) · 2025-12-30 · [link](https://magazine.sebastianraschka.com/p/state-of-llms-2025)

**The take (attributed):** Raschka's year-in-review: **2025 was "the year of reasoning, RLVR, and GRPO."** His forward call — **2026's gains will come more from inference-time scaling, tooling, and [[agentic-ai|agentic capabilities]] than from training the core model**, and the durable competitive moat is **proprietary domain data**, not bigger models.

**Stake:** Independent researcher/author — confirms here he runs his own company, stays independent despite full-time offers, and is mid-way through the GRPO chapter of his reasoning book. Low commercial stake; his predictions aren't talking a product book.

## Argument
- **The DeepSeek moment:** [[deepseek|R1]] (Jan 2025) "was a really big deal" — open-weight, comparable to proprietary frontier, and it introduced [[rlvr|RLVR]] + [[grpo|GRPO]]. Triggered the revised cheap-training narrative (~$5M for V3's final run; +$294K for R1 on top), with the caveat that it excludes salaries/experimentation.
- **His focus-point timeline:** 2022 RLHF+PPO → 2023 LoRA SFT → 2024 Mid-Training → **2025 RLVR+GRPO** → (predicted) **2026 RLVR extensions + more inference-time scaling** → **2027 continual learning** (blocked by catastrophic forgetting).
- **GRPO = "research darling of the year."** He confirms from his own from-scratch runs that GRPO modifications "have a huge impact in practice" — bad updates no longer corrupt runs. Lists the specific tricks adopted by Olmo 3 (DAPO / Dr. GRPO) and DeepSeek V3.2.
- **Next for RLVR:** "explanation-scoring" (judging reasoning, not just final answers) — the old PRM idea, historically unsuccessful but revived via DeepSeekMath-V2; plus expansion beyond math/code.
- **Architectures:** SOTA still decoder transformers; open-weight converged on MoE + an efficiency-tweaked attention (GQA/SWA/MLA); linear-scaling tweaks (Gated DeltaNet in Qwen3-Next/[[kimi-k2|Kimi]] Linear, Mamba-2 in Nemotron 3). Transformers stay dominant "for at least a couple more years."
- **Tool use & agents:** hallucination drops "largely" due to [[tool-use]]; gpt-oss built for tool use but "the open-source ecosystem hasn't fully caught up" (security: "would you trust a new intern with this much access?"). [[agent-protocols|MCP]] became the de facto agent standard faster than he expected (joined the Linux Foundation).
- **"Benchmaxxing" — word of the year:** benchmarks gamed; [[llama|Llama 4]] scored well but disappointed in use. "If the test set is public, it isn't a real test set." Benchmarks are minimum thresholds, not rankings. (Feeds [[agent-evaluation]].)
- **Humanist coding stance:** LLMs are "superpowers," not replacements; he still hand-writes code he "cares about." Warns of LLM-driven **burnout** when "the model does all the doing and the human mainly supervises" — chess analogy: AI as a partner, not a replacement.
- **The edge = private data:** general gains will plateau (à la GPT-4→4.5); the moat is domain-specific proprietary data. Companies wisely decline data deals with OpenAI/Anthropic; LLM dev is commoditizing as open-weight bases (DeepSeek V3.2, [[kimi-k2|Kimi K2]], GLM 4.7) become post-trainable.
- **2026 predictions:** consumer diffusion model (Gemini Diffusion first); open-weight adopts local tool use + agentic capabilities; RLVR into chemistry/biology; classical RAG fades for better long-context; "a lot of LLM benchmark and performance progress will come from improved tooling and inference-time scaling rather than from training."

## Why it matters / where it cuts
The single best one-stop synthesis of the 2025 LLM year from a working implementer, and his 2026 call — **progress shifting from the model to the harness/inference layer** — is directly the radar's [[agentic-ai]] thesis. His "edge = private data" and "commoditizing open weights" reads echo (and partly converge with) [[nathan-lambert]]'s open-vs-closed work. The benchmaxxing stance feeds [[agent-evaluation]] and [[agent-evals-state-2026]].

## Graph
- **Author:** [[sebastian-raschka]]
- **Concepts:** [[reasoning-models]] · [[agentic-ai]] · [[agentic-rl]] · [[tool-use]] · [[agent-protocols]] · [[agent-evaluation]]
- **Entities:** [[deepseek]] · [[grpo]] · [[rlvr]] · [[ppo]] · [[kimi-k2]] · [[llama]] · [[qwen]]
- **Raw:** `raw/blogs/2025-12-30-sebastian-raschka-state-of-llms-2025.md`
