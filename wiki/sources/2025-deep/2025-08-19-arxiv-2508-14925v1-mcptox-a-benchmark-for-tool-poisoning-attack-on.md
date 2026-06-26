---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MCPTox: A Benchmark for Tool Poisoning Attack on Real-World MCP Servers"
authors: Zhiqiang Wang, Yichao Gao, Yanting Wang, Suyuan Liu et al.
url: https://arxiv.org/abs/2508.14925v1
date: 2025-08-19
citationCount: 45
influentialCitationCount: 12
velocity: 4.46
ingested: 2026-06-22
tags: [coding-agents, agent-reliability, agent-security, agent-protocols, agent-evaluation, arxiv, 2025, cited]
---

# MCPTox: A Benchmark for Tool Poisoning Attack on Real-World MCP Servers

**arXiv [2508.14925v1](https://arxiv.org/abs/2508.14925v1)** · 2025-08-19 · **45 citations** (12 influential · 4.46/mo) · Zhiqiang Wang, Yichao Gao, Yanting Wang, Suyuan Liu et al.

## Abstract
By providing a standardized interface for LLM agents to interact with external tools, the Model Context Protocol (MCP) is quickly becoming a cornerstone of the modern autonomous agent ecosystem. However, it creates novel attack surfaces due to untrusted external tools. While prior work has focused on attacks injected through external tool outputs, we investigate a more fundamental vulnerability: Tool Poisoning, where malicious instructions are embedded within a tool's metadata without execution. To date, this threat has been primarily demonstrated through isolated cases, lacking a systematic, large-scale evaluation. We introduce MCPTox, the first benchmark to systematically evaluate agent robustness against Tool Poisoning in realistic MCP settings. MCPTox is constructed upon 45 live, real-world MCP servers and 353 authentic tools. To achieve this, we design three distinct attack templates to generate a comprehensive suite of 1312 malicious test cases by few-shot learning, covering 10 categories of potential risks. Our evaluation on 20 prominent LLM agents setting reveals a widespread vulnerability to Tool Poisoning, with o1-mini, achieving an attack success rate of 72.8\%. We find that more capable models are often more susceptible, as the attack exploits their superior instruction-following abilities. Finally, the failure case analysis reveals that agents rarely refuse these attacks, with the highest refused rate (Claude-3.7-Sonnet) less than 3\%, demonstrating that existing safety alignment is ineffective against malicious actions that use legitimate tools for unauthorized operation. Our findings create a crucial empirical baseline for understanding and mitigating this widespread threat, and we release MCPTox for the development of verifiably safer AI agents. Our dataset is available at an anonymized repository: \textit{https://anonymous.4open.science/r/AAAI26-7C02}.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background and Related Work 2.1 Model Context Protocol 2.2 Tool Poisoning Attack in MCP 2.3 Related Benchmarks 3 MCPTox Construction 3.1 Attack Paradigms 3.2 Test Case Generation 3.3 Dataset Format 3.4 LLM Agent Evaluation 4 Experiments 4.1 Experiment Settings 4.2 Attack Success Rates of Different Agents 4.3 Comparison with IPI Benchmark 4.4 Detailed Analysis 5 Limitation and Future Work 6 Conclusion 7 Ethical Considerations References License: arXiv.org perpetual non-exclusive license arXiv:2508.14925v1 [cs.CR] 19 Aug 2025 MCPTox: A Benchmark for Tool Poisoning Attack on Real-World MCP Servers Zhiqiang Wang, 1 Yichao Gao, 1 Yanting Wang 2 Suyuan Liu, 1 Haifeng Sun, 1 Haoran Cheng 1 Guanquan Shi, 2 Haohua Du, 2 Xiangyang Li 1 Abstract By providing a standardized interface for LLM agents to interact with external tools, the Model Context Protocol (MCP) is quickly becoming a cornerstone of the modern autonomous agent ecosystem. However, it creates novel attack surfaces due to untrusted external tools. W…

**Method / approach.** methodology. Furthermore, these benchmarks largely operate within simulated environments, whereas TP is an ecosystem-level threat that must be evaluated against real-world servers. 3 MCPTox Construction This section details the construction and methodology of our MCPTox benchmark. We begin by defining three distinct Attack Paradigms designed to comprehensively evaluate different triggering methods and attack behaviors (§3.1). We then describe our semi-automated Test Case Generation process, which uses these paradigms to create realistic attack scenarios(§3.2). Subsequently, we formalize the Dataset Format (§3.3) and provide a standardized method for using MCPTox to assess LLM agents (§3.4). 3.1 Attack Paradigms To comprehensively evaluate different triggering methods and attack behaviors, we define three distinct attack paradigms (Table 1 ). For each MCP server, we then construct multiple malicious test cases based on these paradigms. Explicit Trigger - Function Hijack…

**Results.** Experiments 4.1 Experiment Settings 4.2 Attack Success Rates of Different Agents 4.3 Comparison with IPI Benchmark 4.4 Detailed Analysis 5 Limitation and Future Work 6 Conclusion 7 Ethical Considerations References License: arXiv.org perpetual non-exclusive license arXiv:2508.14925v1 [cs.CR] 19 Aug 2025 MCPTox: A Benchmark for Tool Poisoning Attack on Real-World MCP Servers Zhiqiang Wang, 1 Yichao Gao, 1 Yanting Wang 2 Suyuan Liu, 1 Haifeng Sun, 1 Haoran Cheng 1 Guanquan Shi, 2 Haohua Du, 2 Xiangyang Li 1 Abstract By providing a standardized interface for LLM agents to interact with external tools, the Model Context Protocol (MCP) is quickly becoming a cornerstone of the modern autonomous agent ecosystem. However, it creates novel attack surfaces due to untrusted external tools. While prior work has focused on attacks injected through external tool outputs, we investigate a more fundamental vulne…

**Conclusion.** Conclusion 7 Ethical Considerations References License: arXiv.org perpetual non-exclusive license arXiv:2508.14925v1 [cs.CR] 19 Aug 2025 MCPTox: A Benchmark for Tool Poisoning Attack on Real-World MCP Servers Zhiqiang Wang, 1 Yichao Gao, 1 Yanting Wang 2 Suyuan Liu, 1 Haifeng Sun, 1 Haoran Cheng 1 Guanquan Shi, 2 Haohua Du, 2 Xiangyang Li 1 Abstract By providing a standardized interface for LLM agents to interact with external tools, the Model Context Protocol (MCP) is quickly becoming a cornerstone of the modern autonomous agent ecosystem. However, it creates novel attack surfaces due to untrusted external tools. While prior work has focused on attacks injected through external tool outputs, we investigate a more…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[claude]]
- **Raw:** `raw/arxiv/2508.14925v1.md` · `raw/arxiv/2508.14925v1.fulltext.md`
