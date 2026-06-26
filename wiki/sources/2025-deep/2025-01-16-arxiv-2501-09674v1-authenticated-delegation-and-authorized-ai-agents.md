---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Authenticated Delegation and Authorized AI Agents"
authors: Tobin South, Samuele Marro, Thomas Hardjono, Robert Mahari et al.
url: https://arxiv.org/abs/2501.09674v1
date: 2025-01-16
citationCount: 50
influentialCitationCount: 11
velocity: 2.92
ingested: 2026-06-22
tags: [agent-security, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# Authenticated Delegation and Authorized AI Agents

**arXiv [2501.09674v1](https://arxiv.org/abs/2501.09674v1)** · 2025-01-16 · **50 citations** (11 influential · 2.92/mo) · Tobin South, Samuele Marro, Thomas Hardjono, Robert Mahari et al.

## Abstract
The rapid deployment of autonomous AI agents creates urgent challenges around authorization, accountability, and access control in digital spaces. New standards are needed to know whom AI agents act on behalf of and guide their use appropriately, protecting online spaces while unlocking the value of task delegation to autonomous agents. We introduce a novel framework for authenticated, authorized, and auditable delegation of authority to AI agents, where human users can securely delegate and restrict the permissions and scope of agents while maintaining clear chains of accountability. This framework builds on existing identification and access management protocols, extending OAuth 2.0 and OpenID Connect with agent-specific credentials and metadata, maintaining compatibility with established authentication and web infrastructure. Further, we propose a framework for translating flexible, natural language permissions into auditable access control configurations, enabling robust scoping of AI agent capabilities across diverse interaction modalities. Taken together, this practical approach facilitates immediate deployment of AI agents while addressing key security and accountability concerns, working toward ensuring agentic AI systems perform only appropriate actions and providing a tool for digital service providers to enable AI agent interactions without risking harm from scalable interaction.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Why authenticated delegation is important 2.1 Functions of authenticated delegation 2.1.1 Current challenges in delegating authority to AI agents 2.1.2 Communicating limitations and restricting scope 2.1.3 Verification in multi-agent communication 2.1.4 Protecting human spaces online 2.1.5 Supporting contextual integrity 2.2 Background Comparisons to other AI identifiers Comparisons to Model Context Protocol and GPT Actions Documentation, safety, and governance of agentic AI systems How authenticated delegation combines these solutions 3 Extending OpenID Connect for identifying and authenticating AI agents 3.1 OAuth2.0 and OpenID-Connect 3.2 Delegation of authority from the user to the AI agent 3.3 Token-based authentication framework 3.4 Scope Limitations on Delegation 3.5 Using verifiable credentials as an alternative 4 Defining scope and permissions for AI agents 4.1 Structured permission languages 4.2 Authentication flows 4.3 Natural Language Mechanisms 4.4 Combining structured permissions, natural langu…

**Method / approach.** method for expressing flexible, natural language permissions for agents and transforming them into auditable, fine-grained access control rules, that can operate across agent modalities (e.g., web requests, computer use, or language interfaces), Further, this work provides example use cases of the framework in Appendix C and a legal analysis of the implications of this work in subsection 5.5 . Figure 1: Conceptual overview of a verifiable delegation credential for AI agents. Users issue delegation credentials that include: the AI system’s unique identity and properties, delegated permissions with contextual scope restrictions, user metadata, and cryptographic signatures for verifiability. These credentials enable secure, trustworthy interactions between AI agents and third-party services, ensuring traceability and appropriate delegation of authority. 2 Why authenticated delegation is important Authenticated delegation is the process of instructing an AI system to perform a t…

**Results.** evaluation of robustness of LLM translation into structured languages, we leave these specifics to future work. Ultimately, focusing on structured, unambiguous resource constraints is the most reliable way to ensure that an AI agent remains within authorized bounds in a given environment. While there is still room for higher-level (often natural language) task constraints, one should treat these as guidance towards the primary enforcement mechanism. Indeed, while natural language can adequately address the extremely large possible space of agent actions, its transformation into access controls grounds the limitations on agent actions into finite auditable controls. Structured resource scoping reduces the reliance on model alignment alone, decreases the risk of adversarial prompt injections, and simplifies the integration with well-established security mechanisms. Combining this approach with well-designed authentication flows and hel…

**Conclusion.** Conclusion 7 Acknowledgements A Technical Details A.1 Federated OpenID Providers for Agent Mutual Authentication A.2 Identification of AI Systems and AI Agents A.3 ID token threat model B Alternatives in Access Control Management B.1 Schema Validation As Scoping B.2 Controlled Natural Languages C Example Use Cases C.1 AI Agent for Web Browsing Scenario. Approach. Why It Matters. C.2 API-Only Data Manager Scenario. Approach. Why It Matters. C.3 Remote Virtual Environment via SSH Scenario. Approach. Why It Matters. C.4 Agent-to-Agent Collaboration Scenario. Approach. Why It Matters. Authenticated Delegation and Authorized AI Agents Tobin South Samuele Marro Thomas…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2501.09674v1.md` · `raw/arxiv/2501.09674v1.fulltext.md`
