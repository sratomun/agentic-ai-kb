# RAW — Should we control AI instead of aligning it? (Spoiler: no) (Jan Leike, aligned.substack.com)
Source: https://aligned.substack.com/p/should-we-control-ai · 2025-01-24 · captured 2026-06-22 · channel: blog

## What AI control is
The basic pitch for **AI control**: build systems around capable models that ensure they can't cause harm even if misaligned (e.g. a misaligned model deliberately introducing subtle bugs, or trying to self-exfiltrate). Control techniques aim to catch and mitigate this.

Two reasons to do it:
1. So we can use/deploy models that aren't sufficiently aligned.
2. As an additional safeguard in case models aren't as aligned as we think.

- Reason 1 is especially interesting for an **automated alignment researcher**: we might want to leverage capable models for alignment research ASAP, while our alignment methods are still insufficient to trust them — bootstrap a solution if a controlled system can research better control techniques, then make more-trusted systems.
- Reason 2 adds a safety layer and is useful for compliance with frontier safety frameworks.

## How control works
- Most basic approach: use a more-trusted but less-capable model to monitor the untrusted policy — a finetuned "sus" classifier giving a 0–1 score; too high → throw away the sample and/or sound the alarm.
- Not fundamentally new: LLM companies already deploy monitoring classifiers on API traffic, but usually for cost (not trust) reasons and aimed at harmful USER use, not suspicious MODEL behavior.
- Other techniques: only use the untrusted model where output is reliably evaluable (e.g. with an outcome reward); use trusted models to rewrite/recreate outputs; best-of-n sampling against the sus monitor.

## How safe is it?
- Safety margin depends on how hard it is for the policy to subvert the control technique. The control agenda proposes **red teaming** to estimate the difficulty (e.g. finetune a policy to subvert control).
- Doesn't that require solving elicitation? Not necessarily — the red team doesn't need to succeed at eliciting subversion, just to estimate the capability. Might be easier than broad alignment because (1) you might only need good capability predictions, and (2) you can build capture-the-flag evals / honey pots with outcome rewards to measure successful circumvention. "In this sense subverting control might be much easier to evaluate than the task we ultimately want to use the model for."
- BUT hard to gain confidence without understanding elicitation: "It's just pretty unclear how to know that we red teamed the control technique enough." Did we cover all subversion strategies? Did we elicit the policy well, especially on fuzzy tasks like research sabotage?

## Why not just rely on control
- Reason 2 (extra safeguard) is compelling — deploying sus monitors is cheap with basically no downside.
- But without a good handle on elicitation, "we cannot be confident that our control techniques are effective… it's hard to know how much" — so reason 1 is hard to make work.
- More generally: "we should actually solve alignment instead of just trying to control misaligned AI." Control seems tractable today, but "we aren't really facing much misalignment risk yet, so it doesn't add much value at this point," and it's unclear how control scales to superhuman models. Solving alignment is "a much more holistic and sustainable solution."
- Closing line: "Don't try to imprison a monster, build something that you can actually trust!"
- Thanks: Buck Shlegeris, Ethan Perez, Fabian Roger, Ansh Radhakrishnan, Jared Kaplan, Tamera Lanham, and others.
