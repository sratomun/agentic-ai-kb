---
type: source
source_type: blog
title: "Should we control AI instead of aligning it? (Spoiler: no)"
author: Jan Leike
outlet: Musings on the Alignment Problem (aligned.substack.com)
url: https://aligned.substack.com/p/should-we-control-ai
resource: https://aligned.substack.com/p/should-we-control-ai
date: 2025-01-24
stake: Co-lead of Anthropic's Alignment Science team — argues for "solve alignment" over "contain misaligned AI"; markets the alignment-first program he runs
ingested: 2026-06-22
tags: [perspective, frontier-model-governance, agent-security]
---

# Should we control AI instead of aligning it? (Spoiler: no)

**Blog** · Jan Leike (Musings on the Alignment Problem) · 2025-01-24 · [link](https://aligned.substack.com/p/should-we-control-ai)

**The take (attributed):** Leike argues **AI control** (containing a possibly-misaligned model with monitors and guardrails) is a cheap, worthwhile *extra* safety layer — but you can't rely on it to safely deploy untrusted models, because without solving elicitation you can't know how much safety margin it actually buys. The real goal must be to **solve alignment**, not "imprison a monster."

**Stake:** Co-leads Anthropic Alignment Science. This stakes out a position in an intramural safety debate (control vs. alignment) — it argues for the alignment-first agenda his team owns, and against over-trusting the control agenda associated with researchers like Buck Shlegeris.

## Argument
- **Control** = build systems around capable models so they can't cause harm even if misaligned (catch subtle sabotage, self-exfiltration). Two motivations: (1) deploy/use not-yet-aligned models — attractive for bootstrapping an automated alignment researcher; (2) an extra safeguard.
- **Mechanics:** a more-trusted, less-capable model monitors the untrusted policy via a "sus" classifier (0–1); too high → discard the output / sound the alarm. Plus: only use the untrusted model where output is reliably checkable; have trusted models rewrite outputs; best-of-n against the monitor.
- **Safety depends on red-teaming** the policy's ability to subvert control. This needs only *estimating* (not eliciting) the capability — possibly easier than broad alignment, and measurable with capture-the-flag evals / honey pots. But "it's pretty unclear how to know that we red teamed the control technique enough," especially on fuzzy tasks like research sabotage.
- **Verdict:** deploying sus monitors is cheap with ~no downside (reason 2 is good). But without understanding elicitation you can't be confident control is effective, so reason 1 is hard to make work. "We should actually solve alignment instead of just trying to control misaligned AI… Don't try to imprison a monster, build something that you can actually trust!"

## Why it matters / where it cuts
The clearest statement of the **control-vs-alignment** split inside frontier safety research, from the alignment camp. Decision-relevant for the exec as a map of *how the safety field itself disagrees* on near-term strategy — and it sets up the optimism in [[2026-01-22-blog-leike-alignment-not-solved|his 2026 follow-up]], where Leike claims the alignment bet started paying off. Feeds [[agent-security]] and [[frontier-model-governance]].

## Graph
- **Author:** [[jan-leike]]
- **Concepts:** [[agent-security]] · [[frontier-model-governance]] · [[governance-gap]]
- **Entities:** [[anthropic]]
- **Raw:** `raw/blogs/2025-01-24-jan-leike-should-we-control-ai.md`
