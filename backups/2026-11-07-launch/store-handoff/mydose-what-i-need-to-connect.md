# What this Cloud Agent needs to use MyDose

**Endpoint:** `https://mcp.mydose.ai/hub/mcp`  
**Date:** 2026-11-07 (America/New_York)

The URL alone is not enough. The hub returns 401 without a hub access token.

## Need one of these (prefer A)

### A — OAuth / sign-in bound to *this* Cloud Agent
1. In Studio: Settings → AI assistants → Cursor instructions.
2. In **this** Cursor Cloud Agent / MCP settings, add HTTP MCP server: `https://mcp.mydose.ai/hub/mcp`.
3. Complete MyDose consent for the right store.
4. Prefer start **read-only**, then reconnect with **full / Changes allowed** when writing brand kit/pages.
5. Confirm this agent can call MyDose tools (ask: “List the pages on my store”).

Studio showing “Cursor Connected” on desktop does **not** automatically give tools to a separate Cloud Agent run.

### B — Pasted hub key (if OAuth can’t attach to Cloud Agent)
1. Studio → AI assistants → create key (1–30 days; default 7).
2. Put it in **Cursor Secrets / MCP config for this agent** — **do not paste into chat**.
3. Tell the agent the secret name (e.g. `MYDOSE_MCP_TOKEN`) is ready; agent rechecks tools.

## Already have / not blocking
- Your Owner/Admin Studio login
- Dashboard “Cursor Connected” screenshot (proves MyDose-side approval for some Cursor client)
- Brand/audience plan drafts in this project

## Still do not send in chat
- Hub keys, passwords, payment details, or PHI
