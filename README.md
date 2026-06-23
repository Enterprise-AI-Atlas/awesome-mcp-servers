# Awesome MCP Servers

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)

A curated, category-organized registry of [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) servers for AI agents, coding assistants, and MCP-compatible clients.

The goal is to be the definitive place to discover and install servers that let AI agents work with databases, cloud platforms, developer tools, SaaS apps, search engines, file systems, vector stores, and more.

**Inclusion criteria:** Resources must be MCP servers or clearly server-oriented registries. General SDK docs and tutorials are out of scope. See [CONTRIBUTING.md](./CONTRIBUTING.md) for the full quality bar.

> This list is part of a growing family of awesome-list registries. If you are working with Oracle products, also check out [Awesome Oracle Agentic Skills & MCP Servers](../awesome-oracle-agentic-skills-mcp) for Oracle-focused MCP servers and agent skills.

---

## Contents

- [Databases](#databases)
- [Cloud Providers](#cloud-providers)
- [Developer Tools](#developer-tools)
- [AI and LLM Platforms](#ai-and-llm-platforms)
- [Productivity](#productivity)
- [Communication](#communication)
- [Finance](#finance)
- [Search and Web](#search-and-web)
- [File Systems](#file-systems)
- [Memory and Knowledge](#memory-and-knowledge)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

---

## Databases

MCP servers for relational, document, key-value, vector, and analytics databases.

- **[PostgreSQL MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres)** `Official` — Read-only and read/write SQL queries with schema inspection.
  - Install: `npx -y @modelcontextprotocol/server-postgres postgresql://user:pass@host/db`
- **[SQLite MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite)** `Official` — Local SQLite database access and built-in analysis.
  - Install: `npx -y @modelcontextprotocol/server-sqlite /path/to/db.sqlite`
- **[MongoDB MCP Server](https://github.com/mongodb-labs/mongodb-mcp-server)** `Official` — Interact with MongoDB databases and MongoDB Atlas clusters.
- **[Redis MCP Server](https://github.com/redis/mcp-redis)** `Official` — Natural-language interface for managing and searching data in Redis.
  - Install: `uvx --from git+https://github.com/redis/mcp-redis.git redis-mcp-server --url redis://localhost:6379/0`
- **[MariaDB MCP Server](https://github.com/MariaDB/mcp)** `Official` — Manage and query MariaDB databases, with optional vector search.
- **[Elasticsearch MCP Server](https://github.com/elastic/mcp-server-elasticsearch)** `Official` — Query and analyze Elasticsearch indices through MCP. *(Superseded by the Elastic Agent Builder MCP endpoint in Elastic 9.2+.)*
- **[MCP Toolbox for Databases](https://github.com/googleapis/mcp-toolbox)** `Official` — Single open-source MCP server for PostgreSQL, MySQL, MongoDB, Redis, BigQuery, Snowflake, and more.
  - Install: `go install github.com/googleapis/mcp-toolbox@latest`

---

## Cloud Providers

Official and community MCP servers for major cloud platforms.

- **[AWS MCP Server](https://github.com/awslabs/mcp)** `Official` — Reference MCP servers for AWS docs, infrastructure, containers, serverless, and service-specific workflows. AWS also hosts a managed remote endpoint at `https://aws-mcp.us-east-1.api.aws/mcp`.
- **[Azure MCP Server](https://github.com/microsoft/mcp)** `Official` — Tools for Azure resource operations across 40+ services, usable from Copilot, VS Code, Claude, and more.
- **[Google Cloud MCP Server (gcloud)](https://github.com/googleapis/gcloud-mcp)** `Official` — Natural-language access to Google Cloud via the gcloud CLI and dedicated service servers.
- **[Cloudflare MCP Server](https://github.com/cloudflare/mcp)** `Official` — Token-efficient, code-mode MCP server for the entire Cloudflare API.
  - Connect: `https://mcp.cloudflare.com/mcp`
- **[Oracle Cloud Infrastructure MCP Servers](https://github.com/oracle/mcp)** `Official` — Reference MCP servers for OCI Compute, Networking, Storage, Identity, Databases, and more.
- **[Vercel MCP Server](https://vercel.com/docs/agent-resources/vercel-mcp)** `Official` — Remote MCP server for managing Vercel projects and deployments.
  - Connect: `https://mcp.vercel.com`

---

## Developer Tools

MCP servers for version control, infrastructure, observability, and container workflows.

- **[GitHub MCP Server](https://github.com/github/github-mcp-server)** `Official` — Repository, issue, PR, code search, and workflow automation tools.
- **[Git MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/git)** `Official` — Read, search, and manipulate local Git repositories.
- **[GitLab MCP Server](https://github.com/jmrplens/gitlab-mcp-server)** `Community` — Open-source GitLab server with safe/read-only modes, self-hosted support, and 870+ dynamic actions.
  - Install: `docker pull ghcr.io/jmrplens/gitlab-mcp-server:latest`
- **[Docker Hub MCP Server](https://github.com/docker/hub-mcp)** `Official` — Search images and manage Docker Hub repositories.
- **[Kubernetes MCP Server](https://github.com/containers/kubernetes-mcp-server)** `Community` — Native Kubernetes and OpenShift operations via the Kubernetes API.
- **[Terraform MCP Server](https://github.com/hashicorp/terraform-mcp-server)** `Official` — Terraform Registry, HCP Terraform, and workspace management tools.
  - Install: `go install github.com/hashicorp/terraform-mcp-server/cmd/terraform-mcp-server@latest`
- **[Sentry MCP Server](https://github.com/getsentry/sentry-mcp)** `Official` — Debug issues and interact with Sentry from coding agents.
  - Install: `npx @sentry/mcp-server`

---

## AI and LLM Platforms

MCP servers for inference providers, model hubs, and AI services.

- **[Ollama MCP Server](https://github.com/jayluxferro/ollama-mcp)** `Community` — Expose your local Ollama API as MCP tools for chat, completion, and embeddings.
- **[Replicate MCP Server](https://replicate.com/docs/reference/mcp)** `Official` — Search and run models on Replicate through natural language.
  - Install: `npx replicate-mcp`
- **[Hugging Face MCP Server](https://github.com/huggingface/hf-mcp-server)** `Official` — Search models, datasets, Spaces, papers, and run Gradio apps on the Hugging Face Hub.
- **[Groq MCP Server](https://github.com/groq/groq-mcp-server)** `Official` — Fast inference, vision, TTS, STT, and batch processing through Groq.
  - Install: `uvx groq-mcp`
- **[Perplexity MCP Server](https://github.com/perplexityai/modelcontextprotocol)** `Official` — Real-time web search, reasoning, and research via Perplexity Sonar models.
  - Install: `npx -y @perplexity-ai/mcp-server`

---

## Productivity

MCP servers for notes, tasks, calendars, and project management.

- **[Notion MCP Server](https://github.com/makenotion/notion-mcp-server)** `Official` — Read and write Notion pages, databases, and blocks.
  - Install: `npx -y @notionhq/notion-mcp-server`
- **[Obsidian MCP Server](https://github.com/MarkusPfundstein/mcp-obsidian)** `Community` — Interact with an Obsidian vault via the Local REST API plugin.
  - Install: `uvx mcp-obsidian`
- **[Todoist MCP Server](https://github.com/Doist/todoist-ai)** `Official` — Task and project management through Todoist.
  - Connect: `https://ai.todoist.net/mcp`
- **[Trello MCP Server](https://github.com/delorenj/mcp-server-trello)** `Community` — Manage Trello boards, cards, lists, comments, and attachments.
  - Install: `npx -y @delorenj/mcp-server-trello`
- **[Asana MCP Server](https://developers.asana.com/docs/using-asanas-mcp-server)** `Official` — Read and write Asana tasks and projects through a remote MCP server.
  - Connect: `https://mcp.asana.com/v2/mcp`
- **[Google Calendar MCP Server](https://github.com/nspady/google-calendar-mcp)** `Community` — Create, update, search, and check availability across multiple Google Calendars.

---

## Communication

MCP servers for messaging, email, and team collaboration.

- **[Slack MCP Server](https://docs.slack.dev/ai/mcp-server)** `Official` — Search messages, send communications, manage canvases, and retrieve user profiles in Slack.
  - Connect: `https://mcp.slack.com/mcp`
- **[Discord Agent MCP](https://github.com/aj-geddes/discord-agent-mcp)** `Community` — Comprehensive Discord server management with 70+ tools.
  - Install: `git clone https://github.com/aj-geddes/discord-agent-mcp.git && npm install`
- **[Microsoft Teams MCP Server](https://github.com/floriscornel/teams-mcp)** `Community` — Teams and Microsoft Graph API access for chats, channels, messages, and files.
- **[Telegram MCP Server](https://github.com/dryeab/mcp-telegram)** `Community` — Read, send, search, and manage Telegram messages via MTProto.
  - Install: `uvx mcp-telegram`
- **[Twilio MCP Server](https://github.com/twilio/ai)** `Official` — Search Twilio documentation and API specifications.
  - Connect: `https://mcp.twilio.com/docs`
- **[Email MCP Server](https://github.com/pzanna/email_mcp)** `Community` — Read, send, search, and manage emails via IMAP/SMTP.

---

## Finance

MCP servers for payments, banking, trading, and market data.

- **[Stripe MCP Server](https://github.com/stripe/ai)** `Official` — Stripe API search, documentation retrieval, and payment operations.
  - Install: `npx -y @stripe/mcp --api-key=YOUR_STRIPE_SECRET_KEY`
- **[Plaid MCP Server](https://plaid.com/docs/resources/mcp/)** `Official` — Dashboard diagnostics and a local AI coding toolkit for Plaid-connected finance data.
- **[Alpaca MCP Server](https://github.com/alpacahq/alpaca-mcp-server)** `Official` — Natural-language stock, ETF, crypto, and options trading.
  - Install: `uvx alpaca-mcp-server`
- **[Yahoo Finance MCP Server](https://github.com/AgentX-ai/yahoo-finance-server)** `Community` — Stock quotes, financials, news, options, and historical data.
- **[CoinGecko MCP Server](https://docs.coingecko.com/docs/ai-agent-hub/mcp-server)** `Official` — Live crypto prices, market data, historical charts, and DeFi/NFT data.
  - Connect: `https://mcp.api.coingecko.com/mcp`
- **[PayPal MCP Server](https://github.com/paypal/paypal-mcp-server)** `Official` — PayPal API tools for payments, orders, and account operations.

---

## Search and Web

MCP servers for web scraping, browser automation, and search APIs.

- **[Puppeteer MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer)** `Official` — Browser automation for dynamic web pages.
- **[Fetch MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch)** `Official` — Web content fetching and conversion for efficient LLM usage.
- **[Brave Search MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search)** `Official` — Web search via the Brave Search API.
- **[Tavily MCP Server](https://github.com/tavily-ai/tavily-mcp)** `Official` — AI-focused web search and research.
- **[Exa MCP Server](https://github.com/exa-labs/exa-mcp-server)** `Official` — Neural search for web content and research.
- **[Firecrawl MCP Server](https://github.com/mendableai/firecrawl-mcp-server)** `Official` — Scrape and crawl websites into LLM-ready markdown.
- **[Playwright MCP Server](https://github.com/microsoft/playwright-mcp)** `Official` — Cross-browser automation and testing tools from Microsoft.
- **[SerpAPI MCP Server](https://github.com/serpapi/serpapi-mcp-server)** `Community` — Structured search results from Google and other engines via SerpAPI.

---

## File Systems

MCP servers for local and cloud file storage.

- **[Filesystem MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem)** `Official` — Secure local file operations with configurable access controls.
  - Install: `npx -y @modelcontextprotocol/server-filesystem /allowed/path`
- **[Google Workspace MCP Server](https://github.com/taylorwilsdon/google_workspace_mcp)** `Community` — Drive, Docs, Sheets, Slides, Gmail, Calendar, and more through one server.
  - Install: `uvx mcp-google-workspace`
- **[Dropbox MCP Server](https://github.com/ngs/dropbox-mcp-server)** `Community` — List, search, upload, download, and share Dropbox files and folders.
- **[OneDrive MCP Server](https://github.com/MrFixit96/onedrive-mcp-server)** `Community` — OneDrive file sharing and search via Microsoft Graph.
- **[S3 MCP Server](https://github.com/txn2/mcp-s3)** `Community` — Browse, read, write, and generate presigned URLs for S3 and S3-compatible storage.
- **[Cloud FS MCP Server](https://github.com/nogoo9/mcp-server-cloud-fs)** `Community` — Unified cloud file system over S3, Azure Blob, GCS, R2, MinIO, and more.

---

## Memory and Knowledge

MCP servers for vector stores, knowledge graphs, long-term memory, and knowledge bases.

- **[Memory MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/memory)** `Official` — Knowledge graph-based persistent memory system.
- **[Chroma MCP Server](https://github.com/chroma-core/chroma-mcp)** `Official` — Vector search, full-text search, and metadata filtering with Chroma.
  - Install: `uvx chroma-mcp`
- **[Pinecone MCP Server](https://github.com/pinecone-io/pinecone-mcp)** `Official` — Manage Pinecone indexes and query records with integrated inference.
  - Install: `npx -y @pinecone-database/mcp`
- **[Weaviate MCP Server](https://github.com/weaviate/mcp-server-weaviate)** `Official` — Built-in MCP server for Weaviate vector database queries and object management.
- **[Qdrant MCP Server](https://github.com/qdrant/mcp-server-qdrant)** `Official` — Semantic memory layer on top of the Qdrant vector search engine.
  - Install: `uvx mcp-server-qdrant`
- **[Mem0 MCP Server](https://docs.mem0.ai/platform/mem0-mcp)** `Official` — Cloud-hosted long-term memory with add, search, update, and delete tools.
  - Connect: `https://mcp.mem0.ai/mcp`
- **[Zotero MCP Server](https://github.com/cookjohn/zotero-mcp)** `Community` — Access and manage a Zotero research library, including full-text PDFs and citations.
- **[Atlassian Rovo MCP Server](https://github.com/atlassian/atlassian-mcp-server)** `Official` — Search and act on Confluence and Jira data through a remote MCP server.
  - Connect: `https://mcp.atlassian.com/v1/mcp`

---

## Related Awesome Lists

- [Awesome Oracle Agentic Skills & MCP Servers](../awesome-oracle-agentic-skills-mcp) — Oracle-focused agentic skills and MCP servers.

---

## Contributing

Read [CONTRIBUTING.md](./CONTRIBUTING.md) for the quality bar, entry format, and PR process.

---

## License

This list is released into the public domain under [CC0-1.0](./LICENSE).

## Need implementation help?

Enterprise AI Atlas is maintained by [Vibe Coding Agency](https://vibecodingagency.com). If your team needs support designing, building, or deploying production AI systems covered in this atlas, [get in touch](https://vibecodingagency.com).
