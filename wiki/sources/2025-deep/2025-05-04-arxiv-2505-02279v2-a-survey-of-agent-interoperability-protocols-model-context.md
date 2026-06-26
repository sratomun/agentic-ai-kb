---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A survey of agent interoperability protocols: Model Context Protocol (MCP), Agent Communication Protocol (ACP), Agent-to-Agent Protocol (A2A), and Agent Network Protocol (ANP)"
authors: Abul Ehtesham, Aditi Singh, Gaurav Kumar Gupta, Saket Kumar
url: https://arxiv.org/abs/2505.02279v2
date: 2025-05-04
citationCount: 116
influentialCitationCount: 11
velocity: 8.53
ingested: 2026-06-22
tags: [agent-economies, agent-security, agent-protocols, tool-use, multi-agent-systems, arxiv, 2025, cited]
---

# A survey of agent interoperability protocols: Model Context Protocol (MCP), Agent Communication Protocol (ACP), Agent-to-Agent Protocol (A2A), and Agent Network Protocol (ANP)

**arXiv [2505.02279v2](https://arxiv.org/abs/2505.02279v2)** · 2025-05-04 · **116 citations** (11 influential · 8.53/mo) · Abul Ehtesham, Aditi Singh, Gaurav Kumar Gupta, Saket Kumar

## Abstract
Large language model powered autonomous agents demand robust, standardized protocols to integrate tools, share contextual data, and coordinate tasks across heterogeneous systems. Ad-hoc integrations are difficult to scale, secure, and generalize across domains. This survey examines four emerging agent communication protocols: Model Context Protocol (MCP), Agent Communication Protocol (ACP), Agent-to-Agent Protocol (A2A), and Agent Network Protocol (ANP), each addressing interoperability in deployment contexts. MCP provides a JSON-RPC client-server interface for secure tool invocation and typed data exchange. ACP defines a general-purpose communication protocol over RESTful HTTP, supporting MIME-typed multipart messages and synchronous and asynchronous interactions. Its lightweight and runtime-independent design enables scalable agent invocation, while features like session management, message routing, and integration with role-based and decentralized identifiers (DIDs). A2A enables peer-to-peer task delegation using capability-based Agent Cards, supporting secure and scalable collaboration across enterprise agent workflows. ANP supports open network agent discovery and secure collaboration using W3C decentralized identifiers DIDs and JSON-LD graphs. The protocols are compared across multiple dimensions, including interaction modes, discovery mechanisms, communication patterns, and security models. Based on the comparative analysis, a phased adoption roadmap is proposed: beginning with MCP for tool access, followed by ACP for structured, multimodal messaging session-aware interaction and both online and offline agent discovery across scalable, HTTP-based deployments A2A for collaborative task execution, and extending to ANP for decentralized agent marketplaces. This work provides a comprehensive foundation for designing secure, interoperable, and scalable ecosystems of LLM-powered agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Challenges and Solutions in Agent Protocol Interoperability 3 Background and Related Work 3.1 AI Agents: Definition and Scope 3.2 Early Symbolic Agent Languages—Evolution of Agent Communication Standards 3.3 Service-Oriented Integrations and Retrieval-Augmented Generation 3.4 LLM Agents and Function Calling 3.5 Orchestration and Lightweight Agent Frameworks 3.6 Protocol Evolution Timeline 4 MCP 4.1 Client Application (Host) 4.2 MCP Server (Providing Context Capabilities) 4.3 Core Components 4.4 MCP Server Core Capabilities 4.5 MCP Connection Lifecycle 4.6 Security Challenges and Mitigations Across the MCP Lifecycle 5 A2A Architecture 5.1 Core Components 5.1.1 User 5.1.2 Client Agent 5.1.3 Remote Agent (Server) 5.2 A2A Main Components 5.3 A2A Transport Layer and Communication 5.4 A2A Remote Agent (Server) Lifecycle 5.5 Security Challenges and Mitigations Across the A2A Lifecycle 6 ACP Architecture 6.1 ACP Main Components 6.2 ACP Agent Lifecycle 6.3 Security Considerations Across the ACP Lifecycle…

**Method / approach.** method calls and notifications in accordance with the negotiated capabilities. Both parties are expected to adhere strictly to the features agreed upon during initialization, ensuring compatibility and predictability. Each task invocation may include a configurable timeout, and if a response is not received within that window, the client may issue a cancellation notification to prevent resource exhaustion or stale execution threads. Shutdown ensures a clean and predictable end to the session. Either party may initiate termination by closing the transport layer typically HTTP or stdio which signals the end of communication. Upon shutdown, both client and server are responsible for resource cleanup, including the removal of active timeouts, cancellation of subscriptions, and deallocation of any spawned child processes. After this point, no new protocol messages should be sent, with the exception of essential diagnostics like ping or log flush events. 4.6 Security Challenges and Mi…

**Results.** evaluation. Section 9 outlines the phased adoption roadmap. Section 10 concludes and suggests future research directions. 2 Challenges and Solutions in Agent Protocol Interoperability Despite the emergence of multiple open protocols like MCP, ACP, A2A, and ANP, achieving seamless agent interoperability in real-world AI systems remains a non-trivial task. This section identifies key challenges encountered in agent-based architectures and highlights how each protocol addresses them with purpose-built design principles. Lack of Context Standardization for LLMs: Large Language Models (LLMs) require contextual grounding to produce accurate outputs. However, existing application architectures provide no unified mechanism to deliver structured context to LLMs, leading to ad hoc tool integrations and unreliable behavior. Solution: The Model Context Protocol (MCP) addresses this by standardizing how applications deliver tools, datase…

**Conclusion.** Conclusion A Survey of Agent Interoperability Protocols: Model Context Protocol (MCP), Agent Communication Protocol (ACP), Agent-to-Agent Protocol (A2A), and Agent Network Protocol (ANP) Abul Ehtesham Kent State University Kent, OH, USA aehtesha@kent.edu \And Aditi Singh Cleveland State University Cleveland, OH, USA a.singh22@csuohio.edu \And Gaurav Kumar Gupta Youngstown State University Youngstown, OH, USA gkgupta@student.ysu.edu \And Saket Kumar Northeastern University Boston, MA, USA kumar.sak@northeastern.edu Abstract Large language model (LLM)-powered autonomous agents demand robust, standardized protocols to integrate tools, share contextual data, and coordinate tasks across heterogeneous system…

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Raw:** `raw/arxiv/2505.02279v2.md` · `raw/arxiv/2505.02279v2.fulltext.md`
