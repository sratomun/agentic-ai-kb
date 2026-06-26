---
type: source
source_type: blog
title: "Automating AI Research (Import AI 455)"
author: Jack Clark
outlet: Import AI
url: https://jack-clark.net/2026/05/04/import-ai-455-automating-ai-research/
resource: https://jack-clark.net/2026/05/04/import-ai-455-automating-ai-research/
date: 2026-05-04
stake: Anthropic co-founder & Head of Policy. The "intelligence explosion is coming, government must act" thesis directly supports Anthropic's policy positioning and its automated-alignment research agenda. Several of the cited datapoints are Anthropic's own (Opus speedups, automated alignment PoC). Discount the timeline rhetoric; the benchmark-trend evidence is checkable.
ingested: 2026-06-22
tags: [perspective, self-evolving-agents, coding-agents, frontier-model-training, agent-evaluation, governance-gap]
---

# Automating AI Research — "AI systems are about to start building themselves"

**Blog (Import A-Idea essay)** · Jack Clark (Import AI) · 2026-05-04 · [link](https://jack-clark.net/2026/05/04/import-ai-455-automating-ai-research/)
*(Whole-issue essay; no separate paper-roundup digest.)*

**The take (attributed):** Clark argues — "reluctantly," from public benchmark data — that there's a **60%+ chance of no-human-involved AI R&D (a model autonomously training its successor) by end of 2028** (~30% by end of 2027). He claims AI can already automate "vast swathes, perhaps the entirety, of AI *engineering*"; the open question is how much of AI *research* (the creative part) it can automate.

**Stake:** Anthropic co-founder/policy lead. This is the empirical companion to his "appropriate fear" essay — and it leans on Anthropic's own results (Opus training-speedup numbers, the automated-alignment PoC). The recursive-self-improvement framing supports Anthropic's case for proactive governance and its alignment agenda. Weight the benchmark trends; discount the takeoff timeline.

## Argument
Builds a "mosaic" from many benchmarks (acknowledging each is individually flawed):
- **Coding singularity:** SWE-Bench went from Claude 2 ~2% (late 2023) to Claude Mythos Preview 93.9% (saturating). METR time-horizons: ~30s (GPT-3.5, 2022) → 4min (GPT-4, 2023) → 40min (o1, 2024) → ~6h (GPT 5.2, 2025) → ~12h (Opus 4.6, 2026); Cotra (METR) projects ~100h by end of 2026.
- **AI-R&D-core skills:** CORE-Bench (reproduce a paper) ~21.5% (Sept 2024, GPT-4o) → 95.5% / 'solved' (Dec 2025, Opus 4.5). MLE-Bench (Kaggle) 16.9% → 64.4% (Gemini3+search). PostTrainBench: AI gets ~half human uplift (Opus 4.6/GPT 5.4 at 25-28% vs 51% human). Anthropic's CPU-LM-training-speedup task: 2.9× (Opus 4, May 2025) → 16.5× (Opus 4.5) → 30× (Opus 4.6) → 52× (Mythos Preview, Apr 2026) vs a human's 4× in 4-8h. Automated-alignment PoC (#454): agents beat a human baseline on scalable oversight at small scale.
- **Management meta-skill:** single agents now supervise sub-agents (Claude Code, OpenCode) → "synthetic teams."
- **Relativity or Lego?** AI can't yet invent radical new ideas, but "the technology may not need to" — most AI progress is "meat and potatoes" engineering schlep (scale, see what breaks, fix, scale), which AI is now good at. Preliminary creativity signs: a Gemini model resolving open Erdős-1051; a centaur math proof with Gemini. Caveat: math/CS may be unusually AI-amenable; Move 37 hasn't been topped in ten years (weakly bearish).
- **Industry intent:** OpenAI wants an "automated AI research intern by Sept 2026"; Anthropic publishes on automated alignment researchers; Recursive Superintelligence raised $500m, Mirendil targets AI-R&D — hundreds of billions aimed at this goal.
- **Why it matters:** (1) alignment must be near-perfect under recursion (compounding error: 99.9% → 60.5% accurate after 500 generations); (2) productivity multiplier everywhere → access inequality + an "Amdahl's Law for the economy" (physical-world bottlenecks like drug trials); (3) a **capital-heavy, human-light "machine economy"** growing inside the human economy, eventually fully autonomous AI-run corporations posing novel governance challenges.

## Why it matters / where it cuts
The radar's clearest perspective-layer statement of the **recursive-self-improvement / [[self-evolving-agents]] thesis** from a frontier-lab insider — and notable because Clark grounds it in *checkable benchmark trends* (METR, SWE-Bench, MLE-Bench, PostTrainBench) rather than vibes, which is its real value to the exec. The "machine economy" and compute-allocation points feed [[governance-gap]] and [[frontier-model-governance]]: if even a fraction of this holds, *where AI compute gets allocated* becomes a politically charged macro variable, not a procurement detail. Sanity-check: the timeline is Clark's (and Anthropic-aligned); the underlying coding/AI-R&D capability curves are independently observable and the radar's own [[coding-agents]] and [[agent-evaluation]] nodes corroborate the direction.

## Graph
- **Author:** [[jack-clark]]
- **Concepts:** [[self-evolving-agents]] · [[coding-agents]] · [[frontier-model-training]] · [[agent-evaluation]] · [[governance-gap]]
- **Entities:** [[anthropic]] · [[openai]] · [[google-deepmind]] · [[swe-bench]] · [[mle-bench]] · [[claude]]
- **Related:** [[2025-10-13-blog-clark-technological-optimism-appropriate-fear]]
- **Raw:** `raw/blogs/2026-05-04-clark-automating-ai-research.md`
