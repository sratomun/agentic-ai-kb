---
type: concept
tags: [agents, healthcare, clinical, medicine]
created: 2026-06-21
updated: 2026-06-22
census_count: 1065
kind: domain
---

# Clinical & healthcare agents

*Agents applied to medicine — clinical decision support, diagnosis, triage, and workflow automation. One of the largest application clusters in the corpus.*

## What it is
LLM/multimodal agents that plan, use tools, and reason over clinical data: EHR analysis, differential diagnosis, medical imaging interpretation, and evidence-gathering workflows — usually multi-agent and retrieval-augmented, with a growing emphasis on *traceable, verifiable* reasoning.

## Why it matters
Huge volume, high stakes, and heavily gated by safety and regulation — this is exactly where [[agent-security]], [[agent-reliability]], and the [[governance-gap]] bite hardest. It's the clearest preview of what "agents under regulation" looks like in practice, and the patterns that earn trust here (step-level verification, citation, quantitative grounding) transfer to any high-stakes enterprise domain.

## What the evidence shows
**2025 foundations.** The leading clinical agents all converged on the same answer to the trust problem: **make the reasoning auditable**. **DeepRare** (rare-disease diagnosis) pairs traceable reasoning with real gene-testing data and beats the next-best method by ~23 points (→ [[2025-06-25-arxiv-2506-20430v3-an-agentic-system-for-rare-disease-diagnosis-with]]). **MedRAX** integrates SOTA chest-X-ray analysis tools with MLLMs into one agent and ships **ChestAgentBench** (2,500 complex queries, 7 categories), reaching SOTA on CXR interpretation (→ [[2025-02-04-arxiv-2502-02673v2-medrax-medical-reasoning-agent-for-chest-x-ray]]). **MedAgent-Pro** pushes evidence-based diagnosis by integrating quantitative visual tools and verifying *each reasoning step* — the explicit antidote to "confident direct answers" (→ [[2025-03-21-arxiv-2503-18968v3-medagent-pro-towards-evidence-based-multi-modal-medical]]).
- The through-line: in medicine, an agent that can't show its work is unusable — verification and citation are first-class, not afterthoughts.

## Relationships
- governed by [[agent-security]], [[governance-gap]], [[agent-reliability]]
- uses [[multi-agent-systems]], [[agentic-rag]]
- a form of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **58** · [[2025-06-25-arxiv-2506-20430v3-an-agentic-system-for-rare-disease-diagnosis-with|An Agentic System for Rare Disease Diagnosis with Traceable Reasoning]]
- **58** · [[2025-02-04-arxiv-2502-02673v2-medrax-medical-reasoning-agent-for-chest-x-ray|MedRAX: Medical Reasoning Agent for Chest X-ray]]
- **55** · [[2025-03-21-arxiv-2503-18968v3-medagent-pro-towards-evidence-based-multi-modal-medical|MedAgent-Pro: Towards Evidence-based Multi-modal Medical Diagnosis via Reasonin...]]
