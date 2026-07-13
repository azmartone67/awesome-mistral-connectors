# Awesome Mistral Connectors [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![Last Commit](https://img.shields.io/github/last-commit/rdmgator12/awesome-mistral-connectors)](https://github.com/rdmgator12/awesome-mistral-connectors/commits/main)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com/rdmgator12/awesome-mistral-connectors/)

> A curated directory of Mistral's connector and integration surfaces — **Le Chat / Work Connectors** (the featured OAuth connectors plus the curated MCP directory), the **Mistral Agents API built-in tools**, and **native cloud deployment partnerships** — organized by Mistral's official category taxonomy with descriptions and use cases.

**Last updated:** July 2, 2026 · **Le Chat Connectors:** 65 · **Built-in Agent Tools:** 4 · **Deployment Platforms:** 8 · **Connector categories:** 10 · **Version:** 2.0.1

Mistral has three integration surfaces, each with a different shape. **Le Chat Connectors** are third-party services connectable inside Le Chat / Work — split into **Featured Connectors** (direct OAuth, click-to-connect; Mistral-built for Gmail / Calendar / Outlook, partner-built for the rest) and the **MCP Connectors directory** (a curated, admin-added catalog of partner MCP servers), plus **Custom MCP Connectors** (point Work at any remote MCP server you trust). A subset are **Knowledge Connectors** (admin-driven indexed connections to Google Drive and SharePoint; indexes stored in EU data centers). The **Mistral Agents API built-in tools** are first-party tools attachable to Agents via the API — web search, code interpreter, image generation, document library (RAG) — plus the Connectors API which exposes Le Chat connectors and custom MCP servers via the Conversations API, Completions API, and Agent SDK. **Native cloud deployment partnerships** make Mistral models available on Azure AI Foundry, AWS Bedrock, GCP Vertex AI, Snowflake Cortex, IBM watsonx, and others — not user-facing connectors, but the foundation for enterprise deployment.

