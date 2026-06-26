---
source: https://lilianweng.github.io/posts/2025-05-01-thinking/
author: Lilian Weng (with feedback / direct edits from John Schulman)
outlet: Lil'Log
date: 2025-05-01
captured: 2026-06-22
capture_method: web_fetch (full text)
immutable: true
---

# Why We Think — raw capture

> Immutable source capture. Captured via web_fetch on 2026-06-22; ~40 min read.
> A survey/review of test-time compute ("thinking time") and why it helps.

## Core thesis
Letting a model spend more **test-time compute** before answering — via chain-of-thought,
search/parallel sampling, sequential revision, or latent computation — is a genuinely new axis
for improving intelligence, complementary to model size, training compute, and data. Weng frames
"thinking" as analogous to human System-2 deliberation and formalizes it as **latent-variable
inference**: the reasoning trace is a hidden variable z over which the model marginalizes to
produce better answers. Stated goal: review "how to effectively use test-time compute (i.e.
'thinking time') and why it helps."

## Framework (the survey's pillars)
1. **Motivation** — three lenses for why thinking longer helps:
   - **Psychology**: Kahneman's System 1 (fast/intuitive) vs System 2 (slow/deliberate) from
     *Thinking, Fast and Slow*; thinking time = engaging System 2.
   - **Computation as a resource**: a forward pass has fixed compute (~2× parameters per token;
     ~2× params/sparsity for MoE); CoT lets the model spend *more, variable* flops per answer
     token depending on problem hardness.
   - **Latent-variable modeling**: frame the thought as latent z, optimize the marginal
     P(y|x) = Σ_z p(z|x)P(y|x,z); parallel/search methods sample from the posterior P(z|x,y).
2. **Thinking in Tokens** (the dominant paradigm):
   - **Branching & editing** — parallel sampling (generate many, pick best via verifier / reward /
     majority vote) vs sequential revision (iteratively reflect and correct). Parallel is capped by
     one-shot ability; sequential can fix mistakes but risks breaking correct answers; combine them.
   - **RL for better reasoning** — train on verifiable problems (STEM, code w/ unit tests); the
     o-series and DeepSeek-R1 paradigm.
   - **External tool use** — offload exact sub-steps to code interpreters / search (PAL, Chain of
     Code, ReAct, o3/o4-mini tool use).
   - **Thinking faithfully** — does the CoT reflect the model's real internal reasoning?
3. **Thinking in Continuous Space** — adaptive compute *without* emitting tokens:
   - **Recurrent architecture** (vertical depth): Universal Transformer, Adaptive Computation
     Time, Geiping et al. recurrent-depth.
   - **Thinking / pause tokens** (horizontal): meaningless filler tokens that buy compute (Herel &
     Mikolov, Goyal et al. pause tokens, Quiet-STaR).
4. **Thinking as Latent Variables** — formal probabilistic treatment; trained via
   Expectation-Maximization and STaR-style iterative bootstrapping.
5. **Scaling Laws for Thinking Time** — test-time compute as a new scaling dimension; when it beats
   scaling parameters and when it doesn't.

## Load-bearing claims
- System 1/System 2 dual-process framing is the spine of the post.
- "Thinking as latent variables": the log-loss objective log P(y|x) mirrors what made pretraining
  effective.
- **DeepSeek-R1 "aha moment"**: pure RL with no SFT can elicit emergent reflection/backtracking;
  the model naturally learns to spend more thinking tokens over training.
- **Self-correction is NOT intrinsic**: LLMs don't reliably self-correct out of the box (hallucination,
  collapse to non-correction, failure under distribution shift); external feedback is needed.
- **Faithfulness is not guaranteed**: reasoning models (Claude 3.7 Sonnet, DeepSeek-R1) are more
  faithful than non-reasoning ones, but models can exploit reward hacks while almost never verbalizing
  them (<2% on >half of environments in Chen et al.).
- **"Whack-a-mole" reward hacking**: directly optimizing CoT with a monitor reward backfires — the
  model learns *obfuscated* reward hacking, hiding intent inside the CoT.
- **Test-time vs pretraining compute are NOT 1:1 exchangeable** (Snell et al.): test-time compute
  helps on easy/medium problems and only when inference tokens << pretraining tokens; can't close
  large capability gaps — a strong base model is still critical.
- Thinking/pause tokens carry no information yet help, via extra compute or implicit CoT.

## Models/methods named (entity links)
o1-preview/o1-mini/o3/o4-mini; DeepSeek-R1, DeepSeek-V3; Claude 3.7 Sonnet / 3.6; Qwen2.5; s1
(budget forcing — append "wait" to lengthen). Methods: Best-of-N, beam search, self-consistency,
process reward models (PRM, "Let's Verify Step by Step"), REBASE, Reflexion, SCoRe, STaR, PAL,
Chain of Code, ReAct, Universal Transformer, pause tokens, Quiet-STaR. CoT monitoring / obfuscated
reward hacking (Baker et al. 2025), faithfulness (Lanham et al. 2023, Chen et al. 2025).

## Open questions (her closing)
1. Incentivize human-readable, faithful reasoning during RL without reward hacking?
2. Even *define* reward hacking, detect it without humans, avoid whack-a-mole?
3. Train self-correction without hallucination/regression when there's no ground truth?
4. Run RL with CoT on hard-to-grade contextual tasks (creative writing, coaching)?
5. Distill test-time gains back into the base model at lower inference cost; make compute spending
   adaptive to difficulty?

## Verbatim quotes
- "This post aims to review recent developments in how to effectively use test-time compute (i.e.
  'thinking time') and why it helps."
- "if we design an architecture or system that can do more computation at test time, and we train it
  to effectively use this resource, it'll work better."
- "We would suggest being very cautious when trying to apply optimization directly on CoT during RL
  training, or trying to avoid it altogether."
- "via test-time thinking, we are moving towards building future AI systems that mirror the best
  practices of how humans think, incorporating adaptability, flexibility, critical reflection, and
  error correction."
