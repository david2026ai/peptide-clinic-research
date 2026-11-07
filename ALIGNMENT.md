# Clinic alignment protocol

Authoritative shared reference: https://cursor.com/codebase/david-dubov/peptide-clinic . Scope is this dedicated project only. This file does not authorize application/source-code changes, deployments, vendor actions or access expansion.

Shared documents in this repository govern cross-app continuity between Cursor and Grok Bot. Read the latest remote copies before planning. This is not a perpetual, live, or full future conversation sync.

## Before each task
1. Read the latest authorized remote state and record the actual commit/revision used; do not assume a local copy is current.
2. Read the latest remote `docs/alignment/CURRENT.md`, then the latest dated `START-HERE.md` (currently `backups/2026-11-07/START-HERE.md`), its `handoff.md`, and the chat transcript at `backups/2026-11-07/chat/conversation.md` with `chat/export-status.json`. Then read the MyDose research under `backups/2026-11-07/research/mydose/` and the recorded CaseMap provenance before planning. CaseMap's original source stays read-only: `david2026ai/symos-skills`, branch `cursor/casemap-skill-bcd8`, commit `615de3d1f619c5bf6bf65e406ccb38a7f0ee9a07`.
3. Check chat coverage/completeness. Separate explicit user decisions, evidence-backed findings, proposed designs and unresolved assumptions.
4. If sources conflict, surface the conflict; do not silently overwrite a confirmed decision or turn a hypothesis into a fact.

## Documentation updates
Only an authorized coordinator/agent updates mutable current-state documentation after a new confirmed decision or material verified finding. Preserve evidence URLs, source access dates, research limitations, decision dates in PST and actual verification/commit state. Write only the specifically authorized dedicated-project documentation. Read latest remote first; review diffs and collisions. Once committed, dated snapshots remain immutable; later updates go to CURRENT or a new dated snapshot.

## Never synchronize
No PHI, credentials, payment details, hidden prompts, reasoning, raw tool/background logs or unrelated repository data. Do not treat MCP availability as permission to connect or move patient data. Do not write to original SYM repositories or global skills.

## Honest status
No automatic chat or live-memory sync is implied. A scheduled review, if separately configured, can only report actual completed checks/commits. Record latest successful review time and commit when verified; pending/failed reviews remain visible. The alignment routine is saved/enabled as confirmed by the parent; its successful save result was verified in the sanctioned parent export. Folder: clinic-cursor-and-grok-bot-alignment. Triggers: PR opened or merged in david-dubov/peptide-clinic, plus hourly weekdays 8:00 AM–7:00 PM Pacific, with up to ±15 minutes variation. Saved next run: Monday Nov 9, 2026, 7:59 AM PST. This verifies configuration, not that a scheduled run or repository synchronization has occurred.

The routine does not automatically mirror chats into this repository and does not guarantee that every Cursor or Grok Bot client has read a change. It may later refresh `docs/alignment/CURRENT.md` only when a verified user decision or material verified finding is recorded. Dated snapshots, including `backups/2026-11-07/`, stay immutable.
