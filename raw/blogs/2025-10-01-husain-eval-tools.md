---
source: hamel.dev
url: https://hamel.dev/blog/posts/eval-tools/
title: "Selecting The Right AI Evals Tool"
author: Hamel Husain
date: 2025-10-01
captured: 2026-06-22
note: Immutable raw capture. Verbatim full text from web_fetch (nav/boilerplate stripped). Companion to a course exercise where Langsmith, Braintrust, and Arize Phoenix completed the same homework assignment.
---

# Selecting The Right AI Evals Tool

An example of how to assess AI eval tools like Langsmith, Braintrust, and Arize Phoenix.

Over the past year, I've focused heavily on AI Evals, both in my consulting work and teaching. A question I get constantly is, "What's the best tool for evals?". I've always resisted answering directly for two reasons. First, people focus too much on tools instead of the process, thinking the tool will be an off-the-shelf solution when it rarely is. Second, the tools change so quickly that comparisons become outdated immediately.

Having used many of the popular eval tools, I can genuinely say that no single one is superior in every dimension. The "best" tool depends on your team's skillset, technical stack, and maturity.

Instead of a feature-by-feature comparison, it's more valuable to show *how* a panel of data scientists skilled in evals assesses these tools. As part of my AI Evals course, we had three of the most dominant vendors — Langsmith, Braintrust, and Arize Phoenix — complete the same homework assignment (a recipe-chatbot). Panelists: Shreya Shankar and Bryan Bischof (alongside Husain). Vendor reps: Harrison Chase (LangChain CEO) for Langsmith; Wayde Gilliam for Braintrust; SallyAnn DeLucia (Arize) for Phoenix.

## Criteria for Assessing AI Evals Tools

### 1. Workflow and Developer Experience
Reducing friction is more important than any single feature. Be mindful of the time it takes to go from observing a failure to iterating on a solution — e.g., going from viewing a single trace to experimenting with it in a playground. For teams with data-science backgrounds, a notebook-centric workflow is ideal (transparency and control). This is Husain's preferred workflow. Pay attention to SDK ergonomics, docs quality, and integration with existing data tools.

### 2. Human-in-the-Loop Support
The best tools don't try to automate away the human; they empower them. Since **error analysis is the highest ROI activity in AI engineering**, a tool's ability to support efficient human review is paramount. Prioritize tools with first-class support for manual annotation and error analysis. As of this writing, one thing missing from many tools is **axial coding**.

### 3. Transparency and Control vs. "Magic"
Be deeply skeptical of features that promise full automation without human validation — they create a powerful and dangerous illusion of confidence. Be wary of features where an AI agent both creates an evaluation rubric and then immediately scores the outputs. This "stacking of abstractions" hides flaws behind a high score. Favor tools that give control and visibility.

### 4. Ecosystem Integration vs. Walled Gardens
An eval tool should fit your stack, not force you to fit its stack. Beware proprietary DSLs (they add friction). The ability to export data into common formats for analysis in a variety of environments is a must-have.

### Conclusion
The right choice depends on your team's workflow, skillset, and needs. Husain personally uses these tools as a backend data store and uses Jupyter notebooks plus his own custom-built annotation interfaces for most needs.

## Appendix: Vendor Snapshots (Mid-2025)
**Langsmith** — intuitive workflow, smooth trace→playground transition, "Prompt Canvas," dedicated "Annotation Queue." Critiques: limited side-by-side comparison, cluttered UI, AI-generated examples risk homogeneous data.

**Braintrust** — clean UI, structured evals process, strong human-in-the-loop UIs, the "Money Table" (annotate traces with failure modes → sortable/quantifiable failure-mode view). Critiques: the "Loop" AI scorer (creates a rubric then immediately scores — false sense of security); proprietary query language (BTQL); clunky synthetic-data workflows.

**Arize Phoenix** — notebook-centric, export annotated data back to a Pandas DataFrame, open-source and local-first ("hackable"), one panelist's favorite OSS eval tool. Critiques: output-pane readability; wants aggregate visualizations (histograms) over point statistics; monolithic system-prompt editor (wants component-level ablation toggles).
