# Awesome Mistral Connectors [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![Last Commit](https://img.shields.io/github/last-commit/rdmgator12/awesome-mistral-connectors)](https://github.com/rdmgator12/awesome-mistral-connectors/commits/main)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com/rdmgator12/awesome-mistral-connectors/)

> A curated directory of Mistral's connector and integration surfaces — **Le Chat Connectors** (consumer + Pro / Team / Enterprise), the **Mistral Agents API built-in tools**, and **native cloud deployment partnerships** — organized by category with descriptions and use cases.

**Last updated:** May 10, 2026 · **Le Chat Connectors:** 25 · **Built-in Agent Tools:** 4 · **Deployment Platforms:** 7 · **Categories:** 10 · **Version:** 1.0.0

Mistral has three integration surfaces, each with a different shape. **Le Chat Connectors** are third-party services connectable inside [Le Chat](https://chat.mistral.ai) — split into *Regular Connectors* (real-time, no indexing, no admin setup; MCP-powered for partners, Mistral-built for Gmail/Calendar/Outlook) and *Knowledge Connectors* (admin-driven indexed connections to Google Drive, SharePoint; indexes stored in EU data centers). The **Mistral Agents API built-in tools** are first-party tools attachable to Agents via the API — web search, code interpreter, image generation, document library (RAG) — plus the Connectors API (Public Preview as of April 2026) which exposes Le Chat connectors and custom MCP servers via the Conversations API, Completions API, and Agent SDK. **Native cloud deployment partnerships** make Mistral models available on Azure AI Foundry, AWS Bedrock, GCP Vertex AI, Snowflake Cortex, IBM watsonx, and others — not user-facing connectors, but the foundation for enterprise deployment.

Mistral's structural quirks worth knowing: Connectors are on the Free plan for all Le Chat users (announced Sept 2, 2025), while Knowledge Connectors are gated to Team / Enterprise. Mistral is an MCP **client, not a publisher** — there is no official `mistralai/*` MCP server. They invert Google's strategy of shipping their own MCP servers; instead they curate a partner directory and accept arbitrary remote MCPs. OAuth 2.1 with dynamic client registration is supported for custom MCP connectors — uncommon, ahead of most competitors. Connector tool data is not used for training — stated unconditionally across plans. Custom MCP connectors do not yet support dynamic tool discovery, MCP resources, or prompt templates.

For more information, see the [Le Chat Connectors docs](https://docs.mistral.ai/le-chat/knowledge-integrations/connectors), the [Custom MCP Connectors guide](https://docs.mistral.ai/le-chat/knowledge-integrations/connectors/mcp-connectors), the [Agents API tools docs](https://docs.mistral.ai/agents/tools), the [Connectors in Studio launch post](https://mistral.ai/news/connectors), and the [Mistral partners page](https://mistral.ai/partners).

**Legend:** 🅜 Built or maintained by Mistral · 🤝 Official MCP partner connector · 🛠️ Community / third-party · 📡 MCP-powered · 🇪🇺 EU data residency stated · ⏳ Announced but not yet live · 💎 Team / Enterprise tier required.

> This is an independent, community-maintained list. Not affiliated with, endorsed by, or sponsored by Mistral AI. "Mistral," "Le Chat," and related marks are the property of Mistral AI. Each connector is the property of its respective owner.

---

## Contents

- [Le Chat Connectors](#le-chat-connectors)
- [Email and Calendar](#email-and-calendar)
- [File Storage and Documents](#file-storage-and-documents)
- [Productivity](#productivity)
- [Development Tools](#development-tools)
- [Data and Databases](#data-and-databases)
- [Commerce and Payments](#commerce-and-payments)
- [Marketing and Automation](#marketing-and-automation)
- [Mistral Agents API](#mistral-agents-api)
- [Built-in Agent Tools](#built-in-agent-tools)
- [Cloud Deployment](#cloud-deployment)
- [Native Platform Partnerships](#native-platform-partnerships)

## Le Chat Connectors

Connectable services inside Le Chat. Mistral splits these into *Regular* (real-time, no setup) and *Knowledge* (admin-indexed, EU-resident). Add via the **+ Add** button on the Connectors page; admins manage at the workspace level.

## Email and Calendar

- 🅜 [Gmail](https://mail.google.com) - Search, draft, and send email from chat. *Use case: Drafting replies grounded in thread history, summarizing inbox state, scheduling around existing commitments.*
- 🅜 [Google Calendar](https://calendar.google.com) - Read and manage calendar events. *Use case: Finding free time across multiple calendars, drafting meeting invites, summarizing the week's commitments.*
- 🅜 [Outlook](https://outlook.com) - Microsoft 365 email and calendar. *Use case: Email triage, calendar coordination, and scheduling automation in Microsoft 365 environments.*

## File Storage and Documents

- 🅜 🇪🇺 💎 [Google Drive](https://drive.google.com) - Knowledge Connector — indexes the team's content; index stored in EU data centers. *Use case: Org-wide search across Docs / Sheets / Slides, summarizing folders, citing artifacts in research output.*
- 🅜 🇪🇺 💎 [Microsoft SharePoint](https://www.microsoft.com/en-us/microsoft-365/sharepoint/collaboration) - Knowledge Connector — indexes the team's sites; index stored in EU data centers. *Use case: Enterprise document search, retrieving policy and procedure docs, summarizing site content.*
- 🤝 📡 [Box](https://www.box.com) - Search, analyze, and get insights from stored files. *Use case: Cross-document search, summarizing folders, pulling artifacts into a research thread.*

## Productivity

- 🤝 📡 [Notion](https://www.notion.so) - Search, summarize, and author content across your workspace. *Use case: Workspace-wide search, drafting new pages from research output, updating databases via natural language.*
- 🤝 📡 [Asana](https://asana.com) - Plan and track projects, tasks, and team workflows. *Use case: Creating tasks from meeting notes, querying project status, surfacing blockers across teams.*
- 🤝 📡 [Monday.com](https://monday.com) - Manage boards, items, and groups; automate project workflows. *Use case: Cross-board project queries, updating item status from research output, automating routine task creation.*
- 🤝 📡 [Atlassian (Jira + Confluence)](https://www.atlassian.com) - Search, summarize, and act on Jira issues and Confluence pages. *Use case: Issue triage, sprint planning, drafting Confluence pages, querying status across projects.*

## Development Tools

- 🤝 📡 [GitHub](https://github.com) - Search repos, review issues, and manage pull requests. *Use case: Repository-wide code search, PR triage, generating commit messages from diffs.*
- 🤝 📡 [Linear](https://linear.app) - Search, summarize, and manage issues and projects. *Use case: Issue management for engineering teams, cycle planning, surfacing in-flight work across projects.*
- 🤝 📡 [Sentry](https://sentry.io) - Error monitoring and application observability. *Use case: Triaging production errors from chat, summarizing incident timelines, correlating issues with releases.*
- 🤝 📡 [Cloudflare Development Platform](https://developers.cloudflare.com) - Workers, Pages, and edge platform. *Use case: Edge deployment workflows, Workers debugging, configuration queries.*
- 🤝 📡 [DeepWiki](https://deepwiki.com) - Conversational Q&A over public code repositories. *Use case: Onboarding into unfamiliar codebases, answering questions about open-source repos without manually reading the docs.*

## Data and Databases

- 🤝 📡 ⏳ [Databricks](https://www.databricks.com) - Lakehouse data platform. *Use case: Querying Unity Catalog tables, running notebooks from natural-language requests, summarizing analytics inline. (Listed as "coming soon" at Sept 2025 launch — verify availability.)*
- 🤝 📡 ⏳ [Snowflake](https://www.snowflake.com) - Cloud data warehouse. *Use case: Cross-warehouse SQL via natural language, schema introspection, ad-hoc analytics. (Listed as "coming soon" at Sept 2025 launch — verify availability.)*
- 🤝 📡 [Pinecone](https://www.pinecone.io) - Vector database. *Use case: Vector index inspection, query tuning for RAG pipelines, debugging retrieval workflows.*
- 🤝 📡 [Prisma Postgres](https://www.prisma.io/postgres) - Managed PostgreSQL with the Prisma stack. *Use case: Schema introspection and queries against Prisma-managed databases without leaving the assistant.*

## Commerce and Payments

- 🤝 📡 [Stripe](https://stripe.com) - Payments platform. *Use case: Querying customers, transactions, and subscriptions; managing payment flows; surfacing dispute state.*
- 🤝 📡 [PayPal](https://www.paypal.com) - Payments and merchant platform. *Use case: Transaction lookup, refund workflows, merchant account ops.*
- 🤝 📡 [Plaid](https://plaid.com) - Banking and financial-account connectivity. *Use case: Account linking workflows, transaction enrichment, balance queries during financial research.*
- 🤝 📡 [Square](https://squareup.com) - Point-of-sale and payments for merchants. *Use case: Sales reporting, inventory queries, merchant operations from chat.*

## Marketing and Automation

- 🤝 📡 [Brevo](https://www.brevo.com) - Email marketing and CRM platform. *Use case: Campaign queries, contact-list management, transactional email setup.*
- 🤝 📡 [Zapier](https://zapier.com) - Workflow automation across 6,000+ apps. *Use case: Triggering and orchestrating cross-app workflows from a chat thread.*

## Mistral Agents API

## Built-in Agent Tools

Built-in tools attachable to Agents via the [Conversations API](https://docs.mistral.ai/agents/conversations) or the [Agent SDK](https://docs.mistral.ai/agents/agents-and-conversations). Set on the `tools` array.

- 🅜 [Web Search](https://docs.mistral.ai/agents/tools#web-search) - Real-time web search with citations. Tool type `web_search` (free) and `web_search_premium` (higher rate limits). *Use case: Grounded answers from the live web, source-cited synthesis, research workflows.*
- 🅜 [Code Interpreter](https://docs.mistral.ai/agents/tools#code-interpreter) - Sandboxed Python execution with plotting and data analysis. Tool type `code_interpreter`. *Use case: Data crunching, generating charts, running analytical computations inside an Agent turn.*
- 🅜 [Image Generation](https://docs.mistral.ai/agents/tools#image-generation) - Generate images from a text prompt. Tool type `image_generation`. *Use case: Inline image creation during chat, prototype visuals, marketing-asset generation.*
- 🅜 [Document Library](https://docs.mistral.ai/agents/tools#document-library) - Built-in RAG over Mistral Cloud-hosted Libraries. Tool type `document_library` with `library_ids[]`. *Use case: Domain-grounded Q&A on uploaded corpora without building a custom retrieval stack.*

> **Connectors API (Public Preview, April 15, 2026)** — Le Chat connectors and custom MCP servers are now exposed via the Conversations API, Completions API, and Agent SDK. Adds direct tool calling and human-in-the-loop approval flows. Console: [console.mistral.ai/build/connectors](https://console.mistral.ai/build/connectors). Management: [docs.mistral.ai/capabilities/connectors/management](https://docs.mistral.ai/capabilities/connectors/management).

## Cloud Deployment

## Native Platform Partnerships

Not user-facing connectors — the cloud platforms where Mistral's models are deployable as managed services. Listed for completeness because Le Chat Enterprise is sold across these surfaces.

- 🤝 [Microsoft Azure (Azure AI / Foundry)](https://azure.microsoft.com/en-us/products/ai-foundry) - First MaaS launch (Mistral Large, Feb 2024); Mistral Large 3 added Dec 2025.
- 🤝 [AWS Bedrock](https://aws.amazon.com/bedrock/) - Managed serverless endpoints. GA March 2024.
- 🤝 [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) - Vertex AI Model Garden + Le Chat Enterprise listing on GCP Marketplace (May 2025).
- 🤝 [Snowflake Cortex](https://www.snowflake.com/en/data-cloud/cortex/) - LLM functions inside the data cloud (Mar 2024).
- 🤝 [IBM watsonx](https://www.ibm.com/products/watsonx-ai) - On-prem and watsonx.ai catalog deployment.
- 🤝 [NVIDIA](https://www.nvidia.com/en-us/ai/) - Inference partnership across NVIDIA platforms.
- 🤝 [Outscale](https://www.outscale.com) - French-sovereign cloud (Mistral's hometown / EU residency story).

## Contributing

Contributions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md) for the submission flow, surface conventions, and the entry style guide. By contributing you agree to the [Code of Conduct](code-of-conduct.md).

The Le Chat connector directory is admin-visible inside Le Chat under **Connectors → Add** and announcement-driven on [mistral.ai/news](https://mistral.ai/news). When new connectors land, submit a PR with the canonical vendor URL, the surface (Regular vs Knowledge vs Custom MCP), and a specific use case.
