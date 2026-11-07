---
name: clinic-legitscript-ads-gate
description: Use before planning or launching Meta, Google Ads, or paid YouTube for US telehealth/prescription services—LegitScript healthcare certification, platform authorizations, product eligibility, and go/no-go gates.
metadata:
  version: 0.1.0-draft
  refreshed: 2026-11-07
---
# Clinic LegitScript + ads gate

Read `../../AGENTS.md`, `../../SOURCES.md`, clinical-claims filter, Meta filter, Google/YouTube filter, and privacy reference first. This skill decides whether paid acquisition is even eligible—not creative taste. Internal PASS is not platform approval. Refresh primary sources on every substantive audit (access date required).

## Core truth
**LegitScript certification ≠ Meta approval ≠ Google approval ≠ creative clearance.**  
Certification is a driver’s license; each platform still enforces its own traffic laws. LS cannot predict, interpret, or appeal platform ad decisions ([LS FAQ](https://www.legitscript.com/certification/faq/)).

## Step 1 — Classify the advertiser and destination
Record: legal entity, root domain(s), telemedicine vs online pharmacy vs manufacturer, states served, clinical partner/pharmacy affiliates, exact products (approved / compounded / off-label / unapproved), and whether ads or landing pages **promote prescription drugs** vs **general telehealth services**.

Product tracks stay separate: weight (GLP-1), TRT, menopause, experimental peptides. A supplier menu is not ad eligibility.

## Step 2 — LegitScript Healthcare Certification [GUIDANCE → PLATFORM input]
For US online prescribing / telemedicine facilitation:
1. Apply Healthcare Certification **per root domain** (subdomains usually covered; new root = new fee) — [LS FAQ pricing](https://www.legitscript.com/certification/faq/).
2. Affiliates/pharmacies: LS checklist expects partner pharmacies certified or NABP-equivalent paths; unverified partners can block or jeopardize certification.
3. Expedite option exists (LS FAQ: additional fee starts review within two business days)—does **not** shorten compliance review itself.
4. After certify: public verification `https://www.legitscript.com/websites/<domain>`; place seal linking to verification page ([LS welcome](https://www.legitscript.com/certification/healthcare-certification/welcome-to-legitscript-certification/)).
5. Notify LS if services/ownership/sites change; renew annually.

**BLOCKED** for prescription-drug paid paths until live verification URL exists for the **actual advertised domain**. Builder/vendor “we’re certified” does not certify your brand domain.

## Step 3 — Meta pathway [PLATFORM]
Source refreshed 2026-11-07: [Drugs & Pharmaceuticals](https://transparency.meta.com/policies/ad-standards/restricted-goods-services/drugs-pharmaceuticals), [Health & Wellness](https://transparency.meta.com/policies/ad-standards/restricted-goods-services/health-wellness/).

| Ad type | LegitScript + Meta auth? | Targeting floor |
|---|---|---|
| Promote **telehealth services generally** | Written authorization **not** required per Meta Rx policy text | Still follow Health/Wellness, Personal Attributes, adult rules where applicable |
| Promote **prescription drugs** | Active LS (telehealth/pharmacy) **or** manufacturer internal review; Meta onboarding/authorization; consult-professional / valid-prescription disclaimer | US/Canada/NZ only; only countries of certification; **18+** |
| Unsafe / illicit / unapproved substances as Meta determines | Disallowed | — |

Also: weight-loss/cosmetic ads → 18+; no appearance inferiority, fat-pinching shock, cure claims for listed incurable diseases, clickbait outcome timelines without qualifiers. Rx weight-loss products → Drugs & Pharmaceuticals path, not only Health & Wellness.

Onboard: Business Settings → Authorizations → Prescription Drug Ads; classification Online Pharmacy / Telemedicine / Manufacturer; submit **certified website URL** (not only LS verification link) — per LS partner guidance.

## Step 4 — Google Ads / paid YouTube pathway [PLATFORM]
Source refreshed 2026-11-07: [Healthcare & medicines](https://support.google.com/adspolicy/answer/176031?hl=en), [Health in personalized advertising](https://support.google.com/adspolicy/answer/16701855?hl=en).

US table (telemedicine):
- Google allows telemedicine providers accredited by **LegitScript Healthcare Merchant Certification** (telemedicine certification for virtual care + facilitated prescribing).
- Online pharmacies: LS **or** NABP digital/.pharmacy paths.
- **Advertisers must also be certified with Google** (separate healthcare certification application).
- Restricted prescription-drug terms in ads/keywords/destinations unless location table allows.
- Speculative/experimental treatments generally disallowed; unapproved pharmaceuticals/supplements lists apply. DHEA US exception ≠ peptide free-for-all.
- Google errs cautious when landing pages appear to facilitate online prescribing—even “education” destinations can pull the service into scope.

Paid YouTube = Google Ads policy. Organic YouTube Community Guidelines / advertiser-friendly monetization are **separate** reviews.

## Step 5 — What can actually run (practical matrix)
Label each row PASS path / HOLD / BLOCKED for **this** clinic’s current domain+products (update when evidence changes).

| Creative / offer pattern | Meta | Google/YouTube paid | Notes |
|---|---|---|---|
| General telehealth evaluation / “how care works” (no drug promo) | Possible without Rx auth | May still need Google healthcare cert if destination facilitates online Rx | Destination decides scope |
| Named FDA-approved GLP-1 + telehealth | Needs LS + Meta Rx auth + disclaimer + 18+/geo | Needs LS + Google cert; drug-term rules | Strongest competitor pattern |
| Compounded sema/tirz as hero offer | High risk / often HOLD | Experimental/unapproved gates; HOLD | Catalog research HOLD |
| Experimental peptides / RUO / research-chemical framing | BLOCKED as unsafe/unapproved path | BLOCKED speculative/unapproved | Never “education” cloak to checkout |
| TRT / menopause service (no specific controlled-substance promo) | Service vs Rx classification required | Same; controlled-substance extras | Remap CaseMap; counsel |
| Before/after weight transformations | Meta allows some cosmetic B/A 18+; Rx weight → Drugs policy; HOUSE default no medical WL B/A until review | Misleading transformations risk | Prefer process/education |
| Patient-list / health lookalike / portal pixel | HOUSE BLOCKED | Advertiser-curated audiences blocked for sensitive health | See audience skill |

## Step 6 — Gate output
Deliver: domain LS status URL, Meta auth status, Google cert status, product eligibility table, creative class allowed, remaining counsel/clinical decisions. Use `../../templates/audit-report.md` taxonomy. Never write “ready to launch ads” without live certifications + human publication authorization.

## Sources to reopen every audit
- https://www.legitscript.com/certification/faq/
- https://www.legitscript.com/certification/healthcare-certification/welcome-to-legitscript-certification/
- https://transparency.meta.com/policies/ad-standards/restricted-goods-services/drugs-pharmaceuticals
- https://transparency.meta.com/policies/ad-standards/restricted-goods-services/health-wellness/
- https://support.google.com/adspolicy/answer/176031?hl=en
- https://support.google.com/adspolicy/answer/16701855?hl=en
- Linked Google “Apply for healthcare certification” form from current policy page
