# Peptide clinic repo — Agent SDK orient

**Date:** 2026-11-07  
**Repo:** `origin.cursor.com/git/david-dubov/peptide-clinic` (`david-dubov/peptide-clinic` on Origin)  
**Checkout:** `/workspace` (env default) and `/workspace/repos/peptide-clinic` (explicit clone)  
**HEAD:** `2ac26a661f13a5a7a1c771d3a1171dfaa01d2af7` — *Add draft clinic marketing research pack* (2026-11-06)

---

## Verdict

**This Origin repo is not a Grok / Agent SDK mobile agent project.** It is the **Hormone & Peptide Clinic Marketing Pack** (draft v0.1): skills, templates, references, and exports for clinic marketing research/audits. There is no live agent to talk to from this checkout today.

| Expected (Agent SDK) | Actual |
| --- | --- |
| `bot/agent.ts`, `bot/instructions.md` | Missing |
| `package.json` / `@grok/agent-sdk` | Missing |
| `bot/channels/*` (Slack/mobile) | Missing |
| Hosted deploy slug | None in-repo; README says not deployed |
| `agent-sdk validate/info` | Fail: *No agent projects found… need bot/ (or flat-layout markers)* |

Only Origin repo visible to this run’s principal: **`david-dubov/peptide-clinic`**.

---

## What is in the repo

- **Entry/contract:** `AGENTS.md` (clinic marketing authoring rules — not Agent SDK agent entry)
- **Skills:** `skills/clinic-*` (strategy, landing copy, video, clinical claims, Meta, Google/YouTube)
- **Templates / references / exports:** audit, campaign brief, clinic-context, privacy, regulatory snapshot, strategy exports
- **Branches:** `main` only

Useful for Demand OS / peptide-clinic *marketing* work from this Project. Not a runnable bot.

---

## How you would talk to a live Agent SDK / mobile agent (once one exists)

Public docs: https://cursor.com/docs/bdk · Dashboard: https://cursor.com/dashboard/deployed-agents

1. **Auth (required for hosted status / sessions):** Cursor credential via `CURSOR_SERVICE_ACCOUNT_KEY`, `CURSOR_API_KEY` / `CURSOR_API_KEY_FILE`, or `npx --yes "@grok/agent-sdk@0.6.0" login` (operator-run; agents should not login unless asked).
2. **Discover deploy:**  
   `npx --yes "@grok/agent-sdk@0.6.0" deployment list --json --fields slug,status --limit 50`  
   then `deployment get <slug> --json --fields status,lastError`
3. **Message hosted agent:**  
   `npx --yes "@grok/agent-sdk@0.6.0" session create --slug <slug> --message "…" --wait`  
   inspect with `session get <ses_…> --prod`
4. **Local playground (dev):** from a real agent dir with `bot/`:  
   `npx --yes "@grok/agent-sdk@0.6.0" dev ./<slug>` → open printed playground URL
5. **Cursor IDE MCP:** `npx --yes "@grok/agent-sdk@0.6.0" mcp install --url <agent-base-url>` (needs running agent + token as applicable)
6. **Mobile / Grok surface:** hosted agents appear under Cursor’s deployed-agents dashboard after a successful `deploy`; first deploy prints a one-time **alias token** (operator saves privately — never paste into chat). Slack is optional (`bot/channels` + slack skill), not present here.

---

## Current run / deploy status (this environment)

| Check | Result |
| --- | --- |
| Env linked repo | `origin.cursor.com/git/david-dubov/peptide-clinic` |
| Env builds | `no_finished_builds` (default image fallback) |
| `CURSOR_SERVICE_ACCOUNT_KEY` / `CURSOR_API_KEY` | **Absent** |
| `agent-sdk whoami` / `deployment list` | **Unauthenticated** — cannot see team deploys or sessions |
| In-repo deploy config | None |
| Secrets invented | None |

---

## Blockers / decisions for David

1. **Wrong artifact type** — Origin `peptide-clinic` holds the marketing pack, not an Agent SDK bot. Either point this Project at the real Grok/Agent SDK repo (if it lives elsewhere / not yet created), or scaffold one (`agent-sdk init` / create-agent skill) and deploy.
2. **CLI auth** — Attach a Cursor service account or operator `agent-sdk login` before anyone can list deploys or message a hosted agent from this VM.
3. **Do not treat marketing-pack PASS as agent clearance** — pack `AGENTS.md` forbids publication/spend/account access by default.

---

## Next useful moves (when authorized)

- Confirm whether a separate Agent SDK repo/slug already exists under another namespace, or scaffold under this Origin remote.
- After a real `bot/` project exists: `validate` → dry-run `deploy` → operator-run first deploy → `session create` smoke.
- Keep this marketing pack as content source for clinic claims/copy skills the agent may load — not as the agent runtime itself.
