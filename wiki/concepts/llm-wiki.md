---
type: concept
tags: [agents, knowledge, methodology, markdown]
created: 2026-06-22
updated: 2026-06-22
kind: methodology
---

# LLM wiki (the knowledge-as-markdown pattern)

*Curated knowledge kept as a directory of cross-linked Markdown files that agents read, update, and compound over time — the pattern this entire radar is built on.*

## What it is
A way of giving agents durable, shared context: a version-controlled library of markdown notes with YAML frontmatter, interlinked into a graph, plus convention files (`index.md`, `log.md`, `AGENTS.md`/`CLAUDE.md`) that tell agents how to navigate and behave. Popularized by Andrej Karpathy's "LLM wiki" gist and the convergent `AGENTS.md`/`CLAUDE.md` practice across tens of thousands of repos. Now standardized as [[open-knowledge-format|OKF]].

## Why it matters
Karpathy's insight is the load-bearing one: "LLMs don't get bored, don't forget to update a cross-reference, and can touch 15 files in one pass" — the bookkeeping that makes humans abandon personal wikis is exactly what agents are good at. That's *why* this radar works as a self-maintaining graph rather than a pile of documents, and why it compounds. It's also the substrate that makes the radar portable: because it's just markdown + frontmatter + links, it converts cleanly to [[open-knowledge-format|OKF]] and is consumable by any agent that speaks it.

## What the evidence shows
- The pattern emerged organically across three lineages — Karpathy's LLM-wiki gist, the `AGENTS.md`/`CLAUDE.md` convention family, and Obsidian vaults wired to coding agents — then converged.
- Its weakness was that every instance was bespoke (no agreed fields or filenames); [[open-knowledge-format|OKF]] (Jun 2026) fixes that by specifying the minimal interoperability surface.
- It is deliberately the *lowest-friction* substrate that already exists (Markdown + YAML + Git), not a new one — readable with `cat`, diffable in version control, parseable without an SDK.

## Relationships
- championed by [[andrej-karpathy]] → [[2026-04-30-blog-karpathy-sequoia-ascent-2026]]
- standardized by [[open-knowledge-format]]
- pairs with [[mcp]] (knowledge vs tool access)
- the method behind [[knowledge-graph]] in this vault
- serves [[agent-memory]] (durable shared context) and [[agentic-ai]]

## Key references
- [[2026-06-12-okf-introducing-open-knowledge-format]]
- [[2026-04-karpathy-llm-wiki-gist]]
