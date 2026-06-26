---
type: entity
entity_type: method
aliases: [Judge Agent Forest]
tags: [agents, method, llm-as-judge, evaluation]
created: 2026-06-22
updated: 2026-06-22
---

# JAF (Judge Agent Forest)

*Judge Agent Forest — a robust LLM-as-judge method using cohort-level belief propagation and consistency scoring.*

## What it is
JAF (Judge Agent Forest) is an evaluation method where a judge LLM scores each response alongside a random subset of related peers, inducing a cohort knowledge graph and ensemble scoring. It ships a consistency metric (empirical acceptance probability) and beats isolated-judge approaches on 315 triage assets.

## Why it matters
LLM-as-judge is now the de-facto scalable eval approach, but position bias and inconsistency make it unreliable at scale. JAF's cohort-aware ensembling and consistency metric are the most practical fixes available for production eval pipelines.

## Relationships
- addresses [[llm-as-judge]]
- part of [[agent-evaluation]]
- relates to [[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]]

## Cited by
- [[2026-01-29-arxiv-2601-22269v1-jaf-judge-agent-forest]]
