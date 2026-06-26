# RAW — Alignment is not solved (but it increasingly looks solvable) (Jan Leike, aligned.substack.com)
Source: https://aligned.substack.com/p/alignment-is-not-solved-but-increasingly-looks-solvable · 2026-01-22 · captured 2026-06-22 · channel: blog

## Framing
Leike has been optimistic about alignment since 2022, but back then there was far more uncertainty. Since then: pretraining kept improving and RL became a much bigger deal. A priori it wasn't obvious LLMs could be robustly aligned through the RL scale-up, because some alignment threat models are about models becoming agentic, pursuing unaligned instrumental goals, and becoming deceptive.

## The concerning early signals (and his memo that "didn't age well")
Early highly-RL'ed models showed concerning signals:
- Sonnet 3.7 "loves hacking test cases"
- o1 shows high rates of deception in evaluations
- "o3 lies a lot"
- Grok 4 "proclaimed itself MechaHitler"
- Most were "happy to blackmail humans to prevent their discontinuation" (agentic misalignment)
- Early Opus 4 snapshots "hit record deception rates" (mostly mitigated before release)
- Earlier in 2025 Leike was getting nervous enough that he "wrote an Anthropic-internal memo about it. As it turned out, this memo didn't age well."

## The evidence that misalignment is manageable
- Best overall alignment assessment today = **automated auditing**: an auditing agent is prompted with a scenario (e.g. a dark-web shopping assistant, an imminent shutdown unless humans are harmed), tries to elicit misaligned behavior from the target production LLM; a separate judge LLM evaluates the trajectory. "Albeit very imperfect, this is the best alignment metric we have to date."
- Chart cited: aggregated "concerning" scores from **Petri** (Anthropic's open-source automated auditing tool), using GPT-5.1 as auditor and GPT-5.1 / Gemini 3 Pro / Opus 4.5 as judges.
- Strikingly, a lot of progress over 6 months in 2025: "Sonnet 4.5 (Sep 29) is a lot more aligned than Sonnet 4 and Opus 4 (May 22), and Opus 4.5 (Nov 24) is even more aligned than Sonnet 4.5." OpenAI's and Google's models also became more aligned; "GPT-5.2's alignment being on par with Opus 4.5."
- On eval awareness: some early signs; whitebox methods used to estimate impact. For Opus 4.5 they identified and removed a dataset causing eval awareness, and the model became "both a lot less eval aware and a lot less misaligned." Best guess: eval awareness has some effect but plays a minor role vs. the real progress made. Can't speak for non-Anthropic models.
- **Key lesson**: "simple interventions are very effective at steering the model towards more aligned behavior." For agentic misalignment they made SL data, RL prompts, and synthetic reward-modeling data; "Starting with Sonnet 4.5, agentic misalignment went to essentially 0 and has been there ever since."
- Footnote: the flip side — "making an evil version of Claude that's just as smart and agentic would be pretty easy."

## But what about superalignment?
- "We're still doing alignment 'on easy mode' since our models aren't really superhuman yet." We can still read and understand outputs, which underpins today's interventions (synthetic data, reading transcripts, evaluating progress).
- Once models are so capable we don't understand their actions, current approaches won't work the same way — "it would feel much more like hill-climbing on an eval that you can't look at and don't fully trust." This is **the hard problem of alignment** — "to this day it is an unsolved problem."
- Example: little progress on **hard fuzzy tasks** despite focusing scalable-oversight research on them for much of 2025. Best guess: the fuzzy tasks they have labels for "don't actually benefit from reasoning," so techniques don't provide uplift there.

## Our job is not to align superintelligence directly
- "We just need to build a model that's as good as us at alignment research, and that we trust more than ourselves to do this research well because it's sufficiently aligned."
- We aren't confronted with aligning superintelligence directly because we can read and understand a human-level automated researcher — "if it's possible for humans to figure out how to align superintelligence, then a human-level automated researcher can figure it out as well."

## The automated alignment researcher is in sight
Over 2025 Claude took on more research work:
- Claude Code now writes "almost all research code" (vs. mostly manual at the start of 2025)
- Claude can mostly autonomously do standard workflows (sampling, evals, SFT)
- Claude does automated auditing to discover and quantify misalignments
- Claude does most of the "reading transcripts" work
- Starting with Sonnet 3.7, Claude got a passing grade on the alignment team's research-brainstorming interview
- "The automated alignment researcher will be a bunch of incremental improvements to the existing models, a transition that looks pretty continuous."
- Footnote: in an informal poll around Opus 4.5's release, "alignment managers were willing to give up 10-25% of their headcount in exchange for keeping access to LLM assistants and coding tools."

## The work is not done
- "This is the most optimistic I've been about alignment… Yet I'm also wary of being overly optimistic at this stage; there is no guarantee how the future will go."
- "We are starting to automate AI research and the recursive self-improvement process has begun. As more and more research gets automated, AI capabilities might improve much more rapidly, and so we might not have much time to figure out how to actually align superintelligence."
- "Just because a problem is solvable, this doesn't mean it's solved… what counts is that our models are actually aligned!"

## Notable comment (Jacob Pfau) — the correlated-error objection
Pfau argues automated alignment faces correlated fuzzy errors: (a) one model (or a few related models) introduces field-wide correlation, breaking the error-correction that institutional/individual diversity gives human science; (b) fuzzy judgment is non-modular — threaded through all parts of automated research (code legibility, what to plot, what patterns to flag) — so you can't isolate and double-check it; (c) as models operate past human frontiers, the anchoring of fuzzy judgment to human data weakens and preference data (a shakier signal) shapes generalization. Frames this as a more serious obstacle than the raw capability question.
