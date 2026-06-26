---
type: entity
entity_type: person
aliases: [rasbt, Sebastian Raschka PhD]
tags: [agents, person]
affiliation: "Independent — runs Raschka AI Research (RAIR Lab LLC); author & educator; writes 'Ahead of AI' (magazine.sebastianraschka.com). Formerly Staff Research Engineer at Lightning AI; ex-Assistant Professor of Statistics, UW-Madison."
stake: Educator/author ("Build a Large Language Model (From Scratch)", "Build a Reasoning Model (From Scratch)") and independent researcher — low commercial stake; sells books/courses, not a model or fund. The radar's most rigorous *from-scratch implementer* voice on LLM architectures, reasoning, and RL.
url: https://magazine.sebastianraschka.com/
created: 2026-06-22
updated: 2026-06-22
---

# Sebastian Raschka

*Independent researcher, author, and educator who writes the deeply-read "Ahead of AI" — the radar's most implementation-grounded explainer of LLM architectures, reasoning models, and RL-for-LLMs (GRPO/PPO/RLVR). Builds the thing from scratch, then teaches it.*

## Who they are
Sebastian Raschka (handle **rasbt**) is an independent AI researcher and one of the most widely-followed *technical educators* in the LLM space. He runs his own **Raschka AI Research (RAIR) Lab LLC**, writes the **Ahead of AI** magazine (magazine.sebastianraschka.com), and authored the bestselling **Build a Large Language Model (From Scratch)** (translated into 9+ languages) and its 2026 sequel **Build a Reasoning Model (From Scratch)**. Previously a Staff Research Engineer at Lightning AI and an Assistant Professor of Statistics at UW-Madison. His lane is **deep, code-first technical explainers**: how modern LLM architectures, reasoning models, and the RL post-training stack actually work, validated by re-implementing them himself in pure PyTorch.

**Stake:** Independent educator/author — **low commercial stake**. He sells books and courses and does selective consulting; he does not market a model, a lab's product, or an AI fund. His incentive is pedagogical clarity, which makes his framing unusually neutral — but discount the occasional "right tool for the task" / "stay an expert" moralizing as his teaching philosophy, and note he's a transformer/from-scratch traditionalist who may under-weight non-transformer bets. Weight his algorithm-level reads (PPO/GRPO/RLVR mechanics, architecture comparisons) heavily — they're first-hand from his own training runs.

## What they argue (recurring stances)
- **Reasoning is a *specialization*, not a universal upgrade.** "Using reasoning models for everything can be inefficient and expensive" — they're more verbose, costlier, and prone to "overthinking." Use the right type of LLM for the task. ([[2025-02-05-blog-raschka-understanding-reasoning-llms|Understanding Reasoning LLMs]].)
- **[[grpo|GRPO]] is an *efficiency* play, not a reasoning breakthrough.** Its "key motivation... is to improve computational efficiency" — it drops the critic and scores groups of self-sampled answers. "RLVR does not strictly require the GRPO algorithm." He gives real weight to GRPO's *length* and *difficulty* biases and endorses Dr. GRPO / DAPO fixes. ([[2025-04-19-blog-raschka-state-of-rl-for-llm-reasoning|State of RL for LLM Reasoning]].)
- **RL is *not* the sole source of reasoning.** Base models (Qwen2.5, updated DeepSeek-V3) "already show strong reasoning and even the 'Aha moment' without any RL"; it may be "inherited from pre-training." Verdict: "RL definitely turns simple base models into reasoning models. However, it's not the only way." A deliberate counterweight to RL-triumphalism. (Same post.)
- **Skeptical of benchmark theater.** "Benchmaxxing" is his word of 2025: "if the test set is public, it isn't a real test set." Benchmarks are minimum thresholds, not trustworthy rankings — corroborated by his "Sober Look" read that many RL gains "might just be noise" (AIME24 shifts by random seed). ([[2025-12-30-blog-raschka-state-of-llms-2025|State of LLMs 2025]].)
- **The harness, not the model, is increasingly the differentiator.** With vanilla frontier LLMs near-parity, "the harness can often be the distinguishing factor"; "a lot of apparent 'model quality' is really context quality." ([[2026-04-04-blog-raschka-components-of-a-coding-agent|Components of a Coding Agent]].)
- **Progress is shifting from training to the inference/tooling layer.** His 2026 call: "a lot of LLM benchmark and performance progress will come from improved tooling and inference-time scaling rather than from training or the core model itself." ([[2025-12-30-blog-raschka-state-of-llms-2025|State of LLMs 2025]].)
- **The durable competitive moat is proprietary domain data, not bigger models.** General gains will plateau (à la GPT-4→4.5); LLM development is commoditizing as open-weight bases become post-trainable. Selling proprietary data to OpenAI/Anthropic is "short-sighted." (Same post.)
- **Humanist on AI-and-work.** LLMs are "superpowers," not replacements; he still hand-writes code he "cares about." Warns of LLM-driven **burnout** when "the model does all the doing and the human mainly supervises" — chess as the model for sustainable use: AI as a partner. (Same post.)

