---
type: reference
tags: [meta, style-guide]
updated: 2026-06-22
---

# Node style guide — how we write the radar's knowledge graph

The single source of truth for *how* nodes read and connect. Templates in this
folder (`concept-node`, `entity-node`, `source-note-*`) are the *structure*; this
file is the *voice and rules*. The schema (`../../CLAUDE.md`) covers architecture;
this covers node quality. When in doubt, conform to this.

## Voice
- Write for **a senior AI/tech exec** who wants signal, not a textbook.
  Lead with the implication; define just enough to ground it.
- Warm, direct, opinionated. No jargon dumps, no breathless hype, no "in recent years".
- Every node answers, in order: **What it is → Why it matters → How it connects.**
  (Concepts add a synthesis section; entities stay tight.)

## Year-agnostic framing
- Nodes are **living syntheses**, not dated snapshots. Never imply a given year is
  "now" (no "Threads (2026)", no "the 2026 signal"). Use **Foundations / Recent
  developments**, and let the dated `[[source notes]]` carry the timeline.
- The evidence section must **braid years into one story** — lead with the
  foundational (usually most-cited) work, then what changed recently. Do not park a
  year's papers in a link-list while synthesizing only from another year.

## Grounding (non-negotiable)
- Synthesis prose must be grounded in the **full text** of the papers it cites
  (real methods, results, numbers from `raw/arxiv/<id>.fulltext.md`), **not
  abstracts**. Abstracts are for the auto-ingested browsable layer only.
- Never invent findings. If a number isn't in the paper, don't write it.

## Graph hygiene
- **No orphans:** every node has ≥1 inbound and ≥1 outbound link.
- **Reciprocal links:** if A links B as a relationship, add the back-link on B.
- **Promote node-worthy references:** recurring named models / benchmarks / methods /
  orgs / protocols become their own entity nodes (check for an existing node or alias
  first — don't duplicate).
- **Frequency-justify new nodes.** Create a concept/entity only when the corpus
  supports it (a recurring theme or a name that appears across multiple papers).
  Prefer folding a thin sub-theme into a parent over spawning a stub.
- **Fold vs split:** if you fold a sub-theme into a parent hub, name it in the
  parent's `## Includes` section so a reader knows it's aggregated there.
- **Citation lists are machine-maintained.** `## Key papers` and `## Cited by` are
  written/refreshed by the kg-curator skill from Semantic Scholar data — don't
  hand-edit; fix the source data or the curator.

## Tiers (what depth a source note gets)
1. **Census** — every matching paper as metadata in `raw/arxiv/<year>-census/`. Not
   in the graph.
2. **Browsable** — abstract-only auto-notes (`source-note-abstract`), keyword-linked,
   filtered out of the global graph view.
3. **Deep** — full-text reads with analysis (`source-note-deep` / `-survey`),
   first-class graph nodes.

## Perspective layer (blogs, people, debates)
The blog-scanner adds *opinion*, which is handled differently from research/news facts:
- **Attribute, never launder.** A blog claim is "X argues…", not a radar fact. Keep
  the hedge; the authority is the person, not us.
- **Tag the stake.** VCs and lab leaders talk their book — record a `stake:` field
  (their fund / lab / product) on commentary source notes and person nodes so the view
  is read at the right discount.
- **Commentary capture is opportunistic.** Marquee figures (VCs, scientists) mostly
  speak on X/podcasts/talks — capture via WebSearch + Claude in Chrome transcripts
  (`source_type: interview|talk|post`); audio with no transcript is out of scope.
  Verify a person's current affiliation via WebSearch before writing their node.
- **People are nodes.** Promote recurring authors to `person` entity nodes
  (`entity_type: person`, template `person-node.md`) and link post↔person both ways.
- **Disagreement is a node.** When sources take opposing positions on a contested
  question, capture it as a `comparison`/`debate` note in `comparisons/`
  (`debate-note.md`): state the question neutrally, attribute each side to its people,
  and link the evidence each cites. These are the radar's map of *where the field
  disagrees* — its most differentiated content.
- **Cross the layers honestly.** In a debate's "Where it stands", say what the
  *research* layer (arxiv) shows vs the *opinion* layer — without overclaiming.

## OKF compatibility (keep us export-clean)
This wiki is built to convert cleanly to [[open-knowledge-format|OKF]] via the
kg-curator `okf-export` operation (we author in Obsidian wikilinks; export rewrites
them to markdown-link edges). To keep that cheap:
- **Every node keeps a non-empty `type`** in frontmatter (OKF's only hard requirement).
- Keep links **resolvable** (export maps `[[slug]]`→`[Display](/path.md)`; unresolved
  slugs become tolerated-but-ugly broken edges).
- Prefer `url`/`updated` fields (export aliases them to OKF `resource`/`timestamp`).
- We do NOT convert wikilinks in place — that would break Obsidian. Conformance is an
  export artifact, not an authoring constraint.

## Lint checklist (run every curation pass)
Broken `[[links]]` = 0 · orphans = 0 · no duplicate sections · no year-stamped
framing in node headers · citation lists fresh · `_templates/` excluded from the
graph view and from lint.
