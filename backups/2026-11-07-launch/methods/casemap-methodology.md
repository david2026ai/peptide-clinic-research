# Casemap methodology — deep dive

**For:** David Dubov / Scale Your Marketing  
**Date:** 2026-10-21  
**Skill PR:** https://github.com/david2026ai/symos-skills/pull/1  
**Skill path:** `skills/casemap/` (`SKILL.md`, `METHODOLOGY.md`, `schema.yaml`, `maps/`, `canvas/TEMPLATE.md`)

---

## Pipeline

1. **Discover needs** — customer needs + industry value-adds (obvious *and* latent / non-obvious)  
2. **Select attributes** — 5–8 scored axes; each `traces_to` a named need or value-add  
3. **Score** — Us vs 2–4 face competitors on 1–5 (evidence-labeled)  
4. **Focus / Breaker** — where we win; what makes it hard to copy  
5. **Give-ups** — 3–7 things to stop investing in so resources concentrate on Focus  
6. **Persist + graphic** — `maps/<slug>.yaml` + Cursor Canvas (radar/bar + give-ups panel)

---

## Customer-need intake (first-class)

Agents must **analyze and input** what buyers (and where relevant end customers) need and pay for — before locking scored axes.

| Capture | Examples (home services / HVAC intake desk) |
|---|---|
| Jobs-to-be-done | Fill replace calendar without multi-pro races |
| Switching criteria | Escape Angi-class shared dumps |
| Must vs nice | Exclusive fill, consent certs, land-in-CRM = must |
| Willingness-to-pay | Prepaid exclusive rate-per-lead bands; cancel = stop top-up |
| **Latent / non-obvious** | After-hours form death; comfort-advisor close honesty (~25–35%); PE exit from third-party buy; intake minutes as scarce resource |

**Input paths:** (a) structured questions to David/operators · (b) research docs in this store · (c) write into YAML `customer_needs` / `industry_value_adds`.

Label each need `obvious` | `latent` | `non_obvious`. Latent needs can become scored axes when they discriminate. **Do not** ship a map that is only table-stakes (“price, quality, speed”) every vendor already claims.

---

## Industry value-adds

What the industry **rewards commercially** — distinct from supplier vanity.

**Customer-valued (home services):** exclusive fill · speed-to-contact · prepaid clarity · consent / Telephone Consumer Protection Act provenance · land-in-their-CRM · replacement-intent quality · price per booking · owned demand (latent differentiator).

**Supplier vanity (do not score):** Marketing Pro / field-service rebuild, “AI platform,” dashboard beauty.

---

## Differentiators

- Differentiator ≠ feature list  
- Map to scored attributes + breaker test (“if we removed X, would Focus collapse?”)  
- Moat honesty: peers already match (e.g. Modernize exclusive SKUs) vs hard to match (owned YouTube/geo exclusive cells + prepaid proof + land-in-their-CRM)

---

## Direct competitors

- **2–4 face only** on the graphic (prefer 2: Angi Pro, Modernize)  
- Separate tables: attach (ServiceTitan, Housecall Pro, Jobber) · adjacent / liquidity / substitutes  
- Face cards: business model, who they sell to, exclusive vs shared, trust scars, where they score 4–5  

---

## Give-ups (first-class)

Every map lists **3–7** explicit stop-investing items with *why* (`dilutes_focus` | `lose_to_specialist` | `not_icp` | `capital_trap` | `attach_not_face`) and a **reallocation** toward Focus/Breaker.

Home-services examples: Marketing Pro clone · wide 90-day offer menu · statewide spray without ZIP allowlists · storm-roof primary · Demand Operating System as day-1 blocker · PE owned-media HQ rebuild pitches · shared/cheap volume SKU.

---

## Graphics

YAML = source of truth. Canvas = graphic: Us + face on same 1–5 attributes; Focus/Breaker highlighted; **Give-ups side panel** (not on radar). Template: `skills/casemap/canvas/TEMPLATE.md`.

---

## Related in this store

- [`casemap-skill-brief.md`](casemap-skill-brief.md)  
- [`home-services-casemap-scores.md`](home-services-casemap-scores.md)  
- Seed: `skills/casemap/maps/home-services.yaml` in the skill repo  
