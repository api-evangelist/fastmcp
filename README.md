# FastMCP (fastmcp)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

FastMCP is the fast, Pythonic framework for building Model Context Protocol (MCP) servers, clients, and apps. Originally created by Jeremiah Lowin and maintained by PrefectHQ, FastMCP 1.0 was adopted into the official Anthropic MCP Python SDK in 2024, and the standalone FastMCP project (now at v3) remains the most widely used way to ship MCP servers in Python — the project reports powering roughly 70% of MCP servers across all languages.

FastMCP turns ordinary Python functions into MCP tools, resources, prompts, and apps via decorators, auto-generates JSON Schemas from type hints, handles transport negotiation (stdio, Streamable HTTP, SSE), and ships first-class OAuth/OIDC authentication, server composition and proxying, OpenAPI/FastAPI import, a CLI for running and installing servers into Claude Desktop / Claude Code / Cursor / ChatGPT / Gemini CLI / Goose, middleware, lifespan management, elicitation, sampling, progress reporting, OpenTelemetry, and a client library and apps runtime for building interactive UIs rendered inside MCP host conversations.

**APIs.json:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/fastmcp/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Producing
- **Access:** 3rd-Party
- **Repo Type:** opensource (Tier 2 — Python library)
- **License:** Apache License 2.0
- **Language:** Python (>= 3.10)
- **Maintainer Org:** [PrefectHQ](https://github.com/PrefectHQ)
- **Original Author:** Jeremiah Lowin ([@jlowin](https://github.com/jlowin))
- **Anthropic Lineage:** FastMCP 1.0 was incorporated into the official [Model Context Protocol](https://github.com/modelcontextprotocol) Python SDK stewarded by Anthropic.

## Tags

- MCP
- Model Context Protocol
- Python
- Framework
- Open Source
- AI Agents
- Tools
- Resources
- Prompts
- LLMs
- Anthropic

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### FastMCP Server

The Python entry point for exposing tools, resources, prompts, and apps to any MCP client. Decorator-based registration, auto-generated schemas, dependency injection, middleware, lifespan management, context, structured logging, progress reporting, elicitation, authorization, component visibility, pagination, namespace transforms, and OpenTelemetry. Servers can be composed via mounting and proxying, and exposed over stdio, Streamable HTTP, or SSE transports.

**Docs:** [gofastmcp.com/servers/server](https://gofastmcp.com/servers/server)

### FastMCP Client

A Python client library for talking to any MCP server — local or remote — with full protocol coverage: calling tools, reading resources, getting prompts, declaring roots, monitoring progress, server logging, notifications, user elicitation, LLM sampling, and background tasks across stdio, Streamable HTTP, and SSE. Authentication via Bearer tokens, OAuth, and CIMD. A standalone `fastmcp-client` package is available when only the client is needed.

**Docs:** [gofastmcp.com/clients/client](https://gofastmcp.com/clients/client)

### FastMCP Apps

Runtime for building interactive applications rendered directly inside MCP host conversations: approval flows, choice pickers, form input, file uploads, plus prefab and low-level HTML/generative UIs.

**Docs:** [gofastmcp.com/apps/overview](https://gofastmcp.com/apps/overview)

### FastMCP Authentication

A complete authentication and authorization layer for MCP servers: token verification, OAuth Proxy, OIDC Proxy, multi-auth sources, remote OAuth, and a full OAuth server. Provider integrations include Auth0, AWS Cognito, Azure/Entra ID, GitHub, Google, Discord, Keycloak, OCI IAM, Supabase, WorkOS, AuthKit, Descope, PropelAuth, and Scalekit. Authorization integrations cover Permit.io and Eunomia.

**Docs:** [gofastmcp.com/servers/auth/authentication](https://gofastmcp.com/servers/auth/authentication)

### FastMCP OpenAPI and FastAPI Integration

Generate an MCP server directly from an existing OpenAPI 3.x description or a FastAPI application — every HTTP operation becomes an MCP tool with auto-generated schemas and validation. The fastest path from any existing REST API to an agent-callable MCP surface.

**Docs:** [gofastmcp.com/integrations/openapi](https://gofastmcp.com/integrations/openapi) · [gofastmcp.com/integrations/fastapi](https://gofastmcp.com/integrations/fastapi)

### FastMCP CLI

The developer CLI for running, inspecting, installing, and debugging FastMCP servers. One-line install into Claude Desktop, Claude Code, Cursor, ChatGPT, and Gemini CLI.

**Docs:** [gofastmcp.com/cli/overview](https://gofastmcp.com/cli/overview)

## Common Properties

- [Website](https://gofastmcp.com)
- [Quickstart](https://gofastmcp.com/getting-started/quickstart)
- [Installation](https://gofastmcp.com/getting-started/installation)
- [Changelog](https://gofastmcp.com/changelog)
- [FAQ](https://gofastmcp.com/more/faq)
- [GitHub Repository](https://github.com/PrefectHQ/fastmcp)
- [PyPI](https://pypi.org/project/fastmcp)
- [Discord](https://discord.gg/uu8dJCgttd)
- [HTTP Deployment](https://gofastmcp.com/deployment/http)
- [Prefect Horizon (managed)](https://gofastmcp.com/deployment/prefect-horizon)
- [Contributing](https://gofastmcp.com/development/contributing)
- [License (Apache 2.0)](https://github.com/PrefectHQ/fastmcp/blob/main/LICENSE)

## Install

```bash
uv pip install fastmcp
# or
pip install fastmcp
```

## Hello, FastMCP

```python
from fastmcp import FastMCP

mcp = FastMCP("demo")

@mcp.tool
def add(a: int, b: int) -> int:
    """Add two numbers."""
    return a + b

if __name__ == "__main__":
    mcp.run()
```

## Why This Profile

FastMCP is the de-facto Python implementation of the Model Context Protocol — the open protocol Anthropic introduced for connecting LLMs to tools and data. With FastMCP 1.0 having been absorbed into the official Anthropic-stewarded MCP Python SDK, and FastMCP 3.x continuing as the actively maintained framework powering most MCP servers in the wild, this catalog entry captures the full developer surface: server, client, apps, authentication, OpenAPI/FastAPI import, and CLI — plus deployment, integrations, and the broader ecosystem.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
