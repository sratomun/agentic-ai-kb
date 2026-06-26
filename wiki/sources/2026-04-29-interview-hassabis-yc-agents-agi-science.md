---
type: source
source_type: interview
title: "Demis Hassabis: Agents, AGI & The Next Big Scientific Breakthrough"
author: Demis Hassabis (in conversation with Garry Tan, YC)
outlet: Y Combinator — "How to Build the Future" (live)
url: https://www.youtube.com/watch?v=JNyuX1zoOgU
resource: https://www.textpurr.com/transcript/demis-hassabis-agents-agi-the-next-big-scientific-breakthrough
date: 2026-04-29
stake: DeepMind CEO + Nobel laureate — talks the AGI-capability / science book; Gemini, Gemma, Isomorphic are his
ingested: 2026-06-22
tags: [perspective, agentic-ai, reasoning-models, science-agents, world-models, open-models]
---

# Hassabis at YC: Agents, AGI & the Next Scientific Breakthrough (2026-04-29)

**Interview / fireside** · Demis Hassabis (Y Combinator "How to Build the Future," Garry Tan) · 2026-04-29 · [link](https://www.youtube.com/watch?v=JNyuX1zoOgU) · [transcript](https://www.textpurr.com/transcript/demis-hassabis-agents-agi-the-next-big-scientific-breakthrough)

**The take (attributed):** Hassabis argues the **current paradigm (pre-training + RLHF + chain-of-thought) is mostly the final architecture** — "I can't see a world in which… this was a dead end" — but **continual learning, long-term memory, long-horizon reasoning, and consistency are genuinely unsolved**, and he puts it at "about 50/50" whether closing them needs "one or two big ideas" vs. just scaling. AGI "like 2030." **Agents are the path to AGI but "we're just getting going,"** and the missing piece blocking fire-and-forget agents is precisely continual learning.

**Stake:** CEO of [[google-deepmind|Google DeepMind]] ([[gemini|Gemini]], [[open-models|Gemma]]) and co-founder/CEO of Isomorphic Labs; 2024 Nobel laureate. He talks his book on (a) AGI ~2030 and the science-discovery thesis, (b) Gemini's multimodal-from-the-start edge for [[world-models]]/robotics, and (c) Gemma as the "Western open stack." Discount the product-superiority claims; weight the candid capability-gap diagnosis heavily — it's unusually specific and self-critical for a frontier CEO.

## Argument
- **What's missing for AGI:** continual learning, long-term reasoning, "some aspects of memory," and cross-board consistency. "It might be that the existing techniques can just scale… but it could be that there's still one or two big ideas left… my betting is about 50/50." Not more than one or two if any.
- **Memory / continual learning is the agent bottleneck.** Today's systems are "stateless"; we're "cobbling it together with duct tape" (long context windows). A 1M-token window is "working memory" but "pretty brute force" — and only ~20 min of live video. Drawing on his hippocampus PhD: the brain consolidates via replay during REM sleep (DeepMind's 2013 DQN borrowed this as "experience replay"). **Not having continual learning is "one of the things holding back agents from doing full tasks"** — they can't adapt to your specific context, so they're not yet "fire and forget."
- **RL/search heritage is resurfacing.** Thinking modes / chain-of-thought are "aspects of what was… pioneered with AlphaGo." DeepMind is "relooking at" Monte Carlo tree search and AlphaZero-era ideas "at scale… in a more general way" — expect that to drive "the advances the next few years."
- **Reasoning is jagged and brittle.** Lots of headroom left in thinking paradigms (e.g. monitoring/interjecting mid-chain-of-thought). Models "overthink," loop, and — playing chess vs. Gemini — will see a blunder, fail to find better, and play it anyway. Solves IMO-gold problems yet makes elementary errors: "jagged intelligence." Suspects something missing around **introspection on its own thought process**.
- **Agents: just getting started, not overhyped — but unproven at scale.** "We're only in maybe the last couple of months starting to find the really valuable places." Skeptical of the "set off dozens of agents for 40 hours" pattern — "I'm not sure I've seen the output… justify that level of input." Tell-tale: no live-coded AAA hit game tops the charts yet, so "something's still somehow missing… craft and human soul and taste." Expects the value to land "in the next 6 to 12 months," with humans operating at 1,000x *before* full autonomy.
- **Distillation + small/edge models are a core GDM strength.** Frontier capability requires the biggest models, but DeepMind ("we invented the kind of distillation process") packs it into Flash/Flash-Lite/Gemma for >12 dozen-billion-user surfaces. No known informational limit yet; frontier capability reaches edge models within ~6–12 months. **Edge models are deliberately open** (Gemma, "nano-size") because once on-device they're "vulnerable anyway." 40M Gemma downloads in ~2.5 weeks. Wants "Western stacks on open source" since "a lot of the Chinese models are… currently world-leading in open source."
- **Multimodal-from-the-start = the world-model/robotics bet.** Genie builds on Gemini; Gemini Robotics and Waymo use it; assistants on phones/glasses need intuitive physics. Claims GDM is "far and away the strongest" on physical-world understanding.
- **Inference won't be free** (Jevons paradox) — "millions of agents, swarms," or single agents ensembling many directions, will absorb whatever's available; rationing persists for decades.
- **Science is the destination ("root node problems").** Original mission: "solve intelligence… then use it to solve everything else" — and he means everything. AlphaFold is the prototype (3M+ researchers; "almost every drug discovered from now on will have used AlphaFold"). Isomorphic Labs (spun out post-AlphaFold 2) is doing the adjacent chemistry; "big announcements very soon." A **virtual cell** is ~10 years out (starting with a self-contained nucleus); the data bottleneck is imaging a *live* cell without killing it. Other domains (materials, math) are near an "AlphaFold-one moment."
- **The AlphaFold breakthrough pattern (his heuristic):** a problem works for these methods if it's (1) a massive combinatorial search space (no brute-force/special-case solution), (2) has a clear objective function to hill-climb, and (3) has enough data or a simulator for in-distribution synthetic data. Drug discovery fits: "there is a compound out there… as long as the laws of physics allow it, the only question is how to find it efficiently."
- **Genuine scientific creativity is the frontier and the gap.** Co-Scientist and AlphaFold-class systems go "a little bit beyond" base Gemini, but he's "yet to see… a true genuine massive discovery." Inventing — not solving — needs "analogical reasoning… beyond the bounds of what's known," which "I don't think these systems have." His **Einstein test:** train to a 1901 knowledge cutoff; does it produce 1905 special relativity? "Not magical," but "maybe we're missing one or two things." Wants to invent (not just solve) new Millennium-Prize-class problems; favorite to crack: P=NP.
- **Architecture bet for the AGI era:** not "one giant brain." Better to have strong general **tool-using** models (Gemini/Claude) that call specialist systems (AlphaFold-like) as tools — putting all proteins into Gemini "would have too much regression" and hurt its language skills. Founders on a 10-year deep-tech path should "consider AGI appearing in the middle of that journey."

## Why it matters / where it cuts
The 2026 counterpart to his 2025 TIME interview — same destination (scientific superintelligence), but the *capability diagnosis* has sharpened from "5–10 years, missing pieces" to a precise, falsifiable gap list (continual learning, memory, introspective reasoning) with a 50/50 hedge on whether scaling closes it. This is the strongest "the-paradigm-is-basically-right, agents-are-the-path" voice for [[debate-llms-path-to-agi]] — and notably it concedes more to the skeptics than his public timeline suggests (agents unproven at scale; no autonomous scientific discovery yet; the "duct tape" memory critique). So what: watch his **continual-learning / memory** framing as the named blocker on enterprise-grade fire-and-forget [[agentic-ai|agents]], and the **tool-calling-orchestrator over monolithic-model** architecture call.

## Graph
- **Author:** [[demis-hassabis]]
- **Entities:** [[google-deepmind]] · [[gemini]] · [[anthropic]] · [[deepseek]]
- **Concepts:** [[agentic-ai]] · [[reasoning-models]] · [[agentic-rl]] · [[agent-memory]] · [[science-agents]] · [[world-models]] · [[open-models]] · [[distillation]]
- **Debate:** [[debate-llms-path-to-agi]]
- **Raw:** `raw/blogs/2026-04-29-hassabis-yc-agents-agi-science.md`
