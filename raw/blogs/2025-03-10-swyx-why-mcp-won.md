# Why MCP Won

- Author: swyx (Shawn Wang)
- Outlet: Latent.Space
- URL: https://www.latent.space/p/why-mcp-won
- Date: 2025-03-10
- Fetched: 2026-06-22
- Note: partially paywalled; full intro + the 6 reasons captured below.

---

"I'm sorry for all the MCP filling your timeline right now." The Model Context Protocol
launched November 2024, decently received, but the initial flurry died down until the
Feb 26-27 AI Engineer Summit, where swyx booked Mahesh Murag's MCP workshop. Livetweets
went viral (~300k combined views in a week).

"To paraphrase Ben Thompson, the #1 feature of any network is the people already on it.
The power of any new protocol derives from its adoption (aka ecosystem)." MCP has
captured enough critical mass that it is "already the presumptive winner of the 2023-2025
'agent open standard' wars." At current pace, MCP will overtake OpenAPI in July (GitHub
star history). Widely accepted standards (Kubernetes, React, HTTP) convert exploding MxN
problems into tractable M+N ecosystem solutions.

swyx admits he underestimated MCP: "I have seen many attempted XKCD 927's come and go."

## Why MCP Won (in rough descending order)
1. **MCP is "AI-Native" version of old idea.** Technically MCP does what OpenAPI / OData
   / GraphQL / SOAP do. But dismissing on a technical basis neglects sociological
   context. MCP was born from lessons in Claude Sonnet's #1 SWE-Bench result and
   Anthropic's "Building Effective Agents." It reifies patterns already independently
   recurring in every Agent — more ergonomic than an agnostic standard. The
   Tools (Model-controlled) / Resources (Application-controlled) / Prompts
   (User-controlled) split, and putting "dynamic context access at the center of its
   universe" ("Models are only as good as the context provided to them"), means it
   resists relitigating LLM interoperability. → Wins over OpenAPI AND LangChain.
2. **MCP is an "open standard" with a big backer.** A standard from a Big Lab is more
   likely to succeed than one from a startup whose financials incentivize lock-in. "If
   the standard backer seems too big to really care about locking you in... I will adopt
   it." MCP also has a VERY good spec. → Wins over Composio et al. and OpenAI function
   calling (whose docs fall short of an exhaustive spec).
3. **Anthropic has the best developer AI brand.** "If you're going to build a developer
   standard, it helps to be beloved by developers." Sonnet has been king ~9 months. MCP
   enables far more average tools in a single call.
4. **MCP based off LSP (Language Server Protocol), an existing successful protocol.**
   Anthropic adapted Microsoft's LSP rather than inventing from scratch. Fungibility
   between clients and servers; stuck to JSON-RPC for messages.
5. **MCP dogfooded with complete set of 1st-party client, servers, tooling, SDKs.**
   Launched with Claude Desktop client, 19 reference servers (memory, filesystem,
   sequential thinking), MCP Inspector, Python + TS SDKs, llms-full.txt docs. Claude
   Code later added a SECOND official MCP client (CLI). → Wins over less-dogfooded
   BigCo attempts like Meta's llama-stack.
6. **MCP started with a minimal base, but with frequent roadmap updates.** Minimal
   surface area is a key devtools concept.

Non-factors (did NOT contribute much): lining up launch partners (Zed, Cody, Replit);
launching with great documentation.

Postscript: OpenAI (3/27) and Google (4/9) announced MCP support after this post.
