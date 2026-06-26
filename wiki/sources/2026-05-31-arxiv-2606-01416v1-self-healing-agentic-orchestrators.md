---
type: source
source_type: arxiv
title: "Self-Healing Agentic Orchestrators for Reliable Tool-Augmented Large Language Model Systems"
authors: Rahul Suresh Babu, Adarsh Agrawal
url: https://arxiv.org/abs/2606.01416v1
date: 2026-05-31
ingested: 2026-06-21
depth: full-text
tags: [multi-agent-systems, agent-security, tool-use, arxiv]
---

# Self-Healing Agentic Orchestrators for Reliable Tool-Augmented Large Language Model Systems

**Why it matters:** Treats agent reliability as a bounded runtime control problem — map failure signals to recovery actions under budgets, verify, log. 98.8% task success and verifier-guided runs cut silent failures to 0%.

## Takeaways
- [[self-healing-orchestrator|Self-healing orchestrator]] maps observable failure signals → inferred failure classes → targeted recovery under explicit budgets, then verifies recovered trajectories.
- 100-task fault-injection benchmark: 98.8% success vs 94.5% retry-only / 93.8% full-replanning; biggest gap at single-recovery budget (94.0% vs 85.3%/88.2%).
- Verifier-guided self-healing drives silent failures to 0.0%; validated with a live tool-calling model in the loop.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Entities:** [[self-healing-orchestrator]]
- **Raw:** `raw/arxiv/2606.01416v1.md` · `raw/arxiv/2606.01416v1.fulltext.md`
