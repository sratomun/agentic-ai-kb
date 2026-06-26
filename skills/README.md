# Skills — registry

All of Sage's invokable workflows live here, one folder per skill. Each is a
self-contained `SKILL.md` (the Anthropic skill convention: a skill = a directory).
The per-area `CLAUDE.md` "hats" provide context; these are the *automations*.
Data and config stay in their area folders — skills reach them via `wiki/`.

| Skill | Folder | What it does | Reads/writes |
|-------|--------|--------------|--------------|
| arXiv scanner | `arxiv-scanner/` | Pull agents-centric papers into the knowledge graph; build censuses; enrich citations | `wiki/` (raw + wiki) |
| Blog scanner | `blog-scanner/` | Pull *technical essays & opinion* from named authors/labs; add person nodes + attributed stance/debate notes | `wiki/` (raw + wiki) |
| KG curator | `kg-curator/` | Tend the graph: mine new nodes, reciprocal links, enrich citation sections, normalize to templates, lint integrity | `wiki/` (wiki) |

## Conventions
- A skill is a folder with `SKILL.md` (YAML frontmatter: `name`, `description` +
  trigger phrases).
- Skills own their *workflow*; areas own their *data, config, and hat*.

