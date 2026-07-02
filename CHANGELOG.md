# Changelog

All notable changes to this list will be documented in this file. Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versioning follows [Semantic Versioning](https://semver.org/) — MAJOR for category restructures, MINOR for new entries, PATCH for description/URL fixes.

## [Unreleased]

### Planned
- Audit the Le Chat **Connectors → + Add Connector** UI for any partner connectors not yet announced publicly (surface drift between mistral.ai/news posts and the live directory).
- Add a "Custom MCP examples" appendix linking to high-signal community MCP servers known to work with Le Chat (without polluting the curated partner list).

---

## [2.0.1] - 2026-07-02

### Fixed
- Corrected the Connectors-in-Studio launch date in the README's Connectors API callout: the cited post ([mistral.ai/news/connectors](https://mistral.ai/news/connectors), "Connect the dots: Build with built-in and custom MCPs in Studio") is dated **May 22, 2026**, not April 15, 2026. Earlier CHANGELOG entries retain the original wording as historical record.

### Changed
- Header bumped: version 2.0.1, `Last updated` July 2, 2026.
- Added the inaugural **Connector of the Week** block (rotates weekly), matching the sibling-list convention. First pick: Hugging Face — an editorial choice in a zero-churn week.

### Notes
- June 26 – July 2 sweep: **no connector additions or removals.** Re-diffed the June 24 post's full enumeration against the README — 64/64 exact match across all 10 categories; docs Featured tab unchanged (same 12); no Mistral news posts after June 24. Directory stays at 65 (64 enumerated + SharePoint Search API featured variant).
- Watch items: Le Chat → Vibe brand consolidation accelerating in third-party framing (Android app now "Vibe by Mistral (ex-Le Chat)") — a completed rename would force a MAJOR-level retitle. Per-function connector permission toggles are now documented in the MCP Connectors docs (undated; candidate for next content update). Mistral's own naming wobbles between Connectors "Debugger" (post body) and "Playground" (post closing) — README follows the body.

---

## [2.0.0] - 2026-06-26

Major reconcile against the [June 24, 2026 "Bringing more control over your connectors"](https://mistral.ai/news/more-control-over-connectors/) post, which published the full directory (60+ integrations, 64 enumerated) and a 10-category taxonomy. Structural restructure → MAJOR bump.

### Added
- **37 new connectors** from the official directory: BigQuery, MDN, Microsoft Learn, Needle, Supabase, Synapse (Sage Bionetworks) under Knowledge, Data and AI; Hugging Face, Jina, Tavily under Machine Learning; Outlook Calendar, Clockwise, Fireflies under Communication and Scheduling; Close, HubSpot, Intercom, Salesforce, ServiceNow under Work and Customer Operations; Morningstar, Kensho, Pigment under Payments and Financial Data; Amplitude, Hex, Vantage under Analytics and Business Intelligence; Netlify, Stytch under Developer Platforms and Infrastructure; Apify, n8n, Workato under Automation and Integration; BioRender, Data.gouv, PubMed, Scholar Gateway (Wiley) under Research, Scientific and Public Data; Bria, Bright (Bright Data), Cloudinary, Mermaid, Trivago under Content and Media Management.
- **⭐ Featured connector** legend marker (direct OAuth, click-to-connect). Featured set tagged: Atlassian, Box, GitHub, Gmail, Google Calendar, Linear, Notion, Outlook, Outlook Calendar, SharePoint Search API, Slack, Stripe.
- About-section coverage of the **Vibe / Work / Chat / Code** mode split (connectors now live under Work), and the June 24 governance shipment: enriched admin controls (GA), API keys with connector scopes (GA), multi-account connectors (GA), Connectors Debugger (Public Preview), Connectors in Vibe Code (GA), Connectors in Workflows (Public Preview).

### Changed
- **Category restructure:** README sections realigned to Mistral's official 10-category directory taxonomy (Knowledge, Data and AI; Machine Learning; Communication and Scheduling; Work and Customer Operations; Payments and Financial Data; Analytics and Business Intelligence; Developer Platforms and Infrastructure; Automation and Integration; Research, Scientific and Public Data; Content and Media Management). Retires the prior surface-grouped categories.
- **Outlook** split into **Outlook** (email) and **Outlook Calendar** (calendar) to match Mistral's directory.
- Header date → June 26, 2026. Le Chat Connectors count: 28 → 65 (64 directory + SharePoint Search API real-time variant). Connector categories: 11 → 10.

### Removed
- **⏳ "coming soon" flags** on Databricks and Snowflake — both are listed plainly in the June 24 GA directory.

---

## [1.1.0] - 2026-06-05

### Added
- **Slack** under Productivity - Le Chat Regular Connector (🤝 📡 official MCP partner). Search messages, read channels, send messages, and manage canvases.
- **SharePoint Search API** under File Storage and Documents - Mistral-built (🅜) real-time surface over the Microsoft Graph Search API (no indexing). Distinct from the existing admin-indexed, EU-resident **Microsoft SharePoint** Knowledge Connector.

### Changed
- Full reconcile against the official Le Chat connector directory diff (Jun 5, 2026).
- Header date → June 5, 2026.
- Le Chat Connectors count: 26 → 28.

---

## [1.0.2] — 2026-05-22

### Added
- **Dell Technologies AI Factory** under Native Platform Partnerships — expanded collaboration announced [May 18, 2026 at Dell Technologies World](https://www.dell.com/en-us/dt/corporate/newsroom/announcements/detailpage.press-releases~usa~2026~05~mistral-ai-powers-ai-innovation-on-dell-technologies-infrastructure.htm). Mistral language and reasoning models plus orchestration tools brought to Dell PowerRack + NVIDIA GB200 NVL72 on-premises environments.

### Changed
- Header date → May 22, 2026.
- Deployment Platforms count: 7 → 8.

---

## [1.0.1] — 2026-05-15

### Added
- **CMS and Web Publishing** — new category (11th overall).
- **WebsitePublisher.ai** under the new category — directory connector announced [May 5, 2026](https://dev.to/megberts/were-now-in-mistrals-connector-directory-heres-what-that-means-for-ai-powered-web-publishing-206). 44+ MCP tools spanning pages, assets, dynamic entities, forms, and publish-to-live-URL workflows. OAuth 2.1 + DCR.
- About-section bullet for **Le Chat Work Mode** (Apr 29, 2026) — agentic multi-step workflow execution across connected tools with human-in-the-loop approval, Pro / Team / Enterprise. Shifts connectors from single-call lookups to persistent task sessions.

### Changed
- Header date → May 15, 2026.
- Le Chat Connectors count: 25 → 26. Categories: 10 → 11.

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

[Unreleased]: https://github.com/rdmgator12/awesome-mistral-connectors/compare/v2.0.0...HEAD
[2.0.0]: https://github.com/rdmgator12/awesome-mistral-connectors/compare/v1.1.0...v2.0.0
[1.1.0]: https://github.com/rdmgator12/awesome-mistral-connectors/compare/v1.0.2...v1.1.0
[1.0.2]: https://github.com/rdmgator12/awesome-mistral-connectors/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/rdmgator12/awesome-mistral-connectors/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/rdmgator12/awesome-mistral-connectors/releases/tag/v1.0.0
