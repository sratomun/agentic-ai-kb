---
type: source
source_type: arxiv
title: "Insight Agents: An LLM-Based Multi-Agent System for Data Insights"
authors: Jincheng Bai, Zhenyu Zhang, Jennifer Zhang, Zhihuai Zhu (Amazon)
url: https://arxiv.org/abs/2601.20048v2
date: 2026-01-27
ingested: 2026-06-22
depth: full-text
venue: SIGIR '25
tags: [agent-evaluation, data-analysis-agents, multi-agent-systems, arxiv]
---

# Insight Agents: An LLM-Based Multi-Agent System for Data Insights

**Why it matters:** A shipped production data-insight agent (live for US Amazon sellers) that spells out exactly how to score an analyst agent: decompose answer quality into **relevance, correctness, completeness**, gate on all three, and hold it against a **tail-latency budget**. Concrete evidence that insight eval is multi-axis quality + latency, not one score.

## What it is
A hierarchical plan-and-execute multi-agent system: a manager agent (Out-of-Domain detection + BERT-based routing + query augmentation) over two workers — data presenter and insight generator. Built on RAG over tabular seller data via internal **APIs** (deliberately chosen over text-to-SQL for higher accuracy and fewer column hallucinations). LLM is Claude-3-Sonnet via Bedrock.

## Metrics (how they actually measure it)
- **Component models:** OOD detection (precision/recall/runtime), agent routing (accuracy/runtime).
- **End-to-end answer quality (human auditors, 3 dimensions):**
  - **Relevance** = key points addressed / key points in question.
  - **Correctness** = correct insights / total insights in response (precision-like).
  - **Completeness** = required insights present / total required (recall-like).
  - **Question-level accuracy** = % of questions where all three exceed 0.8.

## Results (verified)
- OOD: auto-encoder precision **0.969**, recall 0.721 at 0.009s — vs LLM few-shot 0.616/0.971 at 1.665s.
- Routing: fine-tuned BERT (33M) **0.83** accuracy at 0.31s — vs LLM few-shot 0.60 at 2.14s.
- End-to-end (100-question benchmark, 57 in-scope): Relevancy **0.977**, Correctness **0.958**, Completeness **0.993**; **question-level accuracy 89.5%** (51/57); **P90 latency 13.56s**. (The abstract rounds these to "90%" and "below 15s.")

## So what
For analyst/insight agents, "good" = correctness *and* completeness *and* relevance, each thresholded, plus tail latency under real traffic. Specialized lightweight models (OOD, routing) buy latency vs. all-LLM pipelines. Human eval remains the accuracy backstop where ground truth is fuzzy.

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[data-analysis-agents|Data-analysis agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[insight-agents]]
- **Raw:** alphaXiv full-text (id 2601.20048v2)

## Relationships
- evaluates [[data-analysis-agents]]
- relates to [[agent-evaluation]]
