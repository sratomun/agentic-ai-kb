---
type: source
source_type: arxiv
title: "Agentic Witnessing: Pragmatic and Scalable TEE-Enabled Privacy-Preserving Auditing"
authors: Antony Rowstron
url: https://arxiv.org/abs/2604.24203v1
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CR
tags: [human-agent-interaction, agent-protocols, governance-gap, arxiv, auto-ingested]
---

# Agentic Witnessing: Pragmatic and Scalable TEE-Enabled Privacy-Preserving Auditing

**arXiv:** [2604.24203v1](https://arxiv.org/abs/2604.24203v1) · 2026-04-27 · cs.CR
**Authors:** Antony Rowstron

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Auditing the semantic properties of proprietary data creates a fundamental tension: verification requires transparent access, while proprietary rights demand confidentiality. While Zero-Knowledge Proofs (ZKPs) ensure privacy, they are typically limited to precise algebraic constraints and are ill-suited for verifying qualitative, unstructured properties, such as the logic within a codebase. We propose {\em Agentic Witnessing}, a framework that moves verification from attested execution to {\em attested reasoning}. The system is composed of three agents: a Verifier (who wants to check properties of a dataset), a Prover (who owns the dataset) and an Auditor (that inspects the dataset). The Verifier is allowed to ask a limited number of simple binary true/false questions to the auditor. By isolating an LLM-based Auditor within a Trusted Execution Environment (TEE), the system enables the Verifier to query a Prover's private data via simple Boolean queries, without exposing the raw dataset. The Auditor uses the Model Context Protocol (MCP) to dynamically inspect the target dataset, producing a yes/no verdict accompanied by a cryptographic transcript: a signed hash chain binding the reasoning trace to both the original dataset and the TEE's hardware root of trust. We demonstrate this architecture by automating the artifact evaluation process for 21 peer-reviewed computer science papers with released codebases on GitHub (e.g. Does the codebase implement the system described in the paper?). We verified five high-level properties of these codebases described in the corresponding publications, treating the source code as private. Our results show that TEE-enabled agentic auditing provides a mechanism for privacy-preserving oversight, effectively decoupling qualitative verification from the need for data disclosure.

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-protocols|Agent protocols]] · [[governance-gap|Governance gap]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.24203v1)
