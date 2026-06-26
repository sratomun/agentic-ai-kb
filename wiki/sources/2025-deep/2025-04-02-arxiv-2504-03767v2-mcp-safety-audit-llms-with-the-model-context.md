---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits"
authors: Brandon Radosevich, John Halloran
url: https://arxiv.org/abs/2504.03767v2
date: 2025-04-02
citationCount: 77
influentialCitationCount: 12
velocity: 5.26
ingested: 2026-06-22
tags: [agent-security, agent-protocols, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits

**arXiv [2504.03767v2](https://arxiv.org/abs/2504.03767v2)** · 2025-04-02 · **77 citations** (12 influential · 5.26/mo) · Brandon Radosevich, John Halloran

## Abstract
To reduce development overhead and enable seamless integration between potential components comprising any given generative AI application, the Model Context Protocol (MCP) (Anthropic, 2024) has recently been released and subsequently widely adopted. The MCP is an open protocol that standardizes API calls to large language models (LLMs), data sources, and agentic tools. By connecting multiple MCP servers, each defined with a set of tools, resources, and prompts, users are able to define automated workflows fully driven by LLMs. However, we show that the current MCP design carries a wide range of security risks for end users. In particular, we demonstrate that industry-leading LLMs may be coerced into using MCP tools to compromise an AI developer's system through various attacks, such as malicious code execution, remote access control, and credential theft. To proactively mitigate these and related attacks, we introduce a safety auditing tool, MCPSafetyScanner, the first agentic tool to assess the security of an arbitrary MCP server. MCPScanner uses several agents to (a) automatically determine adversarial samples given an MCP server's tools and resources; (b) search for related vulnerabilities and remediations based on those samples; and (c) generate a security report detailing all findings. Our work highlights serious security issues with general-purpose agentic workflows while also providing a proactive tool to audit MCP server safety and address detected vulnerabilities before deployment. The described MCP server auditing tool, MCPSafetyScanner, is freely available at: https://github.com/johnhalloran321/mcpSafetyScanner

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background 2.1 Need for Standardized Generative AI APIs 2.2 The Model Context Protocol 3 The MCP Allows LLMs to Compromise User Systems 4 Retrieval-Agent Deception Attacks 5 McpSafetyScanner - Multi-Agentic Framework for Proactive MCP Vulnerability Detection and Remediation 6 Discussion, Conclusions, and Future Work 7 Experimental Setup 8 Acknowledgements A MCP Claude Desktop Config File B Claude Attack Examples C Llama-3.3-70B-Instruct Attack Examples D Llama-3.3-70B-Instruct refusals involve explicit harmful/unsafe keywords E McpSafetyScanner determines MCP server vulnerabilities, provides remediations MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits Brandon Radosevich John T. Halloran ∗ Leidos halloranjt@leidos.com Equal Contribution Abstract To reduce development overhead and enable seamless integration between potential components comprising any given generative AI application, the Model Context Protocol (MCP) (Anthropic, 2025d ) has recently been released and, subsequently, wid…

**Method / approach.** Framework for Proactive MCP Vulnerability Detection and Remediation 6 Discussion, Conclusions, and Future Work 7 Experimental Setup 8 Acknowledgements A MCP Claude Desktop Config File B Claude Attack Examples C Llama-3.3-70B-Instruct Attack Examples D Llama-3.3-70B-Instruct refusals involve explicit harmful/unsafe keywords E McpSafetyScanner determines MCP server vulnerabilities, provides remediations MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits Brandon Radosevich John T. Halloran ∗ Leidos halloranjt@leidos.com Equal Contribution Abstract To reduce development overhead and enable seamless integration between potential components comprising any given generative AI application, the Model Context Protocol (MCP) (Anthropic, 2025d ) has recently been released and, subsequently, widely adapted. The MCP is an open protocol which standardizes API calls to large language models (LLMs), data sources, and agentic tools. Thu…

**Results.** Experimental Setup 8 Acknowledgements A MCP Claude Desktop Config File B Claude Attack Examples C Llama-3.3-70B-Instruct Attack Examples D Llama-3.3-70B-Instruct refusals involve explicit harmful/unsafe keywords E McpSafetyScanner determines MCP server vulnerabilities, provides remediations MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits Brandon Radosevich John T. Halloran ∗ Leidos halloranjt@leidos.com Equal Contribution Abstract To reduce development overhead and enable seamless integration between potential components comprising any given generative AI application, the Model Context Protocol (MCP) (Anthropic, 2025d ) has recently been released and, subsequently, widely adapted. The MCP is an open protocol which standardizes API calls to large language models (LLMs), data sources, and agentic tools. Thus, by connecting multiple MCP servers–each defined with a set of to…

**Conclusion.** Conclusions, and Future Work 7 Experimental Setup 8 Acknowledgements A MCP Claude Desktop Config File B Claude Attack Examples C Llama-3.3-70B-Instruct Attack Examples D Llama-3.3-70B-Instruct refusals involve explicit harmful/unsafe keywords E McpSafetyScanner determines MCP server vulnerabilities, provides remediations MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits Brandon Radosevich John T. Halloran ∗ Leidos halloranjt@leidos.com Equal Contribution Abstract To reduce development overhead and enable seamless integration between potential components comprising any given generative AI application, the Model Context Protocol (MCP) (Anthropic, 2025d ) has recently been rele…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[mcp]]
- **Raw:** `raw/arxiv/2504.03767v2.md` · `raw/arxiv/2504.03767v2.fulltext.md`
