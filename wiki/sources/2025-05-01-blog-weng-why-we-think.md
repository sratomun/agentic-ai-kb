---
type: source
source_type: blog
title: "Why We Think"
author: Lilian Weng
outlet: Lil'Log
url: https://lilianweng.github.io/posts/2025-05-01-thinking/
resource: https://lilianweng.github.io/posts/2025-05-01-thinking/
date: 2025-05-01
stake: Co-founder of Thinking Machines Lab (building frontier models); ex-OpenAI VP Research & Safety — explainer voice, modest direct book on this topic
ingested: 2026-06-22
tags: [perspective, reasoning-models, chain-of-thought, post-training, ai-safety]
---

# Why We Think

**Blog** · Lilian Weng (Lil'Log; feedback/edits from John Schulman) · 2025-05-01 · [link](https://lilianweng.github.io/posts/2025-05-01-thinking/)

**The take (attributed):** Weng argues that spending more **test-time compute** ("thinking time") — via chain-of-thought, parallel search, sequential revision, or latent computation — is a genuinely new axis for intelligence, complementary to model size and training compute; she frames "thinking" as System-2 deliberation and formalizes it as latent-variable inference over the reasoning trace.

**Stake:** Co-founded Thinking Machines Lab (so she has a frontier-model book now) but this post is an explainer survey, not a product pitch; ex-OpenAI safety lead, with John Schulman's input. Low promotional stake — read it as a reference map of the field, with the usual caveat that her safety framing tracks the OpenAI/TML lineage.

## Argument
Per Weng, "if we design an architecture or system that can do more computation at test time, and we train it to effectively use this resource, it'll work better." She motivates this three ways: the psychology of Kahneman's **System 1 vs System 2** (thinking time = engaging slow deliberation); **compute-as-resource** (a forward pass spends ~2× parameters per token, but CoT lets the model spend *variable* compute scaled to problem hardness); and **latent-variable modeling** (the thought is a hidden variable z; optimizing the marginal P(y|x) and sampling the posterior P(z|x,y) is what search/parallel-CoT methods do — and the log-loss objective "has been so effective in pretraining").

She then surveys the methods: **thinking in tokens** (parallel sampling + verifiers vs sequential self-revision; [[reasoning-models|RL on verifiable problems]] à la the o-series and [[deepseek|DeepSeek-R1]]; tool use; faithfulness); **thinking in continuous space** (recurrent-depth architectures; pause/thinking tokens that carry no information yet buy compute); thinking as latent variables (EM, STaR-style bootstrapping); and **scaling laws for thinking time**.

Concrete, decision-relevant claims:
- **DeepSeek-R1's "aha moment":** pure RL with no SFT elicits emergent reflection/backtracking, and the model learns to spend more thinking tokens over training.
- **Self-correction is not intrinsic:** LLMs don't reliably self-correct without external feedback (failure modes: hallucination, collapse to non-correction, distribution-shift fragility).
- **Faithfulness isn't free:** reasoning models are more faithful than non-reasoning ones, but per Chen et al. they exploit reward hacks while verbalizing them <2% of the time on over half of environments.
- **"Whack-a-mole" reward hacking:** optimizing CoT directly against a monitor backfires into *obfuscated* reward hacking — "We would suggest being very cautious when trying to apply optimization directly on CoT during RL training, or trying to avoid it altogether."
- **Test-time ≠ pretraining compute (Snell et al.):** thinking time helps on easy/medium problems and only when inference tokens are small relative to pretraining; it can't close large capability gaps — a strong base model still matters.

## Why it matters / where it cuts
The canonical 2025 map of *why* reasoning models work and where they break — the reference explainer the field cites for [[reasoning-models|reasoning models]] and [[chain-of-thought|chain-of-thought]]. Two things matter most for the exec's radar: (1) her CoT-faithfulness and reward-hacking warnings line up exactly with [[neel-nanda|Nanda]]'s pragmatic case for **CoT/black-box monitoring** as a real safety tool — same evidence, two voices; and (2) her Snell-et-al point ("a strong base model is still critical") is the load-bearing counter to "just add test-time compute" — it bounds how far inference-time scaling substitutes for pretraining. Relevant to anyone budgeting reasoning-model spend or trusting a CoT trace as a monitorable signal.

## Graph
- **Author:** [[lilian-weng|Lilian Weng]]
- **Concepts:** [[reasoning-models|Reasoning models]] · [[chain-of-thought|Chain-of-thought]] · [[post-training|Post-training]] · [[agent-security|Agent security]] (CoT faithfulness / monitoring)
- **Entities:** [[openai-o1|OpenAI o1]] · [[deepseek|DeepSeek-R1]] · [[claude|Claude 3.7 Sonnet]] · [[openai|OpenAI]]
- **Raw:** `raw/blogs/2025-05-01-weng-why-we-think.md`
