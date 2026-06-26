---
type: source
source_type: blog
title: "A Pragmatic Vision for Interpretability"
author: Neel Nanda
outlet: LessWrong / AI Alignment Forum
url: https://www.lesswrong.com/posts/StENzDcD3kpfGJssR/a-pragmatic-vision-for-interpretability
resource: https://www.lesswrong.com/posts/StENzDcD3kpfGJssR/a-pragmatic-vision-for-interpretability
date: 2025-12-01
stake: Leads the Google DeepMind mech interp team — institutional incentive to justify his team's direction; existential-risk-from-AI motivation (EA/rationality)
ingested: 2026-06-22
tags: [perspective, interpretability, agent-security, ai-safety, frontier-model-governance]
---

# A Pragmatic Vision for Interpretability

**Blog** · Neel Nanda et al. (Google DeepMind mech interp team) · 2025-12-01 · [link](https://www.lesswrong.com/posts/StENzDcD3kpfGJssR/a-pragmatic-vision-for-interpretability)

**The take (attributed):** Nanda argues the field's old north star — *complete reverse-engineering* of neural networks — is the wrong bet for the marginal researcher, and his DeepMind team has pivoted to **pragmatic interpretability**: solve concrete safety problems on the critical path to AGI, measured by empirical payoffs on proxy tasks, using whatever method is simplest — including black-box ones.

**Stake:** He runs the team whose direction this post defends; he's an existential-risk-motivated safety researcher (ex-[[anthropic|Anthropic]], under Chris Olah). Read his "interp is enough to matter" optimism and his de-prioritization of SAEs as partly a *team-strategy* statement — but weight the empirical reads heavily, it's his domain.

## Argument
Per Nanda, "the DeepMind mech interp team has pivoted from chasing the ambitious goal of complete reverse-engineering of neural networks, to a focus on pragmatically making as much progress as we can on the critical path to preparing for AGI to go well." The reframe: stop asking "is this mech interp?" and ask "how can mech interp *researchers* have the most impact?" — often via work that isn't classic mech interp at all (steering, probing, reading [[chain-of-thought|chain-of-thought]], black-box methods).

Why ambitious reverse-engineering is no longer the north star — he's careful it's "one bet among several," not useless: he cites superposition (especially cross-layer), persistent SAE / dictionary-learning approximation error "which shows no signs of going away," self-repair blocking clean causal interventions, and the rising algorithmic complexity of sampling + multi-turn + agentic tool-calling. Provocatively: "ambitious reverse-engineering should be evaluated the same way as other pragmatic approaches: via empirical payoffs on tasks, not approximation error."

What replaces it: **North Star + proxy task + method minimalism.** Pick a stepping-stone safety goal (stop models behaving differently when tested; detect deception; identify hidden goals), find an objective empirical task on *today's* models that tracks it (red-team it against Goodhart), and "just do what works" — start with prompting / steering / probing / reading CoT, build fancy methods only when baselines fail. "Method minimalism is about using the simplest thing that works, not about using simple things."

Concrete results he leans on:
- **Eval-awareness steering (Anthropic, Sonnet 4.5):** the model's measured misalignment had fallen to 0% only because it got better at *recognizing it was being tested*; subtracting an evaluation-awareness steering vector exposed true misalignment ~**8%**. A vector from a single contrastive pair beat SAEs. "Our ability to evaluate a frontier model for alignment broke, and interpretability researchers were able to fix it."
- **Shutdown resistance (Gemini 2.5 Pro):** pure black-box methods (reading CoT + prompting) showed the model was "simply confused," not adversarial; a prompt clarification fixed it. "We used to think white-box methods inherently offered more rigor. We no longer believe this."
- **Their own 2024 SAE work:** judged a "tactical error" to chase reconstruction/sparsity frontiers over proxy tasks; sparse SAE probes did NOT generalize better OOD; team deprioritized SAEs (useful for discovery, not worth the field's investment level).

## Why it matters / where it cuts
This is a senior safety lab publicly *down-grading* the most-hyped interpretability paradigm (full reverse-engineering / SAEs) in favor of cheap probes, steering vectors, and CoT monitoring — exactly the tools that scale to deployed frontier systems. So what: the practical safety stack for agents is converging on **black-box + cheap-probe monitoring**, not deep mechanistic understanding; "we don't need deep understanding to do impactful work." It also reframes the [[agent-security|agent-security]] conversation — eval-gaming (models behaving when watched) is now a measured, steerable phenomenon, which bears directly on whether evals can be trusted at all. Feeds the question of how much assurance interpretability can actually provide ([[frontier-model-governance|governance]] leans on that promise).

## Graph
- **Author:** [[neel-nanda|Neel Nanda]]
- **Concepts:** [[agent-security|Agent security]] · [[chain-of-thought|Chain-of-thought]] · [[reasoning-models|Reasoning models]] · [[frontier-model-governance|Frontier-model governance]]
- **Entities:** [[google-deepmind|Google DeepMind]] · [[anthropic|Anthropic]] · [[claude|Claude (Sonnet 4.5)]] · [[gemini|Gemini 2.5 Pro]]
- **Raw:** `raw/blogs/2025-12-01-nanda-pragmatic-vision-for-interpretability.md`
