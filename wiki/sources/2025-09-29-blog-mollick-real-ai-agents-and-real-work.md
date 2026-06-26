---
type: source
source_type: blog
title: "Real AI Agents and Real Work"
author: Ethan Mollick
outlet: One Useful Thing
url: https://www.oneusefulthing.org/p/real-ai-agents-and-real-work
resource: https://www.oneusefulthing.org/p/real-ai-agents-and-real-work
date: 2025-09-29
stake: Wharton/UPenn associate professor; Co-Intelligence author — adoption/practitioner-optimist voice
ingested: 2026-06-22
tags: [perspective, agentic-ai, agent-adoption, agent-evaluation]
---

# Real AI Agents and Real Work

**Blog** · Ethan Mollick (One Useful Thing) · 2025-09-29 · [link](https://www.oneusefulthing.org/p/real-ai-agents-and-real-work)

**The take (attributed):** Mollick argues AI has "quietly crossed a threshold: they can now perform real, economically relevant work" — but the unit that's changing is **tasks, not jobs**, and whether agents make us more capable or just bury us in slop "isn't in the AI, it's in how we choose to use it."

**Stake:** Wharton/UPenn professor of entrepreneurship; author of Co-Intelligence — an adoption-optimist who gets early access to frontier models (Claude Sonnet 4.5 here). Weight the hands-on demos and the task-vs-job framing; discount the optimism.

## Argument
- Anchors on OpenAI's **GDPval**: experts (avg 14 yrs experience, finance/law/retail) designed realistic 4–7-hour tasks; AI and human experts both did them; a third expert group blind-graded. Humans "won, but barely." Per Mollick, the striking finding is that AI lost mainly on **formatting and instruction-following**, not hallucinations — "areas of rapid improvement" — so "the next generation of AI models should beat human experts on average."
- Core distinction he presses: GDPval measures **tasks, not jobs**. Jobs are bundles of tasks; AI doing some tasks "shifts what I do," it doesn't replace the job while AI stays jagged and can't do complex human interaction.
- The "very valuable task" demo: he gave **Claude Sonnet 4.5** an economics paper plus its full replication dataset and a minimal prompt; without further instruction Claude read the paper, sorted the archive, converted STATA → Python, and reported a successful reproduction (he verified with GPT-5 Pro). His bigger claim: the academic **replication crisis** could be partly resolved at scale — "implications for all of scientific research."
- On why agents suddenly work: the old limit was a human guiding each step (one error killed a long chain). He cites a Sept 2025 paper (arXiv 2509.09677) — small accuracy gains yield large gains in task length, and "thinking" models **self-correct**, so errors don't stop them. Cites **METR's** length-of-task curve as consistent exponential progress GPT-3 → GPT-5.
- The under-discussed risk: not just labor replacement, but "using agents to do more of the tasks we do now, unthinkingly." His "17 PowerPoints" demo is the nightmare. The GDPval-derived workflow (delegate → review → 1–2 corrections → else do it yourself) gets work **40% faster, 60% cheaper** while retaining control.

## Why it matters / where it cuts
An early, dated, practitioner marker that agents crossed the "real work" line in late 2025 — and a clean framing for the exec: capability is real but bounded to tasks, and the org-level risk is slop-at-scale, not just headcount. Feeds [[agent-adoption]] (how orgs should deploy agents) and the capability-evaluation thread under [[agent-evaluation]] (GDPval as a from-the-user's-seat benchmark). Sets up his Jan 2026 [[2026-01-07-blog-mollick-claude-code-and-what-comes-next|Claude Code]] and [[2026-01-27-blog-mollick-management-as-ai-superpower|Management as AI superpower]] posts.

## Graph
- **Author:** [[ethan-mollick]]
- **Concepts:** [[agentic-ai]] · [[agent-adoption]] · [[agent-evaluation]] · [[coding-agents]]
- **Entities:** [[claude]] · [[anthropic]]
- **Raw:** `raw/blogs/2025-09-29-mollick-real-ai-agents-and-real-work.md`
