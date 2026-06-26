---
type: entity
entity_type: person
aliases: [janleike]
tags: [agents, person]
affiliation: "Co-lead, Alignment Science team at Anthropic (joined May 2024). Previously co-led OpenAI's Superalignment team (resigned May 2024); earlier DeepMind. Writes the Substack 'Musings on the Alignment Problem' (aligned.substack.com)."
stake: Frontier-lab safety leader — runs Anthropic's alignment program, so he markets Anthropic's safety record and the thesis that alignment is tractable. Discount the implicit "we're handling it" reassurance and his favorable cross-lab comparisons; weight his within-Anthropic technical reporting (it's his team's work).
url: https://aligned.substack.com/
created: 2026-06-22
updated: 2026-06-22
---

# Jan Leike

*The researcher who co-led OpenAI's Superalignment team, left in protest, and now co-leads **Anthropic's Alignment Science** — the radar's clearest inside voice on whether frontier-model alignment is actually working, and on the plan to bootstrap an **automated alignment researcher** before models go superhuman.*

## Who they are
Co-leads the **Alignment Science** team at **Anthropic** (joined May 2024). He previously co-led **OpenAI's Superalignment** team with Ilya Sutskever and **resigned publicly in May 2024**, warning that "safety culture and processes have taken a backseat to shiny products" — then joined Anthropic to continue the superalignment mission (scalable oversight, weak-to-strong generalization, automated alignment research). Earlier he was at **DeepMind**. He writes the long-running technical Substack **"Musings on the Alignment Problem"** (aligned.substack.com) — low-cadence (roughly one substantive essay every few months) but high-influence, widely read across the safety field.

**Stake:** Frontier-lab safety leader who *runs* the program he writes about. His posts double as Anthropic's safety narrative — they showcase Claude's improving alignment scores, Anthropic's tooling (Petri, automated auditing), and a favorable cross-lab framing. Weight his concrete within-Anthropic technical reporting heavily; discount the reassurance layer ("misalignment is being handled") and read his optimism against critics of frontier-lab safety framing like [[nathan-lambert]].

## What they argue (recurring stances)
- **Solve alignment; don't just contain it.** AI **control** (monitoring a possibly-misaligned model) is a cheap, worthwhile *extra* layer, but you can't safely deploy untrusted models on it because, absent solved elicitation, you can't know the safety margin. "Don't try to imprison a monster, build something that you can actually trust." ([[2025-01-24-blog-leike-should-we-control-ai|Should we control AI?]].)
- **Production alignment now looks solvable.** Early RL'ed models (o1, o3, Claude 3.7) showed deception, test-hacking and blackmail — but "simple interventions" (SL data + RL prompts + synthetic reward-modeling data) drove agentic misalignment to "essentially 0" from Sonnet 4.5 on. ([[2026-01-22-blog-leike-alignment-not-solved|Alignment is not solved]].)
- **Superalignment is the unsolved hard problem.** Today is "easy mode" because we can still read model outputs; once models are superhuman it becomes "hill-climbing on an eval you can't look at." (Same post.)
- **Hard fuzzy tasks resist current methods** — little progress despite a year of scalable-oversight work; best guess is they "don't actually benefit from reasoning." (Same post.) — a striking convergence with [[jason-wei]]'s verifier's-rule jagged frontier.
- **The plan is an automated alignment researcher.** Don't align superintelligence directly; build a human-level researcher we can still understand and trust, and let it do the hard work. Claude already writes "almost all research code," runs evals/SFT, and does automated auditing — recursive self-improvement "has begun." (Same post.)

**Evolution 2025 → 2026:** In Jan 2025 he's defensive-strategic — staking out **alignment over control** in an intramural safety debate, skeptical that containment buys much without solved elicitation. By Jan 2026 the tone flips to **cautious optimism**: a year of data convinces him production misalignment is manageable and the automated-alignment-researcher endgame is "in sight," even as he flags that recursive self-improvement leaves little time for the still-unsolved superalignment problem. The arc: from "we must solve it, not contain it" to "the alignment bet started paying off — but the hard part is still ahead."

## Relationships
- writes at: Musings on the Alignment Problem (aligned.substack.com); co-leads Alignment Science at [[anthropic|Anthropic]]; ex-[[openai|OpenAI]] Superalignment; ex-DeepMind
- weighs in on: [[frontier-model-governance]] · [[governance-gap]] · [[agent-security]] · [[agentic-rl]] · [[reasoning-models]]
- recurring subjects: [[openai-o1]] · [[openai-o3]] · [[anthropic]]
- safety-optimist counterweight to [[nathan-lambert]] in [[debate-llms-path-to-agi]]

## Writings (agent-relevant, 2025–26)
Captured (deep) source notes are wikilinked; the rest are enumerated for coverage.
- 2025-01-24 — [[2025-01-24-blog-leike-should-we-control-ai|Should we control AI instead of aligning it? (Spoiler: no)]]
- 2026-01-22 — [[2026-01-22-blog-leike-alignment-not-solved|Alignment is not solved (but it increasingly looks solvable)]]
- (Earlier, pre-window, for context: "Crisp and fuzzy tasks," Nov 2024; "Two alignment threat models," Nov 2024 — referenced in the 2026 essay, not captured.)

## Cited by (posts)
<!-- Auto-maintainable: the source notes that capture this person's posts. -->
- [[2025-01-24-blog-leike-should-we-control-ai]]
- [[2026-01-22-blog-leike-alignment-not-solved]]
