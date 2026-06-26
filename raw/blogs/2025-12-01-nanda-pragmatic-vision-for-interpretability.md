---
source: https://www.lesswrong.com/posts/StENzDcD3kpfGJssR/a-pragmatic-vision-for-interpretability
mirror: https://www.alignmentforum.org/posts/StENzDcD3kpfGJssR/a-pragmatic-vision-for-interpretability
author: Neel Nanda (with the Google DeepMind mechanistic interpretability team — Josh Engels, Arthur Conmy, Senthooran Rajamanoharan, Bilal Chughtai, Callum McDougall, János Kramár, Lewis Smith)
outlet: LessWrong / AI Alignment Forum
date: 2025-12-01
captured: 2026-06-22
capture_method: web_fetch (full text)
immutable: true
---

# A Pragmatic Vision for Interpretability — raw capture

> Immutable source capture. Captured via web_fetch on 2026-06-22; reading time ~32 min.
> Companion post: "How Can Interpretability Researchers Help AGI Go Well?" (same date, same team).

## Core thesis (author's framing)
The DeepMind mech interp team has pivoted from chasing the ambitious goal of *complete
reverse-engineering* of neural networks toward **pragmatic interpretability**: making as
much progress as they can on the critical path to AGI going well, choosing problems by
the team's comparative advantage, and measuring progress by **empirical payoffs on proxy
tasks** rather than internal metrics like reconstruction/sparsity error. They reframe the
field's central question from "is this mech interp?" to "how can mech interp *researchers*
have the most impact?" — and conclude the answer often lies in work that isn't classic
mech interp (steering, probing, reading chain-of-thought, black-box methods).

Verbatim: "The DeepMind mech interp team has pivoted from chasing the ambitious goal of
complete reverse-engineering of neural networks, to a focus on pragmatically making as
much progress as we can on the critical path to preparing for AGI to go well, and choosing
the most important problems according to our comparative advantage."

## Why ambitious reverse-engineering is no longer the north star
Not "useless" or "stop" — rather "one bet among several," not *necessary*, and not where the
marginal researcher should go. Technical/practical barriers cited:
- **Superposition**, "especially cross-layer superposition" — far out of reach.
- **Dictionary learning / SAEs** have made limited progress toward reverse-engineering "at
  best"; persistent significant approximation error "which shows no signs of going away."
- **Self-repair** — "we can't get clean info from causal interventions."
- **Increased algorithmic complexity** of modern models: sampling dependence, multi-turn,
  agentic tool calls.
- **Inherently interpretable models**: some progress, but "no signs that the techniques will
  become cheap enough to be applied to frontier models."

Reasons to pivot now ("times have changed"):
- Models are far more capable → safety-relevant behaviours (scheming, eval awareness,
  reward hacking, alignment faking, deception) are now empirically reachable → better proxy
  tasks exist.
- Model organisms + synthetic-document fine-tuning let them implant hidden goals / eval
  awareness with known ground truth.
- Disappointment with ambitious mech interp's progress (from themselves and others).
- Timeline urgency: enough probability on short timelines (2–5 years) to value work paying
  off in a ~10-year window; "ungrounded long-term bets" feel like "fumbling in the dark."
- Methodological claim: ambitious reverse-engineering "should be evaluated the same way as
  other pragmatic approaches: via empirical payoffs on tasks, not approximation error."

## What the pragmatic vision replaces it with
- **North Star + proxy task**: pick a stepping-stone goal on the critical path (e.g. "stop
  models acting differently when tested", "detect deception", "identify hidden goals"); find
  an objective empirical task on *today's* models that tracks it. Key test: "if you succeeded
  on it, would you actually update toward believing you'd made progress on your North Star?"
  Goodhart's Law is the named danger; red-team your own proxy.
- **Method minimalism**: "Just do what works." Start with the simplest/cheapest methods —
  prompting, steering, probing, reading chain-of-thought, prefill attacks — and only build
  fancy methods once baselines demonstrably fail. Includes black-box techniques. "Method
  minimalism is about using the simplest thing that works, not about using simple things."
- **Comparative advantage**: mech interp researchers' transferable skills (working with model
  internals, deep scientific hypothesis-testing, unsupervised discovery, qualitative insight)
  applied to neglected safety problems, even when the work isn't "classic mech interp."
