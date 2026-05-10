# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for new entries, PATCH for description/URL fixes.

## [Unreleased]

### Planned for v1.1.0
- Audit the Le Chat **Connectors → Add** UI for any partner connectors not yet announced publicly (surface drift between mistral.ai/news posts and the live directory).
- Track the Sept 2025 "coming soon" entries (Databricks, Snowflake) to confirm general availability and remove the ⏳ flag.
- Add a "Custom MCP examples" appendix linking to high-signal community MCP servers known to work with Le Chat (without polluting the curated partner list).
- Add `awesome-lint` to CI once the repo is ≥30 days old (lint blocks submissions on `git-repo-age` until 2026-06-09).

---

## [1.0.0] — 2026-05-10

### Added
- Initial seed covering Mistral's three integration surfaces:
  - **Le Chat Connectors:** 25 entries across Email & Calendar, File Storage, Productivity, Development Tools, Data & Databases, Commerce & Payments, and Marketing & Automation. Sourced from [docs.mistral.ai/le-chat/knowledge-integrations/connectors](https://docs.mistral.ai/le-chat/knowledge-integrations/connectors), the [Sept 2, 2025 MCP Connectors launch post](https://mistral.ai/news/le-chat-mcp-connectors-memories), and the [Help Center](https://help.mistral.ai/en/collections/911943-connectors).
  - **Mistral Agents API built-in tools:** 4 entries (`web_search`, `code_interpreter`, `image_generation`, `document_library`) plus a callout for the [April 15, 2026 Connectors in Studio Public Preview](https://mistral.ai/news/connectors).
  - **Native cloud deployment partnerships:** 7 platforms (Azure AI Foundry, AWS Bedrock, GCP Vertex AI, Snowflake Cortex, IBM watsonx, NVIDIA, Outscale).
- README.md with About, Legend (🅜 🤝 🛠️ 📡 🇪🇺 ⏳ 💎), surface-grouped Contents, and per-entry use cases.
- CONTRIBUTING.md with Mistral-specific surface guidance and launch-timeline notes.
- CHANGELOG.md (this file).
- LICENSE (CC0-1.0) — awesome-list canonical convention.
- code-of-conduct.md (Contributor Covenant 2.1).
- .editorconfig + .gitignore.
- Badges row: Awesome, License (CC0-1.0), Last Commit, Track Awesome List.

### Notes
- Mistral does not publish a public connector registry endpoint or SDK enumeration; the directory is admin-visible inside Le Chat and announcement-driven on [mistral.ai/news](https://mistral.ai/news).
- Mistral is an MCP **client**, not a publisher — there is no official `mistralai/*` MCP server. Custom-MCP connectors are user-supplied remote endpoints; they're not enumerated in this list.
- EU data residency is explicitly claimed for Knowledge Connectors (Drive, SharePoint) — flagged with 🇪🇺.
- Sept 2025 launch flagged Databricks and Snowflake as "coming soon" — listed here with ⏳ pending GA confirmation.

[Unreleased]: https://github.com/rdmgator12/awesome-mistral-connectors/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/rdmgator12/awesome-mistral-connectors/releases/tag/v1.0.0
