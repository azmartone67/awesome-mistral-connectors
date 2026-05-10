# Contributing

This list curates Mistral's connector and integration surfaces: **Le Chat Connectors** (Regular + Knowledge), **Mistral Agents API built-in tools**, and **native cloud deployment partnerships**. Contributions welcome.

> This is an independent, community-maintained project. Not affiliated with, endorsed by, or sponsored by Mistral AI.

## What You Can Contribute

### Le Chat Connector additions
When Mistral adds a new Le Chat connector (announced via [mistral.ai/news](https://mistral.ai/news), updated in [docs.mistral.ai](https://docs.mistral.ai/le-chat/knowledge-integrations/connectors), or visible inside Le Chat under **Connectors → Add**), submit a PR adding it to the appropriate category.

Note the connector's surface class:
- **Regular Connector** — real-time, no indexing, no admin setup. Use 🤝 📡 if MCP-powered partner-built; use 🅜 if Mistral-built.
- **Knowledge Connector** — admin-driven, indexed, EU-resident. Use 🅜 🇪🇺 💎 (Team / Enterprise gated).
- **Custom MCP** — user-supplied remote MCP. Don't list custom MCPs unless they're Mistral-curated partner connectors.

### Built-in Agent Tool additions
When Mistral adds a new built-in tool to the Agents API (`tools[].type` value), submit a PR with the tool type, the docs URL, and a use case.

### Deployment Platform additions
When Mistral lands on a new managed-deployment surface (Azure Foundry, Bedrock, Vertex, etc.), submit a PR. Keep this section narrow — model availability only, not adjacent ecosystem (e.g., don't list every cloud-database that *could* call a Mistral endpoint).

### Improved Descriptions
If a description or use case is generic or vague, submit a PR with a more specific one. Use cases should describe what the connector actually unlocks, not what its homepage marketing says.

### Category Corrections
If a connector is in the wrong category, submit a PR moving it.

### Legend / Metadata Corrections
If a 🅜 / 🤝 / 🛠️ / 📡 / 🇪🇺 / ⏳ / 💎 emoji is wrong, submit a PR fixing it.

### Field Reports
Tested a connector and have real-world notes? Add a brief field report below the entry:

```markdown
- 🤝 📡 [Connector Name](https://example.com) - Description. *Use case: ...*
  > **Field report:** One paragraph on what worked, what didn't, what surprised you. Be specific.
```

## Guidelines

- One PR per change unless closely related.
- Keep descriptions concise — one sentence for the description, one for the use case.
- Use cases should be specific and practical, not marketing copy.
- Link to the **vendor's canonical homepage**, not a Mistral docs page (exception: Mistral-built connectors and built-in Agent tools — link to `docs.mistral.ai`).
- Maintain alphabetical order within categories.
- Apply the legend correctly:
  - 🅜 = built/maintained by Mistral
  - 🤝 = official MCP partner connector (third-party-built, Mistral-curated)
  - 🛠️ = community / third-party (rare in this list — most third-party are partner-curated)
  - 📡 = MCP-powered
  - 🇪🇺 = EU data residency stated
  - ⏳ = announced but not yet live as of last public update
  - 💎 = Team / Enterprise tier required

## Surface Notes

Mistral's connector ecosystem launched in waves:
- **Feb 6, 2025** — Le Chat Pro/Team launched; "data connectors and multi-step agents coming soon."
- **May 7, 2025** — Le Chat Enterprise GA with the first wave of Knowledge Connectors (Drive, SharePoint, OneDrive, Calendar, Gmail).
- **Sept 2, 2025** — MCP Connectors directory (20+ partners) and Memories rolled out to the Free plan.
- **Sept 13–14, 2025** — Paris MCP hackathon.
- **Apr 15, 2026** — Connectors in Studio (Public Preview): API/SDK exposure, direct tool calling, human-in-the-loop approval.

Mistral does not publish a public connector registry endpoint or SDK enumeration. Net result: the "ground truth" is the Le Chat **Connectors → Add** UI plus mistral.ai/news. When Mistral updates its directory between announcements, this list will lag — please open an issue or PR if you spot drift.

## Updates

This list is updated as Mistral publishes new connectors, built-in tools, or deployment surfaces. If you notice changes that aren't reflected here, please open an issue or PR.
