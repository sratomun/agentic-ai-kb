---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "{{Paper title}}"
authors: {{First Author et al.}}
url: https://arxiv.org/abs/{{id}}
date: {{YYYY-MM-DD}}
score: {{relevance-score}}
primary: {{primary-arxiv-category}}
tags: [arxiv, auto-ingested, {{concept-tags}}]
---

# {{Paper title}}

**arXiv:** [{{id}}](https://arxiv.org/abs/{{id}}) · {{date}} · {{primary}}
**Authors:** {{authors}}

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
{{verbatim abstract}}

## Graph
- **Concepts:** [[{{concept-slug}}|{{Display}}]] · …
- **Entities:** [[{{entity-slug}}]] · …  (omit line if none)
- **Census record:** `raw/arxiv/{{year}}-census/census-{{year}}.jsonl` (id {{id}})
