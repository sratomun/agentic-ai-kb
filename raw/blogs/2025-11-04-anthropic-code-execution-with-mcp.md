# Code execution with MCP: Building more efficient agents

- **Source:** Anthropic Engineering
- **URL:** https://www.anthropic.com/engineering/code-execution-with-mcp
- **Published:** 2025-11-04
- **Authors:** Adam Jones, Conor Kelly
- **Captured:** 2026-06-22 (web_fetch, full text)

---

Direct tool calls consume context for each definition and result. Agents scale better by writing code to call tools instead. Here's how it works with MCP.

The Model Context Protocol (MCP) is an open standard for connecting AI agents to external systems. Connecting agents to tools/data traditionally requires a custom integration for each pairing; MCP provides a universal protocol — implement once and unlock an ecosystem. Since launching MCP in November 2024, adoption has been rapid: the community has built thousands of MCP servers, SDKs exist for all major languages, and the industry has adopted MCP as the de-facto standard.

Today developers routinely build agents with access to hundreds or thousands of tools across dozens of MCP servers. As the number of connected tools grows, loading all tool definitions upfront and passing intermediate results through the context window slows agents and increases costs.

## Excessive token consumption from tools makes agents less efficient
Two common patterns increase cost and latency:

**1. Tool definitions overload the context window.** Most MCP clients load all tool definitions upfront into context. With thousands of tools, agents process hundreds of thousands of tokens before reading a request.

**2. Intermediate tool results consume additional tokens.** Example: "Download my meeting transcript from Google Drive and attach it to the Salesforce lead." The model calls `gdrive.getDocument(...)` (full transcript loaded into context), then `salesforce.updateRecord(...)` (model writes the entire transcript into context again). The transcript flows through twice. For a 2-hour sales meeting that could be 50,000 extra tokens; larger documents may exceed context limits.

## Code execution with MCP improves context efficiency
Present MCP servers as **code APIs** rather than direct tool calls; the agent writes code to interact with them. One approach: generate a file tree of all available tools from connected MCP servers (TypeScript):

```
servers
├── google-drive
│   ├── getDocument.ts
│   └── index.ts
├── salesforce
│   ├── updateRecord.ts
│   └── index.ts
```

Each tool corresponds to a file (e.g., `getDocument.ts` calling `callMCPTool('google_drive__get_document', input)`). The Google Drive → Salesforce example becomes:

```
const transcript = (await gdrive.getDocument({ documentId: 'abc123' })).content;
await salesforce.updateRecord({ objectType: 'SalesMeeting', recordId: '00Q...', data: { Notes: transcript } });
```

The agent discovers tools by exploring the filesystem — listing `./servers/` then reading specific tool files it needs. This loads only the definitions needed for the current task: **reduces token usage from 150,000 to 2,000 tokens — a 98.7% saving.** Cloudflare published similar findings ("Code Mode"). Core insight: LLMs are adept at writing code; use that strength to interact with MCP servers more efficiently.

## Benefits of code execution with MCP

**Progressive disclosure** — models navigate filesystems well; read tool definitions on-demand. Alternatively a `search_tools` tool finds relevant definitions, with a detail-level parameter (name only / name + description / full definition with schemas) to conserve context.

**Context-efficient tool results** — filter/transform results in code before returning. Fetching a 10,000-row spreadsheet: with code execution, filter in the environment (`allRows.filter(row => row["Status"] === 'pending')`) and the agent sees 5 rows instead of 10,000. Works for aggregations, joins, extracting specific fields.

**More powerful, context-efficient control flow** — loops, conditionals, error handling done with familiar code patterns rather than chaining individual tool calls (e.g., a `while` loop polling Slack for a deployment notification). Saves on time-to-first-token latency: the code execution environment evaluates conditionals rather than the model.

**Privacy-preserving operations** — intermediate results stay in the execution environment by default; the agent only sees what you explicitly log or return. For sensitive workloads, the harness can tokenize PII automatically before it reaches the model, then untokenize via lookup in the MCP client when shared with another tool. Real data flows Google Sheets → Salesforce but never through the model. Enables deterministic security rules about where data can flow.

**State persistence and skills** — filesystem access lets agents maintain state across operations (write intermediate results to files, resume work). Agents can persist their own code as reusable functions; adding a SKILL.md creates a structured **Skill** the model can reference. Over time the agent builds a toolbox of higher-level capabilities, evolving its own scaffolding.

Note: code execution introduces complexity — running agent-generated code requires a secure execution environment with sandboxing, resource limits, and monitoring. Benefits (reduced token costs, lower latency, improved tool composition) should be weighed against these implementation costs.

## Summary
MCP provides a foundational protocol for agents to connect to many tools/systems. Once too many servers are connected, tool definitions and results consume excessive tokens. Many problems here (context management, tool composition, state persistence) have known solutions from software engineering; code execution applies these established patterns to agents.
