# FastMCP

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

FastMCP is the fast, Pythonic framework for building Model Context Protocol (MCP) servers, clients, and apps. Originally created by Jeremiah Lowin and maintained by PrefectHQ, FastMCP 1.0 was adopted into the official Anthropic MCP Python SDK in 2024, and the standalone FastMCP project (now at v3) remains the most widely used way to ship MCP servers in Python — the project reports powering roughly 70% of MCP servers across all languages. FastMCP turns ordinary Python functions into MCP tools, resources, prompts, and apps via decorators, auto-generates JSON Schemas from type hints, handles transport negotiation (stdio, Streamable HTTP, SSE), and ships first-class OAuth/OIDC authentication, server composition and proxying, OpenAPI/FastAPI import, a CLI for running and installing servers into Claude Desktop / Claude Code / Cursor / ChatGPT / Gemini CLI / Goose, middleware, lifespan management, elicitation, sampling, progress reporting, OpenTelemetry, and a client library and apps runtime for building interactive UIs rendered inside MCP host conversations.

**Areas:** MCP · Python · Framework · Open Source · AI Agents · Tools · Resources · Prompts · LLM · Anthropic · A2A

## FastMCP on APIs.io

Everything profiled for FastMCP is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/fastmcp/](https://apis.io/providers/fastmcp/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [FastMCP Server](https://apis.io/apis/fastmcp/fastmcp-server/) — The FastMCP Server is the Python entry point for exposing tools, resources, prompts, and apps to any Model Context Protocol client. Developers instantiate a…
- [FastMCP Client](https://apis.io/apis/fastmcp/fastmcp-client/) — The FastMCP Client is a Python client library for talking to any MCP server — local or remote — with full protocol coverage. It supports calling tools,…
- [FastMCP Apps](https://apis.io/apis/fastmcp/fastmcp-apps/) — FastMCP Apps is the framework's runtime for building interactive applications rendered directly inside MCP host conversations. Apps expose UI surfaces —…
- [FastMCP Authentication](https://apis.io/apis/fastmcp/fastmcp-auth/) — FastMCP ships a complete authentication and authorization layer for MCP servers. Servers can verify tokens, terminate OAuth flows directly, or proxy to an…
- [FastMCP OpenAPI and FastAPI Integration](https://apis.io/apis/fastmcp/fastmcp-openapi/) — FastMCP can generate an MCP server directly from an existing OpenAPI 3.x description or a FastAPI application, turning every HTTP operation into an MCP tool…
- [FastMCP CLI](https://apis.io/apis/fastmcp/fastmcp-cli/) — The FastMCP CLI is a developer command-line tool for running, inspecting, installing, and debugging MCP servers built with FastMCP. It can launch servers…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [fastmcp](https://apis.io/servers/fastmcp/fastmcp/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Fastmcp Domain Security](https://apis.io/security/fastmcp/fastmcp-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://gofastmcp.com)
- [Documentation](https://gofastmcp.com/getting-started/upgrading/from-fastmcp-2)
- [Getting started](https://gofastmcp.com/getting-started/welcome)
- [Changelog](https://gofastmcp.com/changelog)
- [GitHub](https://github.com/PrefectHQ)

## API Evangelist rating

**Kin Score 18.2** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.3 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 28.9 |
| Developer ergonomics | 42.9 |
| Access clarity | 0.0 |

**Agent readiness 5.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | platform (partial credit) |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | near-conformant (partial credit) |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 5.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/fastmcp/](https://apis.io/providers/fastmcp/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for FastMCP: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/fastmcp/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
