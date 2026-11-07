# Casemap skill — how David uses it

**Date:** 2026-10-21  
**For:** David Dubov / Scale Your Marketing  
**Status:** First-party skill in GitHub (methodology recreation) — upgraded with needs intake, latent attributes, give-ups, graphics

---

## What it is

A **strong kickoff ritual** for every vertical / business project:

1. **Discover needs** — customer needs + industry value-adds (obvious *and* latent / non-obvious)
2. Name the venture and **who pays**
3. Pick **2–4 face competitors** (prefer 2; not attach partners)
4. Promote **5–8 discriminating attributes** from needs (`traces_to`); score **1–5** (Us / faces)
5. Name **Focus**, **Breaker**, and **Give-ups** (3–7 stop-investing items)
6. Persist `maps/<slug>.yaml` + `maps/<slug>.md`
7. Open a **Cursor Canvas** chart from the YAML (Focus highlight + give-ups side panel)

Deep dive: [`casemap-methodology.md`](casemap-methodology.md)

## Inspiration vs dependency

[casemap.lovable.app](https://casemap.lovable.app/) inspired the **shape** (attribute scores × us vs face competitors × parallel map). It is **password-gated third-party** — we do **not** scrape it, call it, or depend on it. The skill + YAML live in our GitHub.

## Where it lives

| Asset | Path |
|---|---|
| Skill | `skills/casemap/SKILL.md` in [david2026ai/symos-skills](https://github.com/david2026ai/symos-skills) |
| Methodology | `skills/casemap/METHODOLOGY.md` |
| Schema (v2) | `skills/casemap/schema.yaml` — includes `customer_needs`, `industry_value_adds`, `give_ups`, `differentiators` |
| Canvas template | `skills/casemap/canvas/TEMPLATE.md` |
| Seed map (home services) | `skills/casemap/maps/home-services.yaml` (+ `.md`) |
| Tiny viewer | `skills/casemap/viewer/index.html` |
| SymOS mirror | `skills/casemap/` in [Scale-Your-Marketing/symos](https://github.com/Scale-Your-Marketing/symos) (so session sync / agents discover it) |
| Registry | Listed in `skills/saas/SKILL.md` dashboard |

**PRs:**
- Primary skill: https://github.com/david2026ai/symos-skills/pull/1 (`cursor/casemap-skill-bcd8`)
- SymOS mirror: https://github.com/Scale-Your-Marketing/symos/pull/694 (`cursor/casemap-skill-pointer-bcd8`) — update only if pointer/docs drift

## Trigger phrases

`casemap` · `attribute map` · `customer needs` · `map competitors` · `where should we focus` · `give ups` · `latent attributes` · new vertical kickoff

## Seed: home-services

**Needs (HVAC intake desk):** exclusive fill, replacement intent, speed, prepaid clarity, land-in-CRM, consent provenance, price per booking — plus **latent:** after-hours form death, comfort-advisor close honesty, PE exit from third-party, Angi-burn trust, intake-minutes scarcity.

**Face:** Angi Pro, Modernize · **Attach:** ServiceTitan / Housecall Pro / Jobber (not face).  
**Focus:** exclusive fill → price per booking · **Breaker:** exclusive-only + owned YouTube/geo + prepaid.  
**Give-ups:** Marketing Pro clone, wide offer menu, statewide spray without ZIPs, storm-roof primary, Demand Operating System day-1 blocker, PE owned-media HQ pitches, shared/cheap volume SKU.

Scorecard: [`home-services-casemap-scores.md`](home-services-casemap-scores.md)

## When to re-run

New vertical · pivot · ICP change · new customer-need evidence · 90-day pilot evidence · face competitive set changes.
