---
name: blog-scanner
description: Scan technical blogs and essays from named authors and labs to add industry perspective to the exec's AI Tech Radar knowledge graph. Captures durable technical posts (deep-dives, post-mortems, opinion) — NOT newsletters/roundups — promotes authors to person nodes, and records contested positions as attributed stance/debate notes. Use when the exec says "scan blogs", "what are people writing/saying", "industry perspective", "what's the take on X", or "run the blog scanner".
---

> Lives in `/Skills/blog-scanner/`. Reads/writes the wiki under `../../`.
> The third scanner: arxiv = *what's true*, news = *what happened*, this = *what it
> means / who thinks what*. Before writing any node, read the **source of truth**:
> `../../wiki/_templates/STYLE.md` + the `_templates/*.md`, plus
> `../../CLAUDE.md` and `../../scanners.md`.

# Blog Scanner

Adds the **perspective layer** to the radar: attributed technical opinion from the
people and labs shaping the field. Distinct from the news/briefing layer — this
captures *durable technical essays*, not roundups.

## Triggers
"scan blogs", "what are people writing/saying", "industry perspective on X",
"what's the take on <topic>", "run the blog scanner".

## Run parameters (caller-supplied, not hardcoded)
- **`scope` (date window)** — which years/dates to cover. the exec sets this per run
  ("cover 2025 & 2026", "just this quarter", "everything since 2023"). Default if the exec
  says nothing: **last ~30 days**. The window is an *argument*, never a property of the
  skill — don't bake a year into the workflow.
- **What "scope" governs:** which posts to *newly capture and synthesize* in this run.
  It is **not** a delete filter. Older posts already in the graph stay — they're the
  genealogy of the current work and are load-bearing in debate/person nodes. Never purge
  existing captures just because they fall outside this run's window.
- **`focus` (optional)** — a topic to target instead of a general sweep ("the take on
  evals"). **`authors` (optional)** — limit to specific people/labs.

## What counts (and what doesn't)
- **In:** technical deep-dives, architecture/engineering posts, post-mortems,
  benchmark write-ups, and *opinionated* essays/stances from the authors and labs in
  scanners.md "Technical blogs".
- **Out:** newsletters/roundups (News layer), pure product marketing, release notes,
  SEO content, reposts of papers we already have from arxiv-scanner.

## Steps
1. **Gather.**
   - **Technical blogs:** discover each source's RSS/Atom feed and pull recent posts
     (`web_fetch`); fall back to fetching the page. Default lookback ~30 days (blogs are
     slower-moving than news); or target a topic when asked ("the take on evals").
   - **Leaders & commentary** (the VCs/scientists in scanners.md who don't blog):
     `WebSearch` for their notable recent piece, then use **Claude in Chrome**
     (`navigate` → `get_page_text`) to read the **transcript** — YouTube auto-captions
     (open the transcript panel), published podcast transcripts, or X threads as text.
     `web_fetch` first; Chrome only where gated/JS. **Audio with no transcript page is
     out of scope** — note and skip. Lower capture rate is expected.
2. **Filter** to technical + agents-relevant per the "what counts" rule. Drop the rest.
3. **Dedup** by canonical URL against `../../raw/blogs/`, `raw/news/`,
   and `index.md`. Skip posts that just re-summarize a paper already ingested.
4. **Capture (FULL POST BODY).** Write the real source to
   `../../raw/blogs/<date>-<author-slug>-<slug>.md` — metadata (title,
   author, outlet, URL, date) + full text. raw is immutable.
5. **Ingest as perspective** (template `_templates/source-note-blog.md`, `source_type:
   blog`). Read the full post, then:
   - Write a source note that **attributes the view to its author** — capture the
     *claim/stance/argument*, not just facts. Use hedged language ("X argues…", "per
     Y…"); never launder opinion into radar fact. `source_type:` = `blog` for essays,
     `interview` / `talk` / `post` for commentary captured via Chrome.
   - **Tag the stake.** Add a `stake:` line noting the speaker's incentive (their fund,
     the lab/product they sell) so the view is read at the right discount. VCs and lab
     CEOs talk their book.
   - **Promote the author to a `person` entity node** (`_templates/person-node.md`,
     `entity_type: person`) if not present — **verify their current affiliation via
     `WebSearch`** (titles change), record who they are and their stake, and link
     post↔person reciprocally. This is how the graph gains a "who's-saying-what" layer.
   - Link the post to the **concepts/entities** it touches (sibling links as usual).
6. **Capture debates** (the differentiator). When a post takes a position on a
   *contested* question (e.g. agents-vs-workflows, RL-vs-scaffolding, "evals are
   broken", SLMs-vs-frontier), create/append a **stance note** in
   `../../wiki/comparisons/` (`_templates/debate-note.md`): state the
   question neutrally, then list each side with **who holds it and why**, linking the
   person nodes and source posts. Over time these become the radar's map of where the
   field disagrees.
7. **Integrity check.** No orphans, no broken `[[links]]`; reciprocal links on both
   ends; opinions attributed. Fix and log a one-line `lint` entry if needed.
8. **Report back** in chat: notable posts, new person nodes, debates updated, and the
   3–5 perspective signals worth attention — drawn from the `log.md` entry. No digest
   file; `index.md` + `log.md` are the record.

## Notes
- Respect the web-content rules: if `web_fetch` reports a domain can't be fetched,
  don't work around it — note it and move on.
- Maintenance of existing nodes (normalize, lint, enrich) is the kg-curator skill's job.
- Drafts/notes only; never emails or posts.
