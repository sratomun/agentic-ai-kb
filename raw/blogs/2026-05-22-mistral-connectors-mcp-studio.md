# Connect the dots: Build with built-in and custom MCPs in Studio

Source: https://mistral.ai/news/connectors
Author: Mistral AI
Date: May 22, 2026
Category: Product
Captured: 2026-06-22

---

Today we are releasing Connectors in Studio to unblock developers building highly customised AI applications grounded in enterprise data. All built-in connectors, as well as custom MCPs, are now available via API/SDK to be used with all model and agent calls.

We are also introducing direct tool calling, giving developers precise control over how and when tools are invoked, without authentication barriers getting in the way of testing and iterating. In addition, you can now implement human-in-the-loop approval flows, allowing secure review and confirmation before tool execution, ensuring both flexibility and governance.

- Programmatic access for creating, modifying, listing and deleting your connectors but also listing their tools and directly running them.
- All connectors are centrally registered making them available across Mistral apps: LeChat and AI Studio (with Vibe coming soon).
- Usage via Conversation API, Completions API, and Agent SDK can now facilitate complex workflows and integration with enterprise systems like CRMs, knowledgebases & productivity tools.

## Integrations that live in the platform, not in your code

Building enterprise AI agents is getting easier. The harder part is everything around them: tracking down the right API docs, writing and maintaining tool functions, building integrations, setting up OAuth, handling token refresh, and debugging edge cases like broken pagination.

Because of this, teams keep rebuilding the same integration layer. Even within the same company, similar integrations are often implemented multiple times in arbitrary code, leading to security risks, lack of traffic observability, and duplication of work.

A connector solves this by packaging an integration into a single, reusable entity using the MCP protocol.

```python
my_connector = client.beta.connectors.create(
    name="salesforce-crm",
    description="Salesforce CRM — accounts, contacts, opportunities",
    server="https://your-mcp-server.internal/salesforce",
    visibility="shared_workspace",
    oauth_config={...},
)
```

Once registered, the custom MCP connector is discoverable, governed & monitored in Studio and becomes a native tool for any conversation, agent, or workflow without rewriting integration logic, without re-implementing auth, without duplicating it across teams.

## A runnable golden path

An agent for a multi-step workflow reasoning across sources given agent's secure connectivity to GitHub, public repo content & docs, and live data from the web. Uses the DeepWiki remote MCP server (https://mcp.deepwiki.com/mcp) for code repository exploration. GitHub and web are already built into Mistral. `tool_configuration` controls tool availability (e.g. exclude `delete_file`) without modifying the connector.

## Direct tool calling

Not every workflow needs the model to decide when and how tools are invoked. For a more deterministic experience, users can now call connectors directly:

```python
result = await client.beta.connectors.call_tool_async(
    connector_id="my_deepwiki",
    tool_name="read_wiki_structure",
    arguments={"repoName": "sqlite/sqlite"},
)
```

Especially useful for debugging and pipeline-style automation which limits ambiguity.

## When a human needs to be in the loop

Some actions should not execute without explicit approval. `requires_confirmation` pauses execution and hands control back to your application before the tool runs:

```python
{
   "type": "connector",
   "connector_id": "gmail",
   "tool_configuration": {
       "include": ["gmail_search"],
       "requires_confirmation": ["gmail_search"]
   }
}
```

The model proposes, the user application decides whether to proceed. The boundary between AI judgment and human judgment is explicit and written in code.

## Start building

You can now use Connectors in Studio, in Public Preview.
