---
type: source
source_type: arxiv
title: "GLANCE: A Global-Local Coordination Multi-Agent Framework for Music-Grounded Non-Linear Video Editing"
authors: Zihao Lin, Haibo Wang, Zhiyang Xu, Siyao Dai et al.
url: https://arxiv.org/abs/2604.05076v1
date: 2026-04-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.MA
tags: [agent-economies, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# GLANCE: A Global-Local Coordination Multi-Agent Framework for Music-Grounded Non-Linear Video Editing

**arXiv:** [2604.05076v1](https://arxiv.org/abs/2604.05076v1) · 2026-04-06 · cs.MA
**Authors:** Zihao Lin, Haibo Wang, Zhiyang Xu, Siyao Dai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Music-grounded mashup video creation is a challenging form of video non-linear editing, where a system must compose a coherent timeline from large collections of source videos while aligning with music rhythm, user intent, story completeness, and long-range structural constraints. Existing approaches typically rely on fixed pipelines or simplified retrieval-and-concatenation paradigms, limiting their ability to adapt to diverse prompts and heterogeneous source materials. In this paper, we present GLANCE, a global-local coordination multi-agent framework for music-grounded nonlinear video editing. GLANCE adopts a bi-loop architecture for better editing practice: an outer loop performs long-horizon planning and task-graph construction, and an inner loop adopts the "Observe-Think-Act-Verify" flow for segment-wise editing tasks and their refinements. To address the cross-segment and global conflict emerging after subtimelines composition, we introduce a dedicated global-local coordination mechanism with both preventive and corrective components, which includes a novelly designed context controller, conflict region decomposition module, and a bottom-up dynamic negotiation mechanism. To support rigorous evaluation, we construct MVEBench, a new benchmark that factorizes editing difficulty along task type, prompt specificity, and music length, and propose an agent-as-a-judge evaluation framework for scalable multi-dimensional assessment. Experimental results show that GLANCE consistently outperforms prior research baselines and open-source product baselines under the same backbone models. With GPT-4o-mini as the backbone, GLANCE improves over the strongest baseline by 33.2% and 15.6% on two task settings, respectively. Human evaluation further confirms the quality of the generated videos and validates the effectiveness of the proposed evaluation framework.

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05076v1)
