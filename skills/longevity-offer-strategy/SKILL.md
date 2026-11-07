---
name: longevity-offer-strategy
description: Plan, price and position a premium longevity telehealth membership (labs + clinician + optional compounded protocols), including casemap scoring against Function, Superpower, Lifeforce, AgelessRx and Fountain Life and unit economics from MyDose cost floors. Use whenever the user asks about longevity offers, membership pricing, what to sell, competitor positioning, unit economics, CAC payback, or re-running the casemap for the longevity clinic, even if they don't say "strategy".
---

# Longevity offer strategy

The clinic sells **the plan, not the vial**: a lab-first membership where a clinician reviews results and writes a 12-month plan, with prescriptions added only when clinically appropriate. Keep every recommendation tied to that.

## Workflow

1. **Refresh competitor facts.** Prices in this space move monthly (Function cut $499 to $365 in 2026). Search before quoting any rival price and date every figure.
2. **Run the casemap** (the `casemap` skill if available): needs first, 5–8 attributes traced to needs, Us vs 2 face rivals (default Lifeforce + AgelessRx), Focus, Breaker, 3–7 Give-ups. Score Us as `hypothesis` until pilot data exists.
3. **Always show the visual attribute map** in the chat as soon as scores exist: a parallel-scores line chart (Us + face rivals, 1–5, focus attributes highlighted, series told apart by line style as well as color), total-score tiles, and a Focus/Breaker card beside a Give-ups panel. The user wants to see the map every time the casemap runs, not only read the YAML.
4. **Price from cost floors, not suggestions.** Pull live floors from MyDose (`hub_catalog`, `list_lab_services`). MyDose suggested prices can be below cost in later phases (NAD+ month 2+ was $230 cost vs $229 suggested). Flag any price with < $50/mo margin.
5. **Model contribution per member** with the table in `references/unit-economics.md`. Show the assumptions, never a forecast.
6. **Name what we give up.** Cheapest-vial races, catalog breadth, peptide spectacle, outcome claims.

## Output

The visual attribute map first, then a short memo: the decision, a competitor table, the offer, a pricing table (cost floor / price / margin), contribution per member, payback at three CAC levels, and open questions for MyDose.

## Guardrails

- Never present Us scores or CAC as measured.
- Do not recommend products outside the regulatory status the `longevity-claims-guard` skill allows.
- Medical decisions belong to the clinician; the offer may promise a review, not a prescription.