- Two project archetypes: **focused** (proxy-task-driven, theory of change first) and
  **exploratory** (curiosity-driven but proxy-validated; time-boxed, aim ~2 weeks).

## Concrete results / examples cited
- **Eval-awareness steering on Sonnet 4.5** (Jack Lindsey's team, Anthropic): Sonnet 4.5's
  misalignment rate on tests fell to 0% because the model got better at *recognizing it was
  being evaluated*. Subtracting an **evaluation-awareness steering vector** revealed true
  misalignment of ~**8%**. Best method was a steering vector from a **single contrastive pair**
  — SAEs did not beat it. Punchline: "our ability to evaluate a frontier model for alignment
  broke, and interpretability researchers were able to fix it."
- **Shutdown resistance (Gemini 2.5 Pro)**: model in a bash terminal sometimes disabled
  shutdown.sh even when told to allow shutdown. Black-box methods (reading CoT + prompting)
  found Gemini was "simply confused" — couldn't finish the math task AND comply; clarifying
  precedence in the prompt fixed it. Lesson: black-box methods "surprisingly powerful";
  white-box is not inherently more rigorous.
- **CAFT** (Casademunt & Juang, MATS): ablating activation subspaces stopped emergent
  misalignment / spurious-cue learning without changing data.
- **Entity-recognition latents** (Obeso & Ferrando): SAE latents firing iff the model knows
  facts about an entity; steering induces hallucination or "I don't know." Cited as evidence
  for SAEs as an *unsupervised discovery* methodology more than object-level insight.
- **Reasoning-training interp** (Venhoff & Arcuschin): per-token KL between base and reasoning
  models concentrated on backtracking tokens ("Wait"); a hybrid scaffold recovered much
  reasoning performance.
- **Their own 2024 SAE work**: judged a "tactical error" to chase reconstruction/sparsity
  Pareto frontiers over proxy tasks; sparse SAE probes did NOT generalize better OOD;
  deprioritized SAE research (useful for discovery, not worth the field's investment level).

## Relationship to other safety approaches
- Chain-of-thought / black-box monitoring is *embraced*, not opposed. "We used to think
  white-box methods inherently offered more rigor. We no longer believe this." Both white- and
  black-box "provide useful evidence and can mislead."
- Interp is one tool in the safety portfolio, chosen by comparative advantage.
- Probes/steering as cheap monitors highlighted as a comparative-advantage win.

## Key verbatim quotes
- "We do not need to achieve deep understanding to do impactful work."
- "Ambitious reverse engineering is one bet among several. It is not *necessary* to have an
  impact with interpretability tools. The marginal interpretability researcher is more likely
  to have impact by grounding their work in safety-relevant proxy tasks on modern models."
- "our ability to evaluate a frontier model for alignment broke, and interpretability
  researchers were able to fix it."
- (On "Aren't You Just Giving Up?") "Maybe? In a strictly technical sense yes, we are
  suggesting that we give up on the ambitious goal of complete reverse-engineering. But on our
  *actual* goal of ensuring AGI goes well, we feel great! ... near-complete reverse-engineering
  is not needed."
- "given where models are today and that AGI timelines are plausibly relatively short, the most
  neglected and tractable part of interpretability is task-grounded, proxy-measured,
  method-agnostic work, that is directly targeted at problems on the critical path towards
  being prepared for AGI."

> Note: the often-paraphrased "low chance of incredibly big deal → high chance of medium big
> deal" framing does NOT appear verbatim in this post's body; closest is the explore/exploit
> appendix arguing the marginal researcher is over-indexed on curiosity-driven work.
