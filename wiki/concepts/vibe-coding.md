---
type: concept
tags: [agents, coding-agents, vibe-coding, practice, perspective]
created: 2026-06-22
updated: 2026-06-22
kind: crosscutting
---

# Vibe Coding

*Building software by prompting an LLM and accepting the result **without reviewing the code** — intuition-driven, conversational, human-in-the-loop programming.*

## What it is
A term coined by Andrej Karpathy (Feb 6 2025): "fully give in to the vibes… forget that the code even exists" — describe what you want in natural language, run it, paste errors back, accept the diffs unread. [[simon-willison]] sharpened the definition to its load-bearing core: **vibe coding = building software with an LLM without reviewing the code it writes.** That review boundary is what separates it from disciplined AI-assisted [[coding-agents|agentic coding]] and [[harness-engineering|vibe engineering]] — where you read, test, and can explain every line. It borders [[coding-agents]] (the autonomous end), [[agent-adoption]] (who's newly able to build), and [[agent-security]] (where it bites).

## Why it matters
This is the year's most consequential shift in *who* can build software — and the radar's clearest case of semantic diffusion to watch. For the exec the decision-relevant split is: vibe coding democratizes low-stakes tool-building (the learning curve "shaved down to almost flat") and is a fast way to build intuition, but the same "don't read the diffs" posture is a security and cost liability the moment stakes rise. The strategic read: encourage it for prototyping and enablement; gate it hard for anything touching secrets, money, or production.

## What the evidence shows
**The taxonomy (research layer).** The most-cited treatment, *Vibe Coding vs. Agentic Coding* (60 citations), draws the formal line: vibe coding is **intuitive, human-in-the-loop, reactive-feedback** programming for ideation/prototyping/education; agentic coding is **goal-driven autonomy** (plan-execute-test-iterate) for enterprise automation and CI/CD. Its conclusion is "harmonize, don't choose" — natural-language interfaces coupled to autonomous execution pipelines (→ [[2025-05-26-arxiv-2505-19443v1-vibe-coding-vs-agentic-coding-fundamentals-and-practical]]).

**The definition fight (perspective layer).** [[simon-willison]] anchored the term and warned against diluting it (→ [[2025-03-19-blog-willison-not-all-vibe-coding]]), then named the responsible counterpart "vibe engineering" — noting by Feb 2026 the field is settling on "**agentic engineering**" instead (→ [[2025-10-07-blog-willison-vibe-engineering]]). [[ethan-mollick]] frames vibe-coded coding agents as general-purpose tools for non-coders (→ [[2026-01-07-blog-mollick-claude-code-and-what-comes-next]]); [[nathan-lambert]] argues the skill is now *using* agents well, not writing code (→ [[2026-01-21-blog-lambert-get-good-at-agents]]); [[simon-willison]]'s year-end read marks coding as the breakout domain (→ [[2025-12-31-blog-willison-the-year-in-llms]]).

*Caveat: "vibe" is now a productivity-marketing prefix (VibeSearchBench, Vibe-AIGC in the 2026 census) — discount the label, weight the review-or-not distinction.*

## Relationships
- coined by [[andrej-karpathy]] (Feb 6 2025)
- the disciplined counterpart: [[harness-engineering|vibe engineering]] / agentic engineering; the autonomous end: [[coding-agents]]
- enablement angle: [[agent-adoption]]; liability angle: [[agent-security]]
- perspective voices: [[simon-willison]] (definition), [[ethan-mollick]], [[nathan-lambert]]
- contrasted with autonomy in [[debate-agents-vs-workflows]]

## Key sources
- **research** · [[2025-05-26-arxiv-2505-19443v1-vibe-coding-vs-agentic-coding-fundamentals-and-practical|Vibe Coding vs. Agentic Coding (taxonomy)]]
- **definition** · [[2025-03-19-blog-willison-not-all-vibe-coding]] · [[2025-10-07-blog-willison-vibe-engineering]]
