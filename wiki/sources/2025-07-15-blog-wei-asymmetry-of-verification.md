---
type: source
source_type: blog
title: "Asymmetry of verification and verifier's rule"
author: Jason Wei
outlet: jasonwei.net
url: https://www.jasonwei.net/blog/asymmetry-of-verification-and-verifiers-law
resource: https://www.jasonwei.net/blog/asymmetry-of-verification-and-verifiers-law
date: 2025-07-15
stake: Frontier-lab reasoning/RL researcher (OpenAI at time of writing; → Meta Superintelligence Labs Jul 2025) — talks the book on RL/verifiable-reward training being the path forward
ingested: 2026-06-22
tags: [perspective, agentic-rl, reasoning-models, agent-evaluation]
---

# Asymmetry of verification and verifier's rule

**Blog** · Jason Wei (jasonwei.net) · 2025-07-15 · [link](https://www.jasonwei.net/blog/asymmetry-of-verification-and-verifiers-law)

**The take (attributed):** Wei argues that **with RL "that finally works in a general sense," verifiability is now the master variable for AI progress** — "all tasks that are possible to solve and easy to verify will be solved by AI." Capability advances will be *jagged*, racing ahead exactly where tasks are cheap to check.

**Stake:** OpenAI reasoning/RL researcher (coined chain-of-thought prompting; worked on o1 and deep research); moved to Meta Superintelligence Labs the same month. He's articulating the worldview that justifies the RL-on-verifiable-rewards program he builds — read his bullishness on "anything measurable will be solved" at that discount.

## Argument
- **Asymmetry of verification** = some tasks are far easier to verify than to solve (Sudoku, building Instagram, [[browsecomp|BrowseComp]] tasks). Some are near-symmetric (adding 900-digit numbers); a few invert — harder to verify than to propose (fact-checking an essay; testing a novel diet), per Brandolini's law.
- You can **improve** the asymmetry by front-loading research: an answer key trivializes checking a math answer; test cases with coverage trivialize checking code (what Leetcode does).
- **Verifier's rule:** "ability to verify solutions is equivalent to ability to create an RL environment," so *"the ease of training AI to solve a task is proportional to how verifiable the task is."* Five properties decide trainability: objective truth, fast to verify, scalable to verify, low noise, continuous reward. Most popular ML benchmarks of the last decade fit #1–4 — and have been solved.
- **Why it's the master variable:** neural-net learning is maximized when those properties hold — "a lot of gradient steps where each step has a lot of signal." Iteration speed is *the* reason digital progress outruns physical progress.
- **[[alphaevolve|AlphaEvolve]]** is the marquee example — "a very clever instantiation of guess-and-check" ruthlessly optimizing a verifiable objective; such single-problem optimization is legitimately "train=test."
- **Vs P=NP:** verifier's rule makes no claim about solve-time, and is broader — it covers non-computational tasks (best catalyst, best aerodynamic design) wherever you can measure quickly and at scale.

## Why it matters / where it cuts
This is the cleanest one-line statement of the operating thesis driving the whole reasoning-model wave: **build a verifier, get the capability.** For the exec it's a portable filter — when assessing whether AI will eat a given task, ask "how cheaply and objectively can a good answer be checked?" It also names the **jagged frontier** ("AI much smarter at verifiable tasks") that explains why agents are superhuman at code/math yet shaky on fuzzy, hard-to-verify work — the mirror image of [[2026-01-22-blog-leike-alignment-not-solved|Leike's]] "hard fuzzy tasks don't benefit from reasoning" finding, and a sharp input to [[debate-llms-path-to-agi]].

## Graph
- **Author:** [[jason-wei]]
- **Concepts:** [[agentic-rl]] · [[reasoning-models]] · [[agent-evaluation]]
- **Entities:** [[alphaevolve]] · [[browsecomp]] · [[rlvr]] · [[chain-of-thought]]
- **Debate:** [[debate-llms-path-to-agi]]
- **Raw:** `raw/blogs/2025-07-15-jason-wei-asymmetry-of-verification.md`
