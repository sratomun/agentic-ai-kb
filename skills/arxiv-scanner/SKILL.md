---
name: arxiv-scanner
description: Scan arXiv for new AI-agents research and compile it into the exec's AI Tech Radar knowledge wiki. Captures papers to raw/, then ingests them into interlinked concept/entity pages. Use when the exec says "scan arxiv", "any new agent papers", "check arxiv", or "run the arxiv scanner".
---

> Lives in `/Skills/arxiv-scanner/`. Reads/writes the wiki under `../../`.

# arXiv Scanner

Feeds the AI Tech Radar wiki. Before writing any node, read the **source of truth**:
`../../wiki/_templates/STYLE.md` (voice + rules) and the
`_templates/*.md` (node structure). Also read `../../CLAUDE.md` (schema
+ graph density) and `../../scanners.md` (sources + focus filter).
Maintenance of existing nodes (mining, normalizing, linting) is the **kg-curator**
skill's job — this skill creates; that one tends.

## Triggers
"scan arxiv", "any new agent papers", "check arxiv", "run the arxiv scanner",
"census for <year>", "rank by citations", "pull citation counts".

## Selection criteria (adjusted 2026-06-21 — keep in sync with scanners.md)
- **Endpoint:** `https://export.arxiv.org/api/query` (follow http→https). Page at
  `max_results=200`, `sortBy=submittedDate`, dedup by version-stripped arXiv id.
- **Categories (9):** cs.AI, cs.CL, cs.LG, cs.MA + cs.SE, cs.RO, cs.HC, cs.IR, cs.DB.
  The last five were added to close a measured blind spot (coding, robotics,
  human-agent, retrieval/KG/semantic-layer, text-to-SQL/data agents). A paper counts
  if ANY listed category is in the set.
- **Terms (abstract OR-match):** `agentic OR "multi-agent" OR "tool use" OR
  "LLM agent" OR "language agent" OR "autonomous agent"`. `abs:` matches the
  abstract only, not full text.
- **Relevance score** (rank within month): high-signal terms ×3 (agentic, multi-agent,
  tool use/calling, MCP, orchestration, reasoning/planning agent, self-evolving,
  agent memory/safety/eval, RL…); title hits ×2; medium terms ×1 (benchmark, RAG,
  retrieval, workflow, verifier…); noise ×−2 (vision-only, speech, protein, GNN,
  diffusion-image, recommendation, federated, wireless, traffic, grid); cs.AI/cs.MA
  primary +1.

## Steps
1. **Query arXiv** with the criteria above. **Weekly sweep:** last ~7 days, newest
   first. **Census mode** ("census for <year/range>"): harvest month-by-month across
   the full range (run one month per shell call to stay under timeouts), dedup +
   score, and write a metadata census to `../../raw/arxiv/<year>-census/`
   (`census-<year>.jsonl` = all records; `INDEX.md` = ranked per month). The census is
   the exhaustive metadata layer; deep/full-text ingest and the browsable auto-note
   layer are separate, on-request steps (see below).
2. **Filter** to the agents-centric focus. Drop off-topic papers.
3. **Dedup** by arXiv id against existing files in `../../raw/arxiv/` and `../../index.md`.
4. **Capture (FULL TEXT, not just the abstract)** — raw must be the real source:
   - `../../raw/arxiv/<id>.md` = metadata (title, authors, id+URL, date, categories) + abstract.
   - `../../raw/arxiv/<id>.fulltext.md` = the FULL paper text. Fetch
     `https://arxiv.org/html/<id>` and strip tags; if that 404s or is thin,
     fall back to the PDF (`https://arxiv.org/pdf/<id>`) via `pdftotext`.
   raw is immutable once written.
5. **Ingest into the graph** (full rules in ../../CLAUDE.md "Entities & graph density").
   Read the FULL TEXT, then for each paper:
   - Write a source note in `../../wiki/sources/` ending with a `## Relationships` block.
   - **Promote node-worthy references to their own linked nodes** — models,
     benchmarks, methods, orgs, people. Before creating a node, check for an
     existing one or an alias (don't duplicate). Add reciprocal links on BOTH ends.
   - Update/create `../../wiki/concepts/` pages; link sibling concepts to each other.
   - Update `../../index.md` (grouped by type) and append to `../../log.md`.
6. **Integrity check.** Before finishing, verify no new orphans (every node has ≥1
   inbound and ≥1 outbound link) and no broken `[[links]]`; fix any. Log a one-line
   `lint` entry if you corrected anything.
7. **Report back** in chat — new papers, pages touched, top 3–5 signals — drawn from
   the `log.md` entry. No digest file; `index.md` + `log.md` are the record.

## Ingest tiers (census → browsable → deep)
A census produces three layers, each a deliberate trade of coverage vs depth:
1. **Census (metadata)** — every matching paper as a record in `raw/arxiv/<year>-census/`.
   Exhaustive, not in the graph.
2. **Browsable auto-notes** — abstract-only source notes in
   `wiki/sources/<year>-census/`, keyword-linked to concept/entity hubs, tagged
   `depth: abstract` + `auto-ingested`. Selection = top-N by score ∪ any focus slice
   (e.g. all knowledge-graph papers) ∪ per-domain cohorts. Kept OUT of the global
   graph view via the `.obsidian/graph.json` filter; reachable via local graphs.
3. **Deep notes** — full-text reads with analysis (`depth: full-text`), one per
   genuinely notable paper or survey; these are first-class graph nodes.
- When a census surfaces a recurring sub-theme or named system, **add a concept/entity
  hub** (frequency-justify it first) rather than just more leaves.

## Citation enrichment mode ("rank by citations", "pull citation counts")
arXiv gives no citation data; fetch it from **Semantic Scholar** to rank papers by
real impact (e.g. to choose which census papers deserve deep ingest).
1. **Batch lookup** (resumable): POST to
   `https://api.semanticscholar.org/graph/v1/paper/batch?fields=citationCount,influentialCitationCount,year`
   with up to 500 ids per call as `"ARXIV:<id>"` (version-stripped); back off on 429.
2. **Merge** `citationCount`, `influentialCitationCount`, and a computed
   `velocity` = citations ÷ months-since-publication into the census JSONL.
3. **Write** `raw/arxiv/<year>-census/CITATIONS.md` — top papers by raw citations,
   by influential citations, and by velocity, with **model/technical reports
   excluded** from the "agentic" lists.
4. **Caveats to state every time:** citation *lag* (recent papers undercounted —
   use velocity for a recency-fair view), model-report leakage, and extreme skew
   (median is tiny; the signal is in the head).

## Notes
- arXiv API is free, no key. Be polite: small page size, short sleeps between pages.
- Never invent findings — summarize only what the abstract/paper says; synthesis in
  nodes must be grounded in FULL TEXT, not abstracts (see STYLE.md).
- Stay drafts/notes only; this never emails or posts.