As of mid-2026 Le Chat is organized into **Vibe / Work / Chat / Code** modes, and connectors live under **Work** (and are reusable in **Vibe Code**). The [June 24, 2026 connectors update](https://mistral.ai/news/more-control-over-connectors/) put the directory past **60 integrations** (64 enumerated, organized into the 10 categories below) and shipped enterprise governance: **enriched admin controls** (workspace/org + per-tool on/off, GA), **API keys with connector scopes** (GA), **multi-account connectors** (GA), a **Connectors Debugger** (11-step MCP root-cause analysis, Public Preview), **Connectors in Vibe Code** (GA), and **Connectors in Workflows** (Public Preview) for long-running scheduled runs that don't break on auth.

Mistral's structural quirks worth knowing: Connectors are on the Free plan for all Le Chat users (announced Sept 2, 2025), while Knowledge Connectors are gated to Team / Enterprise. Mistral is an MCP **client, not a publisher** — there is no official `mistralai/*` MCP server. They invert Google's strategy of shipping their own MCP servers; instead they curate a partner directory and accept arbitrary remote MCPs. OAuth 2.1 with dynamic client registration is supported for custom MCP connectors — uncommon, ahead of most competitors. Connector tool data is not used for training — stated unconditionally across plans. Custom MCP connectors do not yet support dynamic tool discovery, MCP resources, or prompt templates. **Work Mode** (April 29, 2026) shifts connectors from single-call lookups to agentic multi-step workflows across connected tools with human-in-the-loop approval on sensitive operations.

For more information, see the [Le Chat Connectors docs](https://docs.mistral.ai/le-chat/knowledge-integrations/connectors), the [Custom MCP Connectors guide](https://docs.mistral.ai/le-chat/knowledge-integrations/connectors/mcp-connectors), the [Agents API tools docs](https://docs.mistral.ai/agents/tools), the [Connectors in Studio launch post](https://mistral.ai/news/connectors), and the [Mistral partners page](https://mistral.ai/partners).

**Legend:** 🅜 Built or maintained by Mistral · 🤝 Official MCP partner connector · 🛠️ Community / third-party · 📡 MCP-powered · 🇪🇺 EU data residency stated · ⭐ Featured connector (direct OAuth, click-to-connect) · 💎 Team / Enterprise tier required.

> This is an independent, community-maintained list. Not affiliated with, endorsed by, or sponsored by Mistral AI. "Mistral," "Le Chat," and related marks are the property of Mistral AI. Each connector is the property of its respective owner.

> [!TIP]
> ### Connector of the Week — July 2, 2026
>
> **Hugging Face** · *Machine Learning*
>
> Inaugural pick in a zero-churn week (the directory is unchanged since the June 24 update), so it goes to the connector that best fits the house: Hugging Face in Le Chat is the most on-brand integration in the directory — Europe's open-model champion wired to the world's open-model hub. Ask Work to find a model for a task, compare checkpoints, pull dataset metadata, or trace a model card's lineage without leaving the chat. For a company that publishes its own weights on the Hub, this connector is less a third-party integration than a homecoming. Listed under Machine Learning below.

---

## Contents

- [Le Chat Connectors](#le-chat-connectors)
  - [Knowledge, Data and AI](#knowledge-data-and-ai)
  - [Machine Learning](#machine-learning)
  - [Communication and Scheduling](#communication-and-scheduling)
  - [Work and Customer Operations](#work-and-customer-operations)
  - [Payments and Financial Data](#payments-and-financial-data)
  - [Analytics and Business Intelligence](#analytics-and-business-intelligence)
  - [Developer Platforms and Infrastructure](#developer-platforms-and-infrastructure)
  - [Automation and Integration](#automation-and-integration)
  - [Research, Scientific and Public Data](#research-scientific-and-public-data)
  - [Content and Media Management](#content-and-media-management)
- [Mistral Agents API](#mistral-agents-api)
  - [Built-in Agent Tools](#built-in-agent-tools)
- [Cloud Deployment](#cloud-deployment)
  - [Native Platform Partnerships](#native-platform-partnerships)

## Le Chat Connectors

Connectable services inside Le Chat / Work. **Featured Connectors** (⭐) use a direct OAuth flow — click `Connect` on the card and authenticate; the featured set is Atlassian, Box, GitHub, Gmail, Google Calendar, Linear, Notion, Outlook, Outlook Calendar, SharePoint Search API, Slack, and Stripe. Everything else comes from the **MCP Connectors directory** — an admin adds it via **+ Add Connector → Browse the directory**. **Knowledge Connectors** (🇪🇺 💎 — Google Drive, SharePoint) require admin setup because they index your team's files into EU data centers. Categories below mirror Mistral's official directory taxonomy (per the June 24, 2026 update).

### Knowledge, Data and AI

- 🤝 📡 ⭐ [Atlassian (Jira + Confluence)](https://www.atlassian.com) - Search, summarize, and act on Jira issues and Confluence pages. *Use case: Issue triage, sprint planning, drafting Confluence pages, querying status across projects.*
- 🤝 📡 [BigQuery](https://cloud.google.com/bigquery) - Google Cloud's serverless data warehouse. *Use case: Natural-language SQL over BigQuery datasets, schema introspection, ad-hoc analytics inline.*
- 🤝 📡 ⭐ [Box](https://www.box.com) - Search, analyze, and get insights from stored files. *Use case: Cross-document search, summarizing folders, pulling artifacts into a research thread.*
- 🅜 🇪🇺 💎 [Google Drive](https://drive.google.com) - Knowledge Connector — indexes the team's content; index stored in EU data centers. *Use case: Org-wide search across Docs / Sheets / Slides, summarizing folders, citing artifacts in research output.*
- 🤝 📡 ⭐ [Notion](https://www.notion.so) - Search, summarize, and author content across your workspace. *Use case: Workspace-wide search, drafting new pages from research output, updating databases via natural language.*
- 🅜 🇪🇺 💎 [SharePoint](https://www.microsoft.com/en-us/microsoft-365/sharepoint/collaboration) - Knowledge Connector — indexes the team's sites; index stored in EU data centers. *Use case: Enterprise document search, retrieving policy and procedure docs, summarizing site content.*
- 🅜 ⭐ [SharePoint Search API](https://learn.microsoft.com/en-us/graph/search-concept-overview) - Featured real-time surface over the Microsoft Graph Search API (no indexing). Distinct from the indexed SharePoint Knowledge Connector above. *Use case: On-demand SharePoint lookups, retrieving site files inline, citing documents without an admin-managed index.*
- 🤝 📡 [Databricks](https://www.databricks.com) - Lakehouse data platform. *Use case: Querying Unity Catalog tables, running notebooks from natural-language requests, summarizing analytics inline.*
- 🤝 📡 [DC Hub](https://dchub.cloud) - Live infrastructure data layer for AI agents: 21,000+ data-center facilities, real-time grid / fiber / gas, and 4,000+ tracked deals across 170+ countries. *Use case: Grounding data-center siting, power-availability, and market questions in cited, daily-refreshed infrastructure data (CC-BY-4.0). Connect the MCP server at https://dchub.cloud/mcp — no key needed for the free tier.*
- 🤝 📡 [MDN](https://developer.mozilla.org) - Mozilla Developer Network web-platform documentation. *Use case: Authoritative HTML / CSS / JS / Web API reference grounded in MDN, cited inline in code answers.*
- 🤝 📡 [Microsoft Learn](https://learn.microsoft.com) - Official Microsoft / Azure / .NET technical documentation. *Use case: Grounded answers from canonical Microsoft docs, API reference, deployment guidance.*
- 🤝 📡 [Needle](https://needle.app) - Managed RAG / semantic search over your document collections. *Use case: Querying a hosted knowledge base (PDF / DOCX / web) with citations, without building a vector stack.*
- 🤝 📡 [Prisma Postgres](https://www.prisma.io/postgres) - Managed PostgreSQL with the Prisma stack. *Use case: Schema introspection and queries against Prisma-managed databases without leaving the assistant.*
- 🤝 📡 [Snowflake](https://www.snowflake.com) - Cloud data warehouse. *Use case: Cross-warehouse SQL via natural language, schema introspection, ad-hoc analytics.*
- 🤝 📡 [Supabase](https://supabase.com) - PostgreSQL app backend (database, auth, storage). *Use case: Schema introspection and queries against the Supabase database, inspecting auth and storage from chat.*
- 🤝 📡 [Synapse](https://www.synapse.org) - [Sage Bionetworks'](https://github.com/Sage-Bionetworks/synapse-mcp) collaborative research-data platform — search datasets, inspect entity metadata, explore project hierarchies, and trace provenance through its hosted OAuth2 MCP server. *Use case: Grounding biomedical research in shared Synapse datasets, citing entity metadata and provenance inline.*

### Machine Learning

- 🤝 📡 [DeepWiki](https://deepwiki.com) - Conversational Q&A over public code repositories. *Use case: Onboarding into unfamiliar codebases, answering questions about open-source repos without manually reading the docs.*
- 🤝 📡 [Hugging Face](https://huggingface.co) - Models, datasets, and Spaces hub. *Use case: Searching models and datasets, pulling model cards, exploring the Hub inline.*
- 🤝 📡 [Jina](https://jina.ai) - Neural search, embeddings, reranking, and the Reader (URL → LLM-ready text). *Use case: Reading web pages cleanly, generating embeddings, reranking results for retrieval pipelines.*
- 🤝 📡 [Pinecone](https://www.pinecone.io) - Vector database. *Use case: Vector index inspection, query tuning for RAG pipelines, debugging retrieval workflows.*
- 🤝 📡 [Tavily](https://tavily.com) - Web search and extraction API built for AI agents. *Use case: Grounded web search with content extraction and citations inside an agent turn.*

### Communication and Scheduling

- 🅜 ⭐ [Gmail](https://mail.google.com) - Search, draft, and send email from chat. *Use case: Drafting replies grounded in thread history, summarizing inbox state, scheduling around existing commitments.*
- 🅜 ⭐ [Google Calendar](https://calendar.google.com) - Read and manage calendar events. *Use case: Finding free time across multiple calendars, drafting meeting invites, summarizing the week's commitments.*
- 🅜 ⭐ [Outlook](https://outlook.com) - Microsoft 365 email (read and send). *Use case: Email triage, drafting replies, and inbox summarization in Microsoft 365 environments.*
- 🅜 ⭐ [Outlook Calendar](https://outlook.com/calendar) - Manage your Outlook calendar — search events, schedule and delete meetings, accept or decline invitations. *Use case: Microsoft 365 scheduling automation, coordinating meetings, triaging invites.*
- 🤝 📡 ⭐ [Slack](https://slack.com) - Search messages, read channels, send messages, and manage canvases. *Use case: Surfacing decisions buried in channel history, posting status updates from research output, drafting canvases for the team.*
- 🤝 📡 [Brevo](https://www.brevo.com) - Email marketing and CRM platform. *Use case: Campaign queries, contact-list management, transactional email setup.*
- 🤝 📡 [Clockwise](https://www.getclockwise.com) - AI calendar assistant for focus time and team scheduling. *Use case: Optimizing meeting placement, protecting focus blocks, coordinating schedules across a team.*
- 🤝 📡 [Fireflies](https://fireflies.ai) - AI meeting notetaker and transcription. *Use case: Searching meeting transcripts, pulling action items, summarizing calls into follow-ups.*

### Work and Customer Operations

- 🤝 📡 [Asana](https://asana.com) - Plan and track projects, tasks, and team workflows. *Use case: Creating tasks from meeting notes, querying project status, surfacing blockers across teams.*
- 🤝 📡 ⭐ [Linear](https://linear.app) - Search, summarize, and manage issues and projects. *Use case: Issue management for engineering teams, cycle planning, surfacing in-flight work across projects.*
- 🤝 📡 [Monday.com](https://monday.com) - Manage boards, items, and groups; automate project workflows. *Use case: Cross-board project queries, updating item status from research output, automating routine task creation.*
- 🤝 📡 [Close](https://close.com) - Sales CRM for startups and SMBs. *Use case: Querying leads and opportunities, logging activity, surfacing pipeline status.*
- 🤝 📡 [HubSpot](https://www.hubspot.com) - CRM with marketing, sales, and service hubs. *Use case: Contact and deal lookups, pipeline reporting, drafting follow-ups from CRM context.*
- 🤝 📡 [Intercom](https://www.intercom.com) - Customer messaging and support platform. *Use case: Triaging conversations, summarizing support threads, drafting customer replies.*
- 🤝 📡 [Salesforce](https://www.salesforce.com) - Enterprise CRM. *Use case: Querying accounts / contacts / opportunities, renewal and pipeline analysis, updating records via natural language.*
- 🤝 📡 [ServiceNow](https://www.servicenow.com) - ITSM and enterprise workflow platform. *Use case: Incident and ticket triage, change requests, querying the CMDB from chat.*

### Payments and Financial Data

- 🤝 📡 ⭐ [Stripe](https://stripe.com) - Payments platform. *Use case: Querying customers, transactions, and subscriptions; managing payment flows; surfacing dispute state.*
- 🤝 📡 [PayPal](https://www.paypal.com) - Payments and merchant platform. *Use case: Transaction lookup, refund workflows, merchant account ops.*
- 🤝 📡 [Square](https://squareup.com) - Point-of-sale and payments for merchants. *Use case: Sales reporting, inventory queries, merchant operations from chat.*
- 🤝 📡 [Plaid](https://plaid.com) - Banking and financial-account connectivity. *Use case: Account linking workflows, transaction enrichment, balance queries during financial research.*
- 🤝 📡 [Morningstar](https://www.morningstar.com) - Investment research and market data. *Use case: Fund and equity research, ratings lookups, pulling portfolio data inline.*
- 🤝 📡 [Kensho](https://kensho.com) - S&P Global's AI and analytics (financial data, entity linking, transcription). *Use case: Financial entity data, market analytics grounded in S&P sources.*
- 🤝 📡 [Pigment](https://www.pigment.com) - Business planning and forecasting platform. *Use case: Querying plans and forecasts, scenario analysis, pulling planning data into chat.*

### Analytics and Business Intelligence

- 🤝 📡 [Amplitude](https://amplitude.com) - Product analytics. *Use case: Querying product and event metrics, funnel and retention analysis in natural language.*
- 🤝 📡 [Hex](https://hex.tech) - Collaborative data notebooks and analytics. *Use case: Running and querying Hex projects, pulling analytics results into a thread.*
- 🤝 📡 [Vantage](https://www.vantage.sh) - Cloud cost observability and FinOps. *Use case: Cloud spend analysis, cost-anomaly detection, optimization queries.*

### Developer Platforms and Infrastructure

- 🤝 📡 ⭐ [GitHub](https://github.com) - Search repos, review issues, and manage pull requests. *Use case: Repository-wide code search, PR triage, generating commit messages from diffs.*
- 🤝 📡 [Cloudflare Developer Platform](https://developers.cloudflare.com) - Workers, Pages, and edge platform. *Use case: Edge deployment workflows, Workers debugging, configuration queries.*
- 🤝 📡 [Netlify](https://www.netlify.com) - Web build, deploy, and hosting platform. *Use case: Deploy status, build-log inspection, site configuration queries.*
- 🤝 📡 [Sentry](https://sentry.io) - Error monitoring and application observability. *Use case: Triaging production errors from chat, summarizing incident timelines, correlating issues with releases.*
- 🤝 📡 [Stytch](https://stytch.com) - Authentication and identity infrastructure. *Use case: Querying users and sessions, inspecting auth configuration, identity workflows.*

### Automation and Integration

- 🤝 📡 [Apify](https://apify.com) - Web scraping and automation actors. *Use case: Running scrapers, pulling structured web data into chat, automating extraction jobs.*
- 🤝 📡 [n8n](https://n8n.io) - Fair-code workflow automation. *Use case: Triggering and managing n8n workflows from a chat thread.*
- 🤝 📡 [Workato](https://www.workato.com) - Enterprise automation / iPaaS. *Use case: Orchestrating cross-app enterprise recipes and workflows.*
- 🤝 📡 [Zapier](https://zapier.com) - Workflow automation across 6,000+ apps. *Use case: Triggering and orchestrating cross-app workflows from a chat thread.*

### Research, Scientific and Public Data

- 🤝 📡 [BioRender](https://www.biorender.com) - Scientific figure and diagram creation. *Use case: Generating and finding scientific illustrations, figure assets for papers and posters.*
- 🤝 📡 [Data.gouv](https://www.data.gouv.fr) - French government open-data platform. *Use case: Querying French public datasets, citing official open data in research.*
- 🤝 📡 [PubMed](https://pubmed.ncbi.nlm.nih.gov) - NIH / NLM biomedical literature database. *Use case: Literature search, citation retrieval, grounding clinical and biomedical answers in primary sources.*
- 🤝 📡 [Scholar Gateway](https://www.wiley.com/en-us/research/scholar-gateway-connect-claude-mistral-ai/) - Wiley connector linking Le Chat to 1,300+ peer-reviewed journals with DOI-linked citations. *Use case: Literature reviews grounded in Wiley journals, verifiable citations with source metadata.*

### Content and Media Management

- 🤝 📡 [Bria](https://bria.ai) - Licensed, commercial-safe visual generative AI. *Use case: Generating and editing rights-cleared images for commercial use.*
- 🤝 📡 [Bright (Bright Data)](https://brightdata.com) - Web-data and scraping platform for live public web access. *Use case: Live web-data retrieval, large-scale public web access, grounding answers in fresh web content.*
- 🤝 📡 [Cloudinary](https://cloudinary.com) - Image and video media management and transformation. *Use case: Managing media assets, transformations, and delivery queries.*
- 🤝 📡 [Mermaid](https://www.mermaidchart.com) - Diagram-as-code authoring via Mermaid Chart. *Use case: Generating and editing flowcharts, sequence diagrams, and ER diagrams from natural language.*
- 🤝 📡 [Trivago](https://www.trivago.com) - Hotel and travel metasearch. *Use case: Hotel price comparison, travel research inline.*
- 🤝 📡 [Website Publisher (WebsitePublisher.ai)](https://www.websitepublisher.ai) - Build and publish full websites through conversation; 44+ MCP tools spanning pages, assets, dynamic entities, forms, and one-step publish to live URLs. OAuth 2.1 + dynamic client registration. *Use case: Building marketing sites, prototyping landing pages, managing CMS content, and publishing to production without leaving Le Chat. Joined the directory May 5, 2026.*

## Mistral Agents API

### Built-in Agent Tools

Built-in tools attachable to Agents via the [Conversations API](https://docs.mistral.ai/agents/conversations) or the [Agent SDK](https://docs.mistral.ai/agents/agents-and-conversations). Set on the `tools` array.

- 🅜 [Web Search](https://docs.mistral.ai/agents/tools#web-search) - Real-time web search with citations. Tool type `web_search` (free) and `web_search_premium` (higher rate limits). *Use case: Grounded answers from the live web, source-cited synthesis, research workflows.*
- 🅜 [Code Interpreter](https://docs.mistral.ai/agents/tools#code-interpreter) - Sandboxed Python execution with plotting and data analysis. Tool type `code_interpreter`. *Use case: Data crunching, generating charts, running analytical computations inside an Agent turn.*
- 🅜 [Image Generation](https://docs.mistral.ai/agents/tools#image-generation) - Generate images from a text prompt. Tool type `image_generation`. *Use case: Inline image creation during chat, prototype visuals, marketing-asset generation.*
- 🅜 [Document Library](https://docs.mistral.ai/agents/tools#document-library) - Built-in RAG over Mistral Cloud-hosted Libraries. Tool type `document_library` with `library_ids[]`. *Use case: Domain-grounded Q&A on uploaded corpora without building a custom retrieval stack.*

> **Connectors API (Public Preview, May 22, 2026)** — Le Chat connectors and custom MCP servers are exposed via the Conversations API, Completions API, and Agent SDK. Adds direct tool calling and human-in-the-loop approval flows. The June 24, 2026 update added API keys with connector scopes, multi-account connectors, a Connectors Debugger, Connectors in Vibe Code (GA), and Connectors in Workflows (Public Preview). Console: [console.mistral.ai/build/connectors](https://console.mistral.ai/build/connectors). Management: [docs.mistral.ai/capabilities/connectors/management](https://docs.mistral.ai/capabilities/connectors/management).

## Cloud Deployment

### Native Platform Partnerships

Not user-facing connectors — the cloud platforms where Mistral's models are deployable as managed services. Listed for completeness because Le Chat Enterprise is sold across these surfaces.

- 🤝 [Microsoft Azure (Azure AI / Foundry)](https://azure.microsoft.com/en-us/products/ai-foundry) - First MaaS launch (Mistral Large, Feb 2024); Mistral Large 3 added Dec 2025.
- 🤝 [AWS Bedrock](https://aws.amazon.com/bedrock/) - Managed serverless endpoints. GA March 2024.
- 🤝 [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) - Vertex AI Model Garden + Le Chat Enterprise listing on GCP Marketplace (May 2025).
- 🤝 [Snowflake Cortex](https://www.snowflake.com/en/data-cloud/cortex/) - LLM functions inside the data cloud (Mar 2024).
- 🤝 [IBM watsonx](https://www.ibm.com/products/watsonx-ai) - On-prem and watsonx.ai catalog deployment.
- 🤝 [NVIDIA](https://www.nvidia.com/en-us/ai/) - Inference partnership across NVIDIA platforms.
- 🤝 [Outscale](https://www.outscale.com) - French-sovereign cloud (Mistral's hometown / EU residency story).
- 🤝 [Dell Technologies AI Factory](https://www.dell.com/en-us/dt/ai-solutions/ai-factory.htm) - On-premises and enterprise-infrastructure deployment via Dell AI Factory with NVIDIA. Expanded collaboration announced May 18, 2026 at Dell Technologies World — Mistral's language and reasoning models plus orchestration tools brought to Dell PowerRack + NVIDIA GB200 NVL72 environments.

## Contributing

Contributions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md) for the submission flow, surface conventions, and the entry style guide. By contributing you agree to the [Code of Conduct](code-of-conduct.md).

The Le Chat connector directory is admin-visible inside Le Chat / Work under **Connectors → + Add Connector** and announcement-driven on [mistral.ai/news](https://mistral.ai/news). When new connectors land, submit a PR with the canonical vendor URL, the surface (Featured OAuth vs MCP directory vs Knowledge vs Custom MCP), the official category, and a specific use case.
