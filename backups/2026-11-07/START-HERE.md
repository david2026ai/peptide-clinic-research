# START HERE — clinic research and conversation handoff

Prepared November 7, 2026; completed chat export merged after approximately 12:12 PM PST. This is a portable research/documentation snapshot, not production software or a clinical launch authorization.

## Read in this order
1. `handoff.md` — confirmed decisions, assumptions, findings, open gates and next work.
2. `chat/conversation.md`, `conversation.json` and `export-status.json` — complete supplied spoken snapshot with 143 chronological messages plus two confirmed widget/answer supplement records. All 141 indexed user/assistant messages recovered in full. Read exact timestamp/attachment limitations; two newer assistant updates have no exposed exact time. `decision-summary.md` remains explicitly non-verbatim.
3. `research/mydose/README.md`, `ARCHITECTURE-AND-MIGRATION.md`, `PORTABILITY.md`, `MCP-INVENTORY.md` and `integration-inventory.md`.
4. MyDose structured records: `integration-inventory.csv`, `mcp-inventory.csv`, `portability-inventory.csv`, `migration-economics.csv`, `economics-assumptions.json`; then `SOURCES.md`, `sources.json`, `source-access-log.json` and `sources/`.
5. `research/mydose/builder-comparison/research-notes.md`, `vendor-comparison.csv`, `sources.csv` and its official-source snapshots.
6. `research/branding/README.md`, `maps/clinic-brand-options.md`, `maps/clinic-brand-options.yaml`, `attribute-scores.csv`, `shortlist.csv`, `domain-checks.csv`, `evidence-register.csv`, `discarded-and-hold.csv`, `framework-source.json`. The YAML uses JSON notation, valid YAML 1.2.
7. `pages/README.md` and the two `.canvas.tsx` snapshots for the actual completed interactive reports; `links.json` for live Pages.
8. `alignment-protocol/ALIGNMENT.md` and `CURRENT.md` are proposed root-document contents for the parent-authorized importer, plus routine-status.json documenting saved configuration, not proof that a scheduled run or synchronization succeeded.

## Required response after reading
Report your understanding under Confirmed decisions / Evidence-backed findings / Hypotheses / Missing access or contracts / Proposed next steps. Explicitly acknowledge the snapshot/timestamp limitations and distinguish summary from verbatim text. Do not implement, deploy, install/connect MCPs, open accounts, contact vendors, buy domains or change clinical decisions. Do not edit unrelated repositories.

## Destination and layout
User selected the existing dedicated Cursor Origin repository: https://cursor.com/codebase/david-dubov/peptide-clinic . No GitHub backup or SYM-repository change is requested now.

Archive paths start at `backups/2026-11-07/`; extract at repository root only through the parent-authorized importer. No extra workspace/folder prefix, nested ZIPs or git checkout included. Never overwrite existing source code. Review path collisions and report them. The importer may create root `ALIGNMENT.md` and `docs/alignment/CURRENT.md` from the proposed contents after reading the latest remote state. Once committed, the dated snapshot is immutable; future current-state updates belong outside it.

## Integrity
`MANIFEST.json` and `SHA256SUMS.txt` describe snapshot payload files. The manifest and checksum file intentionally do not hash themselves or one another. `VALIDATION.json` is a derived validation result and is also excluded from that self-referential set. `provenance.json` records input-archive sizes/hashes and CRC tests.

No real PHI, credentials, card data, hidden instructions, reasoning, raw tool logs or CloudAgent transcript dumps are intentionally included. Private user-source repository links and public Page IDs are intentional provenance, not credentials.

Chat privacy note: three internal project-agent link targets were redacted, with visible labels retained. See chat/redaction-log.json. Other message text and Page/repository/source/file links are retained.
