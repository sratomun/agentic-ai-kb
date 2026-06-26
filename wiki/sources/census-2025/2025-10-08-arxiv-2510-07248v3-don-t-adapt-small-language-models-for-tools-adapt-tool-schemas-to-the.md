---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Don't Adapt Small Language Models for Tools; Adapt Tool Schemas to the Models"
authors: Jonggeun Lee et al.
url: https://arxiv.org/abs/2510.07248v3
date: 2025-10-08
score: 12
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, tool-use, multi-agent-systems]
---

# Don't Adapt Small Language Models for Tools; Adapt Tool Schemas to the Models

**arXiv:** [2510.07248v3](https://arxiv.org/abs/2510.07248v3) · 2025-10-08 · cs.CL
**Authors:** Jonggeun Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Small language models (SLMs) enable scalable tool-augmented multi-agent systems where multiple SLMs handle subtasks orchestrated by a powerful coordinator. However, they struggle with tool-use tasks, particularly in selecting appropriate tools and identifying correct parameters. A common failure mode is \textit{schema misalignment}: models hallucinate plausible tool names that are absent from the provided tool schema, due to different naming conventions internalized during pretraining. Rather than training models to adapt to unfamiliar schemas, we propose adapting schemas to align with models' pretrained knowledge. We introduce \textbf{PA-Tool} (Pretraining-Aligned Tool Schema Generation), a training-free method that leverages peakedness, a signal used in contamination detection that indicates pretraining familiarity, to rename tool components. By generating multiple candidates and selecting the candidate with the highest peakedness, PA-Tool identifies pretraining-aligned naming patterns. Experiments on MetaTool and RoTBench show improvements of up to 17\%, with schema misalignment errors reduced by 80\%. PA-Tool enables small models to substantially improve tool-use accuracy without retraining, showing that schema-level interventions can unlock the tool-use potential of resource-efficient models. Our code is available at https://github.com/holi-lab/PA-Tool.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[multi-agent-systems]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2510.07248v3)
