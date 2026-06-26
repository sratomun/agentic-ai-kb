---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentAuditor: Human-Level Safety and Security Evaluation for LLM Agents"
authors: Hanjun Luo, Shenyu Dai, Chiming Ni, Xinfeng Li et al.
url: https://arxiv.org/abs/2506.00641v3
date: 2025-05-31
citationCount: 56
influentialCitationCount: 7
velocity: 4.4
ingested: 2026-06-22
tags: [agent-reliability, agent-security, agentic-rag, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# AgentAuditor: Human-Level Safety and Security Evaluation for LLM Agents

**arXiv [2506.00641v3](https://arxiv.org/abs/2506.00641v3)** · 2025-05-31 · **56 citations** (7 influential · 4.4/mo) · Hanjun Luo, Shenyu Dai, Chiming Ni, Xinfeng Li et al.

## Abstract
Despite the rapid advancement of LLM-based agents, the reliable evaluation of their safety and security remains a significant challenge. Existing rule-based or LLM-based evaluators often miss dangers in agents' step-by-step actions, overlook subtle meanings, fail to see how small issues compound, and get confused by unclear safety or security rules. To overcome this evaluation crisis, we introduce AgentAuditor, a universal, training-free, memory-augmented reasoning framework that empowers LLM evaluators to emulate human expert evaluators. AgentAuditor constructs an experiential memory by having an LLM adaptively extract structured semantic features (e.g., scenario, risk, behavior) and generate associated chain-of-thought reasoning traces for past interactions. A multi-stage, context-aware retrieval-augmented generation process then dynamically retrieves the most relevant reasoning experiences to guide the LLM evaluator's assessment of new cases. Moreover, we developed ASSEBench, the first benchmark designed to check how well LLM-based evaluators can spot both safety risks and security threats. ASSEBench comprises 2293 meticulously annotated interaction records, covering 15 risk types across 29 application scenarios. A key feature of ASSEBench is its nuanced approach to ambiguous risk situations, employing "Strict" and "Lenient" judgment standards. Experiments demonstrate that AgentAuditor not only consistently improves the evaluation performance of LLMs across all benchmarks but also sets a new state-of-the-art in LLM-as-a-judge for agent safety and security, achieving human-level accuracy. Our work is openly accessible at https://github.com/Astarojth/AgentAuditor.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large language model (LLM)-based agents are rapidly evolving from passive text generators into autonomous decision-makers capable of complex, goal-driven behaviors [48]. By leveraging the general reasoning abilities of LLMs and extending them with tool use and real-time environment interaction, these agents are moving closer to the vision of artificial general intelligence (AGI) [49, 58, 9, 95, 91, 1, 88]. However, this expanded agency introduces a new class of risks: agents may exhibit unsafe or insecure behaviors during autonomous interactions, especially in high-stakes or dynamic scenarios [29, 13, 89, 45, 44]. Traditional LLM safety evaluation focuses mainly on the generated content [104, 99, 43, 18, 62, 80], but agentic systems require a much deeper assessment of their interactive behaviors and decision-making processes. Reliable evaluation of these dynamic ∗ † Co-first Author Corresponding Author (lxfmakeit@gmail.com) 39th Conference on Neural Information Processing Systems (NeurIPS 2025). behaviors is essential for building trustworthy LLM agents, yet current…

**Method / approach.** methodologies struggle to keep pace with the complexity and diversity of real-world agent risks [90, 50]. Several benchmarks have been proposed to evaluate the safety or security of LLM agents, such as ToolEmu [71], AgentSafetyBench [98], and AgentSecurityBench [97]. While these benchmarks simulate various threats, they are largely limited to test LLM standalone risk management abilities. Similar to LLM safety benchmark [26, 78, 99, 18, 57, 62], most LLM-based agent benchmarks also rely on automated evaluation methods: 1. Rule-based Evaluators, which use predefined rules or patterns, and 2. LLM-based Evaluators, which leverage the semantic understanding of LLMs (see Section 2 for details). While rule-based evaluators are interpretable and efficient, they lack flexibility and struggle with implicit or novel risks. LLM-based evaluators, on the other hand, can capture more complex semantics but often suffer from inconsistency, bias, and limited interpretability. Both approaches face sign…

**Results.** Experiments demonstrate that AgentAuditor not only consistently improves the evaluation performance of LLMs across all benchmarks but also sets a new state-of-the-art in LLM-as-a-judge for agent safety and security, achieving human-level accuracy. Our work is openly accessible at https://github.com/Astarojth/AgentAuditor-ASSEBench. 1 Introduction Large language model (LLM)-based agents are rapidly evolving from passive text generators into autonomous decision-makers capable of complex, goal-driven behaviors [48]. By leveraging the general reasoning abilities of LLMs and extending them with tool use and real-time environment interaction, these agents are moving closer to the vision of artificial general intelligence (AGI) [49, 58, 9, 95, 91, 1, 88]. However, this expanded agency introduces a new class of risks: agents may exhibit unsafe or insecure behaviors during autonomous interactions, especially in high-stakes or dynamic scenario…

**Conclusion.** conclusions, and represent valuable ’meta-cognitive’ experiences. Finally, the reasoning memory RM is presented as follows: RM = {rmj }K j=1 , rmj = {idj , M sj , M vj , CoTj }, 3.3 (5) Stage 3: RAG-based Memory Augmented Reasoning Following the construction of the F M and RM , we employ memory-augmented reasoning, an approach based on the principles of RAG. When a target shot M si from F M is presented for evaluation, AgentAuditor utilizes a multi-stage retrieval strategy to identify the k most relevant entries from RM . First, with a Top-n strategy, a set of n most similar shots Mn (i) is retrieved by computing the cosine similarity between the content embedding eci of the target shot and the content embeddings ecj of all shots in RM .…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2506.00641v3.md` · `raw/arxiv/2506.00641v3.fulltext.md`
