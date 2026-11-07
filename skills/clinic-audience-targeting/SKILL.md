---
name: clinic-audience-targeting
description: Use when designing Meta or Google/YouTube audiences, exclusions, geo/age settings, lead forms, or measurement for clinic ads—LegitScript-aware, privacy-safe, no patient-list targeting.
metadata:
  version: 0.1.0-draft
  refreshed: 2026-11-07
---
# Clinic audience & measurement targeting

Read `../../AGENTS.md`, `references/privacy-measurement.md`, `clinic-legitscript-ads-gate`, Meta/Google filters. Default launch posture is conservative (HOUSE). Law/platform terms can be stricter; counsel owns legal applicability.

## Segment model first
Use attribute-map / CaseMap:
- **Beachhead (recommended research default):** US adult cash-pay weight-care clarity seekers
- Expand to menopause/TRT only after remap + clinical capacity
- Never make experimental-peptide seekers the master paid ICP

Value / Deliver / Give-up must match creatives and landing pages.

## Meta targeting floors (Rx path)
When ads promote prescription drugs (after LS + Meta auth):
- Countries: US / Canada / NZ only; only where certified
- Age: **18+**
- No targeting under 18 for Rx
Weight-loss / cosmetic / dietary health ads also require 18+ under Health & Wellness.

General telehealth service ads: still avoid personal-attribute copy; apply adult targeting when weight/sexual/reproductive context applies.

## Google / paid YouTube — sensitive health personalization
Source: [Health in personalized advertising](https://support.google.com/adspolicy/answer/16701855?hl=en) (refreshed 2026-11-07).

**Cannot use advertiser-curated audiences** for sensitive health categories (includes chronic conditions, sexual/fertility, intimate body functions, invasive procedures/injections):
- Customer Match
- Your data / remarketing segments
- Audience expansion
- Lookalike segments

**Can use** (subject to other policies): predefined Google audiences (in-market, affinity, life events, many demographics), location (not a substitute for clinical patient-location checks).

Custom segments with sensitive creative/landing pages: Display may serve only to non-sensitive/contextual; other campaigns often ineligible—verify current footnote 4 on policy page.

## HOUSE default matrix (launch)
| Tactic | Stance | Why |
|---|---|---|
| Geo + age + language matching licensed states | Allowed after ops proof | Clinical coverage gate |
| Interest / contextual / Search intent keywords (non-restricted) | Conditional | Platform drug-term + claims filters |
| Predefined Google in-market/affinity | Conditional | Sensitive-category rules |
| Public-page engagement retargeting (non-PHI marketing site) | Conditional after privacy review | No portal/intake pixels |
| Patient CRM / EHR list upload | BLOCKED | PHI / sensitive health |
| Health lookalikes / condition-page retargeting | BLOCKED | HOUSE + often PLATFORM |
| Portal / checkout / intake pixels + CAPI purchase | BLOCKED | MyDose Studio: no signup/purchase/patient events to ads; privacy |
| Lead form with diagnosis/symptom PHI questions | BLOCKED | HOUSE |
| Aggregate spend / public-page reporting | Allowed | Preferred measurement |

## Lead forms & landing
- Minimal fields; no quiz diagnosis; no “guaranteed eligibility”
- Secure clinical intake on **separate origin** after marketing CTA
- State availability honest; no 50-state claim without proof
- Match CaseMap Focus: show cost components and next steps on landing

## Measurement plan template
Event | Destination | Identifiers | Allowed? | Approver
---|---|---|---|---
(fill per campaign)

No bland event rename to hide health context. Hashing ≠ deidentification clearance.

## Output
Audience blueprint, exclusion list policy, geo/age, form fields, measurement matrix, open privacy/counsel items. Mark overall BLOCKED if Rx ads planned without LS + platform certs.
