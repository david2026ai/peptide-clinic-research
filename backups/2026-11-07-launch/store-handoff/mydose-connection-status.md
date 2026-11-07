# MyDose connection status (this cloud agent)

**Checked:** 2026-11-07 America/New_York

## What we see from this session
- **No MyDose MCP namespace** is registered among this agent’s dynamic tools.
- Direct probe of `https://mcp.mydose.ai/hub/mcp` returns **401**: *“A hub access token is required. Sign in through the MyDose hub.”*
- Browser login subagent for Studio UI is **running separately**; that is not the same as MCP tools on this agent.

## How to connect Cursor (official docs)
From [Build with an AI assistant](https://docs.mydose.ai/studio/build-with-ai):

1. In Studio dashboard → **Settings → AI assistants**.
2. Choose **Cursor**.
3. Add MCP server URL: `https://mcp.mydose.ai/hub/mcp`
4. Sign in / approve store access (start **read-only**, then full when writing pages).
5. Or create a **pasted key** (1–30 days, default 7) on that page — treat like a password; **do not paste into chat**. Prefer Cursor Secrets / MCP OAuth UI.

## After connect works
Ask: “List the pages on my store.” Then we can set brand kit (Plainvero draft), colors, and non-PHI pages.
