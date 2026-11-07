---
cursor:
  subagentId: "bc-eec4a59b-e93f-57ca-8f72-e582c1c0952b"
---

# MyDose connection confirmation check

**Time:** 2026-11-07 America/New_York  
**User evidence:** Screenshot of Studio → Settings → AI assistants shows **Cursor** Connected Nov 7, 2026 with tags “Changes allowed” and “Clinic tools”.

## This cloud agent (`bc-eec4a59b…`) recheck
| Check | Result |
| --- | --- |
| Dynamic tool namespaces matching mydose/studio/clinic | **None** |
| `POST https://mcp.mydose.ai/hub/mcp` without token | **401** hub access token required |
| App secrets for MyDose | **None** listed for workspace |

## Interpretation
MyDose dashboard connection to **Cursor** is confirmed on their side (user screenshot). That approval is **not yet visible as MCP tools inside this Cloud Agent run**. Likely the OAuth/connection is bound to a desktop/other Cursor client, not automatically inherited by this cloud session.

## Honest status to report
**Not confirmed for this agent.** User’s Studio UI shows Cursor connected; this agent still cannot list/call MyDose tools.
