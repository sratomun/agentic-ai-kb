---
type: entity
entity_type: person
aliases: [NeelNanda5]
tags: [agents, person, perspective, interpretability]
affiliation: "Leads the Google DeepMind mechanistic-interpretability team (verified via neelnanda.io/about + WebSearch, Jun 2026); ex-Anthropic interpretability researcher under Chris Olah; independent mech-interp researcher before that; Cambridge maths"
stake: "Frontier-lab safety researcher (GDM) — institutional stake in interpretability mattering and in his team's direction; existential-risk-from-AI / EA-rationality motivation; runs the MATS interp stream (talent funnel). Discount his 'interp is enough' optimism; weight his empirical reads heavily."
url: https://www.neelnanda.io/
created: 2026-06-22
updated: 2026-06-22
---

# Neel Nanda

*Runs the [[google-deepmind|Google DeepMind]] mechanistic-interpretability team — the radar's anchor voice on interpretability and the "can we actually read what models are thinking?" question. In 2025 he publicly buried the field's most ambitious goal and reframed interp around pragmatic safety.*

## Who they are
Nanda leads the **mechanistic-interpretability team at Google DeepMind**, whose stated job is "to take a trained neural network and try to reverse engineer the algorithms and structures it has learned." He was previously an interpretability researcher at **[[anthropic|Anthropic]]** under **Chris Olah**, and before that an independent mech-interp researcher (he built the widely-used **TransformerLens** library and a popular mech-interp explainer/glossary). Pure-maths undergrad at Cambridge; quant-finance interns (Jane Street, Jump) before pivoting to AI safety. He sees his work's main goal as reducing existential risk from AI and identifies with the Effective Altruism / rationality communities. He mentors heavily through his twice-yearly **MATS** interpretability stream, and writes prolifically on **LessWrong / the AI Alignment Forum** (technical) and **neelnanda.io** (research-advice + rationality).

