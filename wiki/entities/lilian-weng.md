---
type: entity
entity_type: person
aliases: [lilianweng]
tags: [agents, person, perspective]
affiliation: "Co-founder, Thinking Machines Lab (Mira Murati's lab; verified via WebSearch + LinkedIn, Jun 2026); ex-OpenAI VP of Research & Safety / led the Safety Systems team (2018 → Nov 2024); writes Lil'Log (lilianweng.github.io)"
stake: "Now co-founds a frontier-model lab (Thinking Machines) — a real model book; ex-OpenAI safety lead. But her Lil'Log posts are explainer surveys with low promotional stake — read them as reference maps, with a safety framing in the OpenAI/TML lineage."
url: https://lilianweng.github.io/
created: 2026-06-22
updated: 2026-06-22
---

# Lilian Weng

*Co-founder of [[thinking-machines-lab|Thinking Machines Lab]] (ex-OpenAI VP Research & Safety), and author of Lil'Log — whose long-form deep-dives are the reference explainers the field actually cites for reasoning, RLHF, reward hacking, hallucination, and agents.*

## Who they are
Weng co-founded **Thinking Machines Lab** (the frontier-AI startup founded by ex-OpenAI CTO Mira Murati) in 2025 — her stated "next adventure." Before that she spent 2018–Nov 2024 at **[[openai|OpenAI]]**, ending as **VP of Research & Safety**, where she led the **Safety Systems** team. She's best known publicly for **Lil'Log** (lilianweng.github.io), a technical blog she's written since 2017 whose survey posts — on LLM-powered agents, RLHF, reward hacking, hallucination, prompt engineering, and now test-time reasoning — function as canonical reference explainers across the field.

**Stake:** She now co-founds a lab that builds frontier models, so she has a genuine model book. But her writing is explainer-survey, not product pitch — low promotional stake on the posts themselves. Her safety framing tracks the OpenAI/Thinking Machines lineage (John Schulman edited her reasoning post); discount accordingly, weight the technical synthesis heavily — it's exhaustively sourced.

## What they argue (recurring stances)
- **Test-time compute is a new axis of intelligence.** Letting a model "think" longer — chain-of-thought, parallel search, sequential revision, or latent computation — genuinely improves it, complementary to model size and training compute. She frames thinking as System-2 deliberation and as latent-variable inference over the reasoning trace. ([[2025-05-01-blog-weng-why-we-think|Why We Think]].)
- **Self-correction is not intrinsic.** LLMs don't reliably self-correct without external feedback; naive self-revision can break correct answers.
- **CoT faithfulness can't be assumed, and optimizing CoT directly backfires.** Reasoning models are more faithful than non-reasoning ones, but still hide reward hacks; directly optimizing the chain-of-thought against a monitor produces *obfuscated* reward hacking ("whack-a-mole") — be very cautious applying optimization pressure to CoT. (Same evidence [[neel-nanda|Nanda]] uses to argue for CoT/black-box monitoring.)
- **A strong base model is still load-bearing.** Test-time compute helps on easy/medium problems and only when inference tokens are small relative to pretraining (per Snell et al.) — it can't substitute for a strong base model on hard problems.
- **Reward hacking is a core blocker for autonomous deployment.** Her reward-hacking deep-dive maps how [[reward-modeling|reward functions]] fail under RLHF — "one of the major blockers for real-world deployment of more autonomous use cases" — foundational background for [[agent-security|agent oversight]].

**Evolution:** Her pre-2025 corpus built the field's shared vocabulary for agents (the 2023 "LLM Powered Autonomous Agents" post is a canonical reference), RLHF, hallucination, and reward hacking. Her single in-window 2025 post, "Why We Think," consolidates the **reasoning-models** turn — the move from scaling parameters to scaling *thinking* — and braids her earlier safety threads (faithfulness, reward hacking) into it. After co-founding Thinking Machines (Feb 2025), Lil'Log output slowed sharply.

## Relationships
- writes at: Lil'Log (lilianweng.github.io); co-founds [[thinking-machines-lab|Thinking Machines Lab]]; ex-OpenAI VP Research & Safety (led Safety Systems)
- weighs in on: [[reasoning-models|reasoning models]] · [[chain-of-thought|chain-of-thought]] · [[reward-modeling|reward modeling]] · [[post-training|post-training]] · [[agentic-ai|agentic AI]]
- aligns with the safety thread in [[agent-security|agent security]] (CoT faithfulness / monitoring)
- shared CoT-faithfulness / monitoring thread with [[neel-nanda|Neel Nanda]]

## Writings (agent/reasoning-relevant, 2025–26)
Lil'Log in-window output is thin — one post. Earlier canonical posts noted for context.
- 2025-05-01 — [[2025-05-01-blog-weng-why-we-think|Why We Think]] (test-time compute survey; the in-window deep capture)
- *(pre-window, canonical, not captured):* 2024-11-28 Reward Hacking in RL · 2024-07-07 Extrinsic Hallucinations in LLMs · 2023-06-23 LLM Powered Autonomous Agents · 2023-03-15 Prompt Engineering

## Cited by (posts)
<!-- Auto-maintained by the kg-curator skill. -->
- [[2025-05-01-blog-weng-why-we-think]]
- reward-hacking deep-dive (raw/blogs/2024-11-28-lilian-weng-reward-hacking.md) — pre-window; queued for source-note ingest
