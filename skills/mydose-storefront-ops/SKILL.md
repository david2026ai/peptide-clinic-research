---
name: mydose-storefront-ops
description: Operate a MyDose Studio storefront through the MyDose MCP connector — read the catalog and cost floors, check margins, list lab services, set brand kit, listings, prices and discounts, and handle confirmation-required actions safely. Use whenever the user mentions MyDose, the storefront, listings, the brand kit, pricing a package, or going live.
---

# MyDose storefront ops

## Read first (safe)

- `hub_overview` → store id, setup steps still open.
- `hub_catalog(storeId)` → offered packages, `costFloorUsd` per pricing phase, suggested price.
- `clinic_invoke_operation("list_services", {view:"summary"})` → every service on the clinic account (more than the storefront offers).
- `clinic_invoke_operation("list_lab_services")` → lab kits and prices.

## Margin check (always before pricing)

For each package and every phase: margin = price − phase cost. Flag phases under $50/mo or negative (NAD+ month 2+ and late-phase GLP-1s have been negative at suggested price).

## Writes

- Brand kit (`hub_save_brand_kit`), listings (`hub_save_listing`), discounts: describe the change and get the user's yes in chat before calling.
- Destructive commands (go-live, refunds, cancellations, publishing, deletions) return `confirmation_required`: show the summary verbatim, wait for an explicit yes, then resend with the same arguments plus `confirm_code`. Never self-confirm.
- Payment, payouts and signup happen through the interactive links the tools return; never collect credentials in chat.

## Data care

Clinic tools reach protected health information. Fetch only what the task needs; never pull patient lists for marketing.