**Evolution 2025 → 2026:** Early 2025 he's the field's *reasoning explainer* — defining reasoning models, mapping the four build methods, and dissecting the [[deepseek|DeepSeek R1]] / [[rlvr|RLVR]] / [[grpo|GRPO]] unlock from first principles (his most-cited contribution). Through mid-2025 he goes *architecture-comparative* (the Big LLM Architecture Comparison, gpt-oss, Qwen3, attention variants, MoE/MLA/linear-attention hybrids). By late 2025 his year-in-review widens to *industry synthesis* (benchmaxxing, tool use, MCP, private-data moats, the inference-over-training shift). And in 2026 he moves squarely into the **agent layer** — coding agents, harness anatomy, the model-vs-context thesis — tracking the field's own pivot from "build the model" to "wrap the model." Throughout, the constant is *from-scratch implementation* as his epistemics.

## Relationships
- writes at: Ahead of AI (magazine.sebastianraschka.com); runs Raschka AI Research (RAIR Lab LLC); authored "Build a Large Language Model (From Scratch)" and "Build a Reasoning Model (From Scratch)"
- explains / weighs in on: [[reasoning-models]] · [[agentic-rl]] · [[coding-agents]] · [[agentic-ai]] · [[tool-use]] · [[agent-memory]] · [[multi-agent-systems]] · [[agent-evaluation]] · [[agent-protocols]]
- recurring subjects: [[deepseek]] · [[grpo]] · [[ppo]] · [[rlvr]] · [[qwen]] · [[llama]] · [[kimi-k2]] · [[openai-o1]] · [[openai-o3]] · [[gpt-5]] · [[claude]]
- complements [[nathan-lambert]] (both ground the RL/reasoning story; Raschka the *implementer* lens, Lambert the *research-org/governance* lens)
- relates to [[debate-agents-vs-workflows]] · [[agent-evals-state-2026]]

