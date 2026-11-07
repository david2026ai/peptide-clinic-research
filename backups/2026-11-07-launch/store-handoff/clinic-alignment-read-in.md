---
cursor:
  subagentId: "bc-eec4a59b-e93f-57ca-8f72-e582c1c0952b"
---

# Clinic alignment — read-in summary (no implementation)

**Date:** 2026-11-07 (America/New_York)  
**Repo HEAD read:** Origin `david-dubov/peptide-clinic` `d3ea59f` (*Add November 7 clinic research snapshot*)  
**Constraint:** Read-only. CaseMap provenance read-only. No brand/niche/vendor selected. No other-repo writes. Snapshot ≠ live chat sync.

## Sources read (order)

1. `/agent/repos/peptide-clinic/ALIGNMENT.md`
2. `/agent/repos/peptide-clinic/docs/alignment/CURRENT.md`
3. `/agent/repos/peptide-clinic/backups/2026-11-07/START-HERE.md`
4. `/agent/repos/peptide-clinic/backups/2026-11-07/handoff.md`
5. `/agent/repos/peptide-clinic/backups/2026-11-07/chat/conversation.md` (start + decision-summary) + `chat/export-status.json` + `chat/decision-summary.md`
6. `/agent/repos/peptide-clinic/backups/2026-11-07/research/mydose/README.md` + `ARCHITECTURE-AND-MIGRATION.md` + `economics-assumptions.json` (referenced core research)
7. `/agent/repos/peptide-clinic/backups/2026-11-07/research/branding/README.md` + `maps/clinic-brand-options.md` + `shortlist.csv` + `domain-checks.csv`

**Snapshot limits (acknowledge):** Chat = dated export, not future sync. 143 spoken + 2 widget supplements; 141 indexed messages full; start Nov 6 1:14:53.359 PM PST; last exact ts Nov 7 12:07:18.230 PM PST; export ~12:12 PM PST; two later assistant updates without exact times. Three internal agent-link targets redacted. `decision-summary.md` is **not** verbatim.

---

## Goals

1. Explore standing up a **US cash-pay** hormone/peptide-adjacent clinic (research/planning only).
2. Diligence **Hedonic** offer/catalog, then **MyDose** as possible first clinical storefront, with owned brand/marketing and exit/portability thinking.
3. Apply user’s **CaseMap** skill to branding shortlist (decision-clarity position)—without selecting a name/niche.
4. Keep work in dedicated Origin **`david-dubov/peptide-clinic`**; keep existing **SYM GitHub / global skills read-only**.
5. Align Cursor ↔ Grok via shared `ALIGNMENT.md` / `docs/alignment/CURRENT.md` (documented protocol; **not** automatic chat sync).

---

## Confirmed decisions

| Decision | Source |
| --- | --- |
| Destination = this Origin clinic repo (not GitHub / not SYM) | CURRENT, handoff, START-HERE |
| Research/planning only — no launch, implementation, MCP connect, purchases, domain buys, vendor outreach, publication | CURRENT, handoff |
| Existing SYM repos + shared skills **read-only** | ALIGNMENT, CURRENT, conversation |
| **No** final brand, niche, clinical partner, pharmacy, state footprint, or business model selected | CURRENT, handoff |
| **No vendor selected** (MyDose/Hedonic remain unevaluated-to-pick) | CURRENT |
| Economics assumptions ≠ proven performance | CURRENT |
| CaseMap provenance locked read-only: `david2026ai/symos-skills` @ `cursor/casemap-skill-bcd8` / `615de3d1…` | ALIGNMENT, CURRENT, branding |
| Dated `backups/2026-11-07/` immutable; future locks → `docs/alignment/CURRENT.md` | ALIGNMENT |
| Alignment routine **config** verified (folder clinic-cursor-and-grok-bot-alignment; PR + weekday hourly PT); successful scheduled sync **not** observed | CURRENT |

---

## Evidence-backed findings (not decisions)

- **MyDose Studio public tariff:** $499/mo incl. 50 active + $15/extra; free until first live purchase; pass-throughs (meds/consults/labs/Rx/shipping/processing) unpublished.
- Export rights, price-control scope, MSA/BAA, clinical custody, payment/subscription portability, partner continuity → need contracts + synthetic acceptance.
- Auto-migrate at patient 51 **not** justified; negotiate caps; illustrative lean leave-breakeven **626** actives / 24 mo (assumptions).
- Named public refs: Stripe Connect, NVP Medical Group P.A.; historical NewLife / WorkOS; Studio limits (no SMS sequences, no Studio care-message reply, no signup/purchase events to ads).
- Inventories preserved: 29 integrations, 19 MCP/service rows, 18 portability groups; MCP docs ≠ permission to connect.
- **Branding CaseMap:** weight scenario vs Ro/Mochi only (not niche lock). Candidate Focus = personal decision receipt; **no Tier-1 Breaker**. Leads: Plainvero / Rillstead / Clearbyline. RDAP “not found” ≠ registrar-available; exact `rillstead.com` / `clearbyline.com` registered. No USPTO candidate sets / trademark clearance.
- Hedonic Pages remain linked context (offer diligence / catalog strategy)—not executed SOW.

---

## Assumptions / hypotheses (unverified)

- US adult cash-pay planning frame.
- Conditional **MyDose-first** MVP recommendation if gates pass; own brand/domain/content day one.
- Brand position = understandable costs/decisions/next steps—not superior medicine.
- Illustrative replacement costs ($60k / $3.5k / $5 / 24 mo) and all Us CaseMap scores = targets, not measured.
- Owned frontend + retained MyDose backend does **not** remove MyDose fees.
- Repository name / peptide interest ≠ authorization for experimental-peptide treatment launch.

---

## Unresolved choices

1. Launch **niche** (weight vs menopause vs TRT vs other)—CaseMap weight map is scenario-only; menopause was a prior catalog hypothesis, not a mandate.
2. **Name** territory → lead + backup; registrar quotes; counsel clearance; no-PHI recall tests.
3. Clinical entity / partner / states / ownership (PC/MSO) design.
4. Vendor path: MyDose vs Hedonic stack vs alternatives (Beluga etc.)—contract/export/price-control answers first.
5. Whether/when to fund owned frontend or migration; volume-cap negotiation.
6. Formulary / compounding / advertising eligibility per product (esp. peptides)—HOLD experimental revenue until independent clearance.
7. Post-snapshot work (e.g. Telegra diligence in Project store) is **outside** this immutable backup; not a CURRENT decision unless later recorded.

---

## Proposed next steps (authorized planning only — not implementation)

Per handoff / CURRENT open work; await explicit authorization before any of these become actions beyond docs:

1. Check `docs/alignment/CURRENT.md` before each task; record only **approved** decisions there.
2. Narrow naming territory (still no purchase).
3. Choose segment only after partner/legal/unit-econ gates; request MyDose MSA/BAA/export/price-control packet.
4. Replace migration assumptions with signed rates before any build/move.
5. Do **not** implement, deploy, connect MCPs, contact vendors, buy domains, or modify other repositories.

## CaseMap / read-only constraints (followed)

- Framework source commit `615de3d1…` treated as immutable provenance.
- SYM / global skills not written.
- No brand/niche/vendor treated as selected despite research recommendations.
