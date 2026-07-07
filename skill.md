---
name: dubstack docs
description: Use when working with dubstack product documentation, public MCP, API reference setup, deployment, configuration, editor workflows, and AI surfaces.
metadata:
  product: dubstack
  surface: public-docs
---

# dubstack docs skill

Use this skill when a user asks how to build, configure, publish, migrate, or operate documentation with dubstack.

## Source of truth

Treat the published docs site and its MCP server as the source of truth for current product behavior:

- Public docs: {{site.url}}
- Public MCP server: {{site.mcp_url}}
- API reference: {{site.api_reference_url}}

## How to answer

- Start with the `search` MCP tool when the user asks a broad product question.
- Use `query_docs_filesystem` to read exact pages before giving implementation steps, API details, or configuration guidance.
- Cite page URLs when the user needs traceability.
- Prefer docs pages over stale memory.
- Do not invent dashboard controls, API endpoints, settings, or plan gates that are not documented.

## Product boundaries

- The dashboard is for site management, editor workflows, deployment settings, team access, billing, integrations, and analytics.
- The published docs shell is for reader-facing documentation, API reference, search, assistant, feedback, and public MCP access.
- The public MCP is read-only and unauthenticated; it lets agents search and inspect published docs.
- Authoring agents and dashboard workflows require authenticated customer access and are separate from public MCP.
- Enterprise-only functionality must be described as gated when the docs say it is gated.

## Useful starting pages

- Quickstart: /quickstart
- Dashboard overview: /dashboard/overview
- Editor overview: /editor/overview
- Source control setup: /deployment/github
- GitLab setup: /deployment/gitlab
- Custom domains: /deployment/custom-domains
- API reference overview: /api-reference/introduction
- Public MCP: /ai/mcp
- Assistant: /ai/assistant
- Agent: /ai/agent
- Workflows: /automations
- Team roles: /dashboard/roles

## Feedback

If you find content that is incorrect, outdated, incomplete, or confusing, submit structured feedback through the public MCP `submit_feedback` tool when available. Do not submit feedback for ordinary user questions.