## Writings (agent-relevant, 2025–26)
Captured (deep) source notes are wikilinked; the rest are enumerated for coverage. (His magazine and blog also run many quick model/architecture notes — only the agent/reasoning-relevant long-form pieces are listed.)
- 2025-01-23 — Noteworthy LLM Research Papers of 2024 — https://magazine.sebastianraschka.com/p/ai-research-papers-2024-part-1
- 2025-02-05 — [[2025-02-05-blog-raschka-understanding-reasoning-llms|Understanding Reasoning LLMs]]
- 2025-03-08 — Inference-Time Compute Scaling Methods to Improve Reasoning Models (The State of LLM Reasoning Model Inference, Part 1) — https://magazine.sebastianraschka.com/p/state-of-llm-reasoning-and-inference-scaling
- 2025-03-29 — First Look at Reasoning From Scratch: Chapter 1 — https://magazine.sebastianraschka.com/p/first-look-at-reasoning-from-scratch
- 2025-04-19 — [[2025-04-19-blog-raschka-state-of-rl-for-llm-reasoning|The State of Reinforcement Learning for LLM Reasoning (GRPO)]]
- 2025-06-17 — Understanding and Coding the KV Cache in LLMs from Scratch — https://magazine.sebastianraschka.com/p/coding-the-kv-cache-in-llms
- 2025-07-01 — LLM Research Papers: The 2025 List (January to June) — https://magazine.sebastianraschka.com/p/llm-research-papers-2025-list-one
- 2025-07-19 — The Big LLM Architecture Comparison (DeepSeek V3 → GLM) — https://magazine.sebastianraschka.com/p/the-big-llm-architecture-comparison
- 2025-08-09 — From GPT-2 to gpt-oss: Analyzing the Architectural Advances — https://magazine.sebastianraschka.com/p/from-gpt-2-to-gpt-oss-analyzing-the
- 2025-09-06 — Understanding and Implementing Qwen3 From Scratch — https://magazine.sebastianraschka.com/p/qwen3-from-scratch
- 2025-10-05 — Understanding the 4 Main Approaches to LLM Evaluation (From Scratch) — https://magazine.sebastianraschka.com/p/llm-evaluation-4-approaches
- 2025-11-04 — Beyond Standard LLMs (linear-attention hybrids, text diffusion, code world models, recursive transformers) — https://magazine.sebastianraschka.com/p/beyond-standard-llms
- 2025-12-03 — From DeepSeek V3 to V3.2: Architecture, Sparse Attention, and RL Updates — https://magazine.sebastianraschka.com/p/technical-deepseek
- 2025-12-08 — From Random Forests to RLVR: A Short History of ML/AI Hello Worlds — https://sebastianraschka.com/blog/2025/hello-world-ai.html
- 2025-12-30 — [[2025-12-30-blog-raschka-state-of-llms-2025|The State Of LLMs 2025: Progress, Problems, and Predictions]]
- 2026-01-24 — Categories of Inference-Time Scaling for Improved LLM Reasoning — https://magazine.sebastianraschka.com/p/categories-of-inference-time-scaling  *(paywalled; only preview retrievable)*
- 2026-02-01 — State of AI 2026 with Sebastian Raschka, Nathan Lambert, and Lex Fridman (4.5h interview) — https://sebastianraschka.com/blog/2026/state-of-ai-interview.html
- 2026-02-25 — A Dream of Spring for Open-Weight LLMs: 10 Architectures from Jan–Feb 2026 — https://magazine.sebastianraschka.com/p/a-dream-of-spring-for-open-weight
- 2026-03-22 — A Visual Guide to Attention Variants in Modern LLMs — https://magazine.sebastianraschka.com/p/visual-attention-variants
- 2026-04-04 — [[2026-04-04-blog-raschka-components-of-a-coding-agent|Components of A Coding Agent]]
- 2026-04-18 — My Workflow for Understanding LLM Architectures — https://magazine.sebastianraschka.com/p/workflow-for-understanding-llms
- 2026-05-16 — Recent Developments in LLM Architectures: KV Sharing, mHC, and Compressed Attention — https://magazine.sebastianraschka.com/p/recent-developments-in-llm-architectures
- 2026-06-06 — LLM Research Papers: The 2026 List (January to May) — https://magazine.sebastianraschka.com/p/llm-research-papers-2026-part1

## Cited by (posts)
<!-- Auto-maintainable: the source notes that capture this person's posts. -->
- [[2025-02-05-blog-raschka-understanding-reasoning-llms]]
- [[2025-04-19-blog-raschka-state-of-rl-for-llm-reasoning]]
- [[2025-12-30-blog-raschka-state-of-llms-2025]]
- [[2026-04-04-blog-raschka-components-of-a-coding-agent]]