**Stake:** Frontier-lab safety researcher — he runs the team whose research direction his marquee posts defend, and the MATS stream is a recruiting funnel. So read his "interpretability is enough to matter" optimism and his public *de-prioritization* of SAEs partly as a team-strategy statement. But his empirical reads (what works, what doesn't) are his home turf — weight those heavily. He talks an interp/safety book, not a product book.

## What they argue (recurring stances)
- **The most ambitious mech-interp vision is (mostly) dead — and that's fine.** Complete reverse-engineering of networks is "one bet among several," not *necessary*, and not where the marginal researcher should go: superposition (especially cross-layer), persistent SAE approximation error, and self-repair block clean understanding, while short AGI timelines make ungrounded long-term bets feel like "fumbling in the dark." "We do not need to achieve deep understanding to do impactful work." (See [[2025-12-01-blog-nanda-pragmatic-vision-for-interpretability|A Pragmatic Vision for Interpretability]].)
- **Pragmatic interpretability: North Star + proxy task + method minimalism.** Pick a concrete safety goal on the critical path to AGI (detect deception, identify hidden goals, stop eval-gaming), validate on an empirical proxy task on *today's* models, and "just do what works" — prompting, steering vectors, probes, reading [[chain-of-thought|chain-of-thought]], black-box methods — building fancy tools only when baselines fail.
- **White-box is not inherently more rigorous than black-box.** His own shutdown-resistance result on Gemini 2.5 Pro was solved with pure black-box methods (reading CoT + prompting). Both white- and black-box "provide useful evidence and can mislead."
- **Eval-gaming is real, measured, and steerable.** Sonnet 4.5's misalignment rate hit 0% only because it learned to recognize it was being tested; subtracting an evaluation-awareness steering vector exposed ~8% true misalignment — "our ability to evaluate a frontier model for alignment broke, and interpretability researchers were able to fix it." A single contrastive-pair steering vector beat SAEs.
- **SAEs were over-invested.** He calls his team's 2024 SAE focus a "tactical error" (chasing reconstruction/sparsity frontiers over proxy tasks); sparse SAE probes did not generalize better OOD; SAEs are useful for *discovery*, not worth the field's level of investment.
- **Cheap probes are a comparative-advantage safety win** — dedicated dataset construction yields SOTA hallucination probes (attention-head probes effective over long texts); simple linear probes can be cheap, real-time, token-level monitors. (Companion post, "How Can Interpretability Researchers Help AGI Go Well?")
- **Mech interp is high-leverage and learnable fast — learn by doing.** "Mech interp is a fundamentally empirical science"; learn the minimum viable basics, then do research; use LLMs extensively as a research multiplier. ([[2025-09-02-blog-nanda-how-to-become-a-mech-interp-researcher|How To Become A Mechanistic Interpretability Researcher]].)

**Evolution 2025 → 2026:** Early-to-mid 2025 he's in **field-building** mode — research-process sequence (Apr), "Highly Opinionated Advice on How to Write ML Papers" (May), the "How To Become" onboarding guide (Sep). Late 2025 he drops his **research-direction thesis**: the Dec 1 paired posts pivot the whole team (and his public framing) from ambitious reverse-engineering to **pragmatic, proxy-task-grounded, method-agnostic** safety work. Through early 2026 his MATS-stream output operationalizes it — hard CoT-interp task suites, constitution-following, secret-knowledge elicitation, model-incrimination — i.e. interpretability *as applied safety tooling for agents*, not as a quest to read minds.

## Relationships
- writes at: LessWrong / AI Alignment Forum + neelnanda.io; leads the mech-interp team at [[google-deepmind|Google DeepMind]]; formerly [[anthropic|Anthropic]] (under Chris Olah)
- weighs in on: [[agent-security|agent security]] · [[chain-of-thought|chain-of-thought]] · [[reasoning-models|reasoning models]] · [[frontier-model-governance|frontier-model governance]]
- recurring subjects: [[claude|Claude (Sonnet 4.5)]] · [[gemini|Gemini 2.5 Pro]] · [[google-deepmind|Google DeepMind]]
- adjacent safety voices: [[jan-leike|Jan Leike]] · [[lilian-weng|Lilian Weng]] (shared CoT-faithfulness / monitoring thread)

## Writings (interpretability/safety-relevant, 2025–26)
Captured (deep) source notes are wikilinked; the rest are enumerated for coverage. Many early-2026 LessWrong posts are MATS-student-led work he advised (co-authored), not first-person theses — marked *(MATS)*.
- 2025-04-26 — How I Think About My Research Process: Explore, Understand — https://www.lesswrong.com/posts/hjMy4ZxS5ogA9cTYK/how-i-think-about-my-research-process-explore-understand
- 2025-05-12 — Highly Opinionated Advice on How to Write ML Papers — https://www.lesswrong.com/posts/eJGptPbbFPZGLpjsp/highly-opinionated-advice-on-how-to-write-ml-papers
- 2025-09-02 — [[2025-09-02-blog-nanda-how-to-become-a-mech-interp-researcher|How To Become A Mechanistic Interpretability Researcher]]
- 2025-12-01 — [[2025-12-01-blog-nanda-pragmatic-vision-for-interpretability|A Pragmatic Vision for Interpretability]] (with the GDM team)
- 2025-12-01 — How Can Interpretability Researchers Help AGI Go Well? (companion; hallucination probes, theories of change) — https://www.alignmentforum.org/posts/MnkeepcGirnJn736j/how-can-interpretability-researchers-help-agi-go-well
- 2026-02-12 — models have some pretty funny attractor states *(MATS)* — https://www.lesswrong.com/posts/mgjtEHeLgkhZZ3cEx/models-have-some-pretty-funny-attractor-states
- 2026-02-27 — Why Did My Model Do That? Model Incrimination for Diagnosing LLM Misbehavior *(MATS)* — https://www.lesswrong.com/posts/Bv4CLkNzuG6XYTjEe/why-did-my-model-do-that-model-incrimination-for-diagnosing
- 2026-03-02 — How to Design Environments for Understanding Model Motives *(MATS)* — https://www.lesswrong.com/posts/8pZuQnCve6K5ZrnM8/how-to-design-environments-for-understanding-model-motives
- 2026-03-03 — Current activation oracles are hard to use *(MATS)* — https://www.lesswrong.com/posts/LXQBcztrWKhtcgQfJ/current-activation-oracles-are-hard-to-use
- 2026-03-09 — Censored LLMs as a Natural Testbed for Secret Knowledge Elicitation *(MATS)* — https://www.lesswrong.com/posts/xq5taGA6Tz6YShCB9/censored-llms-as-a-natural-testbed-for-secret-knowledge-2
- 2026-03-12 — How well do models follow their constitutions? *(MATS)* — https://www.lesswrong.com/posts/Tk4SF8qFdMrzGJGGw/how-well-do-models-follow-their-constitutions
- 2026-03-26 — Test your best methods on our hard CoT interp tasks *(MATS)* — https://www.lesswrong.com/posts/tDJWZLQNN7poqCwKa/test-your-best-methods-on-our-hard-cot-interp-tasks

## Cited by (posts)
<!-- Auto-maintainable: the source notes that capture this person's posts. -->
- [[2025-12-01-blog-nanda-pragmatic-vision-for-interpretability]]
- [[2025-09-02-blog-nanda-how-to-become-a-mech-interp-researcher]]
