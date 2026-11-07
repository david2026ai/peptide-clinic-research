# US clinic website and funnel builder research

Accessed **November 7, 2026 (PST; America/Los_Angeles)**. Research only. Eight exact vendor/offerings; primary-source evidence, not authenticated product testing or signed-contract validation. No accounts connected, forms submitted, outreach, payments, Pages or repository edits.

## Recommendation

For David: **own the brand, domain and marketing content immediately; outsource clinical care initially.** Shortlist MyDose Studio for a fast MVP, HighLevel HIPAA for a marketing-led no-code frontend/CRM, and WordPress on HIPAA Vault Starter for greater frontend ownership. Obtain a competing backend quote from Locke Bio, whose application-support partnership is documented by LegitScript itself.

There is no blanket HIPAA-plus-LegitScript builder credential. Separate four questions:
1. HIPAA-supporting vendor contract, covered product, entity relationship and configuration. HHS does not recognize private HIPAA certifications. A cash-pay medical practice is not automatically a Covered Entity merely because it treats patients; counsel must map physician practice/MSO/BA roles. Other privacy/FTC duties may still apply. [HHS-CERT]
2. LegitScript healthcare merchant/business model and website/domain certification, including clinical/pharmacy affiliates, licenses and permissible products. A builder does not grant it. No exact current entity/domain certification was independently verified here. [LS-TELE, LS-CHECK, LS-STATUS]
3. Payment underwriting: a gateway integration or PCI badge does not authorize this prescription business.
4. Google/YouTube/Meta advertiser, product, creative, destination and targeting rules. Certification does not approve every peptide or ad.

## Shortlist summary

| Offering | Category | Public price (USD) | Selection implication |
|---|---|---|---|
| MyDose Studio | Branded telehealth backend/storefront | $499/mo incl50 active, +$15/extra; clinical/fulfillment extras | Fast MVP; Studio client BAA and exit rights still needed |
| HighLevel + HIPAA | DIY website/funnel/CRM/workflows | $97 Starter + $297 HIPAA = $394/mo before usage | Strong marketing fit, not a medical backend |
| Wix eligible + PHI | Website builder with approved HIPAA apps | Exact eligible-plan amount not reliably rendered | Real BAA available; US Wix Payments prohibits medical practices/e-doctors/Rx |
| PatientGain | Healthcare managed agency/platform | Website headline $800-$4000/mo; custom $10k+ setup, typically $2500/mo; quote required | Ownership/buyout and proprietary apps constrain migration |
| Jotform Gold/Enterprise | Secure intake/signatures, not EHR | Gold $129 monthly/$99 annual monthly equivalent; Enterprise quote | Low-cost intake; standard BAA assumes actual Covered Entity customer |
| Formstack + HIPAA/EDS | Intake/docs/sign/workflows | Forms $99 monthly/$83 annual; HIPAA add-on extra quote | Security-mode API/webhook restrictions material |
| HIPAA Vault WP Starter | Managed healthcare host + custom WP | $349/mo; optional managed plugin updates $50+ | Ownership path; design/software/clinical services extra |
| Locke Bio | White-label telehealth/funnels/backend | Current quote required | Official LS expedited-review partnership evidence, not blanket certification |

## Critical findings

### Wix: new HIPAA capability, but payment mismatch
Do not repeat the outdated blanket statement that Wix never signs BAAs. Eligible editors: Harmony, Studio and Headless. Named eligible plans: Business, Plus, Elite, Business Elite and Enterprise. PHI protection and BAA must be activated; old Forms replaced; approved app list controls coverage. Identifying analytics are reduced; Facebook/Instagram Inbox channels disconnected; booking notes discouraged. [WX-HIPAA]

US Wix Payments expressly prohibits private medical practices/e-doctors/prescription medicines and separately lists peptides/research chemicals. Use only a separately approved clinical/payment arrangement, not assumed native checkout permission. [WX-PAY]

Standard Wix hosting portability is limited. Studio Two offers beta code export to Node hosting, still relying on Wix media/fonts/APIs; no proof HIPAA coverage extends outside Wix. Do not collapse the standard and beta offerings. [WX-EXPORT, WX-BETA]

### HighLevel: permanent add-on and incomplete export
BAA signing is not the final hardening step: each required subaccount needs its HIPAA toggle. Package documented as non-cancellable/non-refundable/permanent. Terms say BAA effectiveness depends on paid active package and payment failure terminates it; obtain counsel's view on retention/survival duties. [HL-HIPAA, HL-TERMS]

Contact CSV excludes automation/email/SMS history and truncates latest note at255 characters. No supported editable external website export. A contacts download is not full clinical or funnel migration. [HL-CSV, HL-EXPORT]

### Jotform: contracting entity and record-system limits
Standard published BAA is null if customer is not actually a Covered Entity. This matters if David contracts through a marketing/MSO entity: obtain an acceptable physician-entity or subcontractor structure, not just a HIPAA toggle. BAA says Jotform is not an EHR/designated record set and information must transfer into an appropriate record system before direct care use. Gold is single-user; use Enterprise or another appropriate team product rather than shared credentials. [JF-BAA, JF-PRICE]

### Formstack: security can change the integration plan
EDS documentation says no submit actions/webhooks; API submissions cannot include attachments. Default integration/email restrictions exist; optional granular overrides can weaken them but do not confer lawful PHI-disclosure permission. Confirm exact HIPAA/EDS SKU and proposed workflow before purchase. Base Forms price is not HIPAA all-in pricing. [FS-EDS, FS-PRICE]

### PatientGain: managed marketing, not fully portable software
Domain and patient data belong to client. Website/content rights depend on upfront setup or buyout; no-upfront subscriptions generally require12 months. Proprietary CRM/apps/AI/workflows/servers do not transfer. Public price ranges conflict across pages; require a fixed SOW and buyout schedule. Server-side 'obfuscation' claims are not independently proven HIPAA deidentification. [PG-PRICE, PG-OWN, PG-GLP]

### HIPAA Vault: secure hosting is one component
$120 Essential is editor-only; Starter349 is the relevant admin/custom-plugin tier. Plan table says Starter SSH/root but FAQ says no SSH: get written entitlements. Host BAA does not automatically cover arbitrary plugins, CRM, email, tracking or checkout. Design, optimization, WooCommerce setup and integration work are outside normal hosting scope. [HV-WP]

### Locke Bio: stronger LS application evidence, open contractual questions
LegitScript's February2023 announcement promises expedited application review for customers, not automatic certification. Confirm it remains offered. Canadian HQ does not prohibit US deployment, but require US processing/BAA/provider/pharmacy evidence. Public marketing-site privacy/terms are not a platform MSA or patient BAA. [LS-LOCKE, LB-HOME, LB-PRIV, LB-TERMS]

### MyDose: builder swap does not remove backend fees
Public FAQ says all states except New Jersey; get treatment-specific coverage. Studio active patient is one whose live plan payment covers any part of the billing month. Separate marketing frontend does not eliminate MyDose backend charges. Enterprise certification claim is not independent proof of Studio brand-domain certification. A health privacy URL found in search returned404; do not treat its search snippet as current Studio BAA evidence. [MD-FAQ, MD-STFAQ, MD-ENT]

## Practical frontend / clinical boundary

Separately registered clinic domain and owned content/creative -> public marketing frontend containing no PHI -> separate secured intake/patient portal -> clinical group/EHR -> eRx/labs/pharmacy -> approved payment/subscriptions.

An explicit redirect to a separate clinical origin is the cleanest initial boundary. An embedded secure form does not cure an unsuitable host's terms, pixels, session replay, referrers, logs or surrounding scripts. Names/emails/phone numbers with treatment inquiry or appointments can be PHI; do not label them universally safe lead fields.

HHS acknowledges the2024 partial court vacatur about IP address plus visits to unauthenticated health webpages. Do not say every anonymous health-page view automatically is PHI. Actual PHI disclosure restrictions remain. A cookie banner is not a HIPAA authorization. Hashing, server-side routing or 'obfuscation' alone is not HIPAA deidentification. [HHS-TRACK]

Start with dummy data; no Meta/Google/HYROS/Phonexa on intake, appointments, patient login, checkout or portal before legal and technical review. Audit URLs, referrers, query strings, logs, session replay, errors, CRM tags and conversion payloads. Separate clinical, communications/TCPA and recurring-payment consent.

Webflow terms3.6 prohibit PHI and say it does not offer HIPAA-compliant services. Marketing-only frontend linked to a separate secure portal is different from claiming Webflow is a HIPAA host. WebFetch500 was followed by successful normal public curl; raw source retained. [WF-TERMS]

MyDose Studio docs are narrower than general ecommerce tracking: general-page pageviews only, off by default/platform-gated; NEVER signup, purchase or patient events. General-page switch does not guarantee ad approval and must not be used to conceal a restricted destination. Studio has no SMS marketing flows; medical messaging occurs in clinical system. [MD-ADS, MD-STFAQ, MD-COMP]

## MCP and in-house skills
Confirmed official MCPs: **MyDose, HighLevel, Wix, Jotform**. Documented availability is not proof other buildout companies use them, nor proof production PHI processing through our bot is covered.
- MyDose endpoint https://mcp.mydose.ai/hub/mcp ; excludes clinical records/sensitive finance actions, but operational lists can still be sensitive. [MD-MCP]
- HighLevel official OAuth MCP supports broad CRM operations; opened documentation describes >550 operations/38domains. [HL-MCP]
- Wix endpoint https://mcp.wix.com/mcp ; site/API/account operations. [WX-MCP]
- Jotform endpoint https://mcp.jotform.com ; HIPAA plan plus explicit PHI-object scopes. Dedicated HIPAA REST endpoint also documented. [JF-MCP, JF-API]

No official MCP verified in reviewed sources for Formstack, PatientGain, HIPAA Vault or Locke Bio. PatientGain documents EMR REST connector. Locke homepage advertises documented APIs/webhooks/own frontend, but public schema not located. Formstack has material EDS restrictions. [PG-API, LB-HOME, FS-EDS]

Use dummy/non-PHI skills first: copy/SEO, catalog presentation, claims-review checklist, funnel QA, approved event-schema review, and export-rehearsal checklist. Platform BAA does not automatically cover an AI client, bot runtime, MCP proxy, logs/tracing, general workflow platform or downstream plugin. Scope those separately before PHI access.

## Software-only costs: not equivalent clinical stacks
- MyDose:50active499/mo;100active1249;200active2749;500active7249. Formula499+15*max(0,N-50). All clinical/medication/lab/shipping/processing extras remain. [MD-PRICE, MD-STFAQ]
- HighLevel HIPAA baseline394/mo =4728/year before usage and all clinical backend costs. [HL-HIPAA, HL-PRICE]
- HIPAA Vault Starter349 + Jotform Gold129 =478/mo; optional50 managed updates ->528/mo. HOST+INTAKE ONLY. Development/design, CRM/EHR, prescribers, eRx/labs/pharmacy, compliance/security operations and processing remain separate. [HV-WP, JF-PRICE]
- Jotform Gold1188/year annual billing versus1548/year month-to-month, single user. [JF-PRICE]
- Formstack Forms996/year annual or99/mo; Suite3000/year annual or299/mo; quoted HIPAA add-on extra. [FS-PRICE]

Do not infer a394 or478 stack replaces MyDose at50 patients. Compare total replacement clinical/tech/security operating cost, one-time build/migration, dual running and risk reserve.

## Questions counsel/vendors must resolve before live data
1. Exact legal entities and roles: physician practice, MSO/brand, vendor, pharmacy, merchant of record and record custodian. Correct BA/subcontractor agreements.
2. Actual BAA/product schedules; PHI subprocessors including hosting/email/SMS/video/AI/support; processing locations, breach notice, MFA/access/audits, backups/restoration, retention/deletion.
3. Exact live LegitScript seal/directory record for current legal entity/domain; new-brand process, fees, affiliates, products and renewal responsibility. 'Legitimate' and 'certified' are not interchangeable. No exact-domain status independently verified here.
4. Service/state matrix: GLP1/hormones/testosterone and controlled-substance requirements, visits/labs, prescriber and pharmacy licenses. US software availability is not US medical coverage.
5. Written payment underwriter acceptance; subscriptions/renewals/cancellations/refunds; merchant ownership and token/mandate portability; clinical approval/denial handling.
6. Dummy export demonstration: demographics, intake, attachments, signed/versioned consent/audits, notes/labs/Rx/orders/messages, subscription identifiers. Contacts CSV insufficient; record custodian controls lawful transfer.
7. Domain/source/content rights and plugin licenses; pricing escalators, per-patient triggers, setup/buyout/exit; read-only records after termination; migration support; portability of provider/pharmacy relationships.
8. Sandbox network/payload checks, least privilege/MFA, unsubscribe and subscription cancellation, EHR sync/export/restore before live PHI. No accounts were created during this research.

## Vendor-level evidence matrix

### MyDose Studio

- **Category:** Telehealth backend + branded storefront/funnels
- **Recommended use:** Fast clinical MVP; own marketing assets separately
- **Baa evidence:** HIPAA security claims; Studio customer BAA/exact legal entity not independently verified
- **Covered product and subprocessors:** Intake/clinical/providers/pharmacy/payments claimed; signed scope and subcontractor list required
- **Security and tracking limits:** Claims encryption/RBAC/audits. General-page visits only to ads, off by default/platform-gated; no signup/purchase/patient events; no SMS marketing flows
- **Domain seo landing ab:** Own domain; CMS/templates/page SEO; landing pages. A/B tests advertised on Studio site but exact feature scope not product-tested
- **Payments recurring rx:** Stripe/payouts/programs; clinician review before prescribing; recurring/merchant terms require contract
- **Consent:** Starter legal text; logged consent claims; counsel review required
- **Api webhook mcp:** Official MCP https://mcp.mydose.ai/hub/mcp; excludes clinical records and sensitive payment/bank/signup/terms/go-live actions
- **Export ownership migration:** Complete outbound clinical/content/subscription export and independent-hosting rights not verified
- **Us coverage:** FAQ says US except New Jersey; verify treatment-specific matrix
- **Public price usd:** $499/month after first patient includes50 active; $15/extra; free sandbox; no setup per Studio FAQ
- **Additional fees:** Drugs/consults/labs/Rx/shipping/card processing at cost; actual schedule needed
- **Legitscript evidence:** Enterprise page claims certification; exact current Studio brand-domain/entity status NOT verified
- **Unresolved questions:** Signed BAA/entity/subprocessors; brand-domain certification; complete exports; subscription/payment portability; exit rights
- **Source ids:** MD-PRICE;MD-FAQ;MD-ENT;MD-MCP;MD-STFAQ;MD-ADS;MD-COMP

### HighLevel + HIPAA package

- **Category:** True DIY builder/funnels + CRM/workflows
- **Recommended use:** Best marketing-led no-code candidate; separate clinical backend
- **Baa evidence:** Explicit BAA; HIPAA add-on297/month; agency-to-clinic agreement chain required
- **Covered product and subprocessors:** Per-subaccount HIPAA enablement; contacts/notes/custom fields/SMS/MMS/recordings/email/forms/calendars/invoices listed. Subprocessor list not eligible-product matrix
- **Security and tracking limits:** Encryption/MFA/audits. No blanket PHI permission for pixels/HYROS/Phonexa/integrations/AI; package non-cancellable; BAA tied to paid status
- **Domain seo landing ab:** Own domain; website/funnels/forms/quiz/calendar; SEO/AB exact selected-plan behavior not tested
- **Payments recurring rx:** Gateway/payments/subscription tools, not prescribing or pharmacy; underwriting required
- **Consent:** Forms/workflows; design clinical consent/versioning/retention separately
- **Api webhook mcp:** Official OAuth MCP/API; opened docs >550 operations38 domains; API plan limits verify
- **Export ownership migration:** Contacts CSV excludes automation/email/SMS history and truncates latest note255chars; no supported external website export
- **Us coverage:** US software; not clinician coverage; US hosting vendors and India support affiliate listed
- **Public price usd:** $97 Starter + $297 HIPAA = $394/month baseline
- **Additional fees:** Usage/communications/AI/integrations and all clinical/EHR/pharmacy costs extra
- **Legitscript evidence:** No included clinic/domain certification independently verified
- **Unresolved questions:** BAA eligible integrations/AI; permanent add-on; export completeness; registrar/domain control
- **Source ids:** HL-HIPAA;HL-PRICE;HL-MCP;HL-SUB;HL-TERMS;HL-EXPORT;HL-CSV

### Wix eligible plan + PHI Protection

- **Category:** True no-code website builder; selective HIPAA apps
- **Recommended use:** Brochure/SEO and approved intake; not native clinic checkout
- **Baa evidence:** Documented BAA after PHI activation; Business/Plus/Elite/Business Elite/Enterprise
- **Covered product and subprocessors:** Harmony/Studio/Headless listed; only approved apps; old Forms replace; exact covered app/processing schedule needed
- **Security and tracking limits:** Identifying analytics restricted; Facebook/Instagram Inbox disconnected; booking notes discouraged; external tools not automatically covered
- **Domain seo landing ab:** Own domain/pages/SEO/CMS; HIPAA-safe AB testing not verified
- **Payments recurring rx:** US Wix Payments prohibits medical practices/e-doctors/Rx and separately lists peptides/research chemicals. Separately approved clinical/payment integration needed
- **Consent:** Approved forms/bookings; clinical consent/version audit verify
- **Api webhook mcp:** Official Wix MCP https://mcp.wix.com/mcp; APIs; external AI PHI coverage not established
- **Export ownership migration:** Standard sites require Wix hosting; Studio Two beta export exists with Wix dependencies; external-host HIPAA coverage unverified
- **Us coverage:** HIPAA option for eligible US healthcare organizations; no medical network
- **Public price usd:** Exact eligible-plan current price not reliably rendered; verify US quote
- **Additional fees:** Clinical/pharmacy and approved processor separate
- **Legitscript evidence:** No included clinic/domain certification verified
- **Unresolved questions:** Approved apps/BAA annex; merchant acceptance; export beta compatibility; PHI API/MCP boundary
- **Source ids:** WX-HIPAA;WX-PRICE;WX-PAY;WX-MCP;WX-EXPORT;WX-BETA

### PatientGain VaultDocSites / GOLD-PLATINUM / Custom

- **Category:** Healthcare DFY agency + proprietary website/CRM/funnels
- **Recommended use:** Managed healthcare-marketing benchmark; weaker in-house portability
- **Baa evidence:** Explicit BAA for applicable services/apps; custom service BAA
- **Covered product and subprocessors:** Website/CRM/forms/texting/analytics/consent scope claimed; exact product/subprocessor chain obtain
- **Security and tracking limits:** Encryption/audit/US-server claims; server-side/obfuscation is not proof of HIPAA deidentification
- **Domain seo landing ab:** Client-owned domain; WordPress; SEO; vendor A/B-tested designs, not confirmed self-service experiments
- **Payments recurring rx:** Bill-pay app; clinical recurring Rx checkout not established; clinical backend separate
- **Consent:** Consent app tier-specific; PLATINUM included/GOLD extra per transparency table
- **Api webhook mcp:** Documented EMR REST connector; no official MCP verified
- **Export ownership migration:** Patient data/own content/domain owned; site needs setup/buyout; proprietary apps/AI/workflows/servers do not migrate
- **Us coverage:** US practice marketing; GLP1/weight-loss support documented; no provider network
- **Public price usd:** Homepage website800-4000/month; custom transparency10000+setup typically2500/month; conflicting pages require written quote
- **Additional fees:** Ads additional; transparency discusses18%ad management; custom integrations/buyout extra as contracted
- **Legitscript evidence:** GLP1 advertising experience not independent certification evidence
- **Unresolved questions:** Fixed quote/buyout; exact export fields; code ownership; BAA subprocessor and certification work scope
- **Source ids:** PG-HOME;PG-PRICE;PG-OWN;PG-API;PG-GLP

### Jotform Gold / Enterprise HIPAA

- **Category:** Secure intake/forms/signatures; not website or EHR
- **Recommended use:** Low-cost intake component for owned frontend
- **Baa evidence:** Published BAA; actual Covered Entity customer required or standard BAA null; Gold/Enterprise activation
- **Covered product and subprocessors:** Form platform/storage subprocessors; label PHI fields; downstream agreements required; exact residency verify
- **Security and tracking limits:** Encrypted data/audit claims; notification emails no PHI; Gold one user, no shared staff login
- **Domain seo landing ab:** Embeds/hosted forms; custom domain Enterprise; external frontend SEO/AB
- **Payments recurring rx:** Payment integrations generally supported; gateway recurring/Rx underwriting independently required
- **Consent:** Form signatures; Gold1000signed docs/month; clinical consent/version/retention workflow design
- **Api webhook mcp:** Official MCP gates PHI by enabled plan+explicit scopes; dedicated HIPAA REST endpoint; API/webhooks/export
- **Export ownership migration:** Not EHR/designated record set per BAA; transfer to proper record system before care; exported PHI customer responsibility
- **Us coverage:** HIPAA product; no clinicians/pharmacy; US data residency contract verify
- **Public price usd:** $129/month monthly or $99/month annual Gold; Enterprise quote multiuser/custom domain
- **Additional fees:** Hosting/EHR/clinical/pharmacy/processor extra; Gold1000payment submissions/month
- **Legitscript evidence:** No certification included/verified
- **Unresolved questions:** MSO vs Covered Entity contracting; EHR sync; complete attachment/consent exports; AI client BAA
- **Source ids:** JF-PRICE;JF-FAQ;JF-BAA;JF-API;JF-MCP

### Formstack Forms/Suite + HIPAA/Enhanced Data Security

- **Category:** Secure intake/workflows/docs/sign; not full website
- **Recommended use:** Structured workflows after integration proof
- **Baa evidence:** Standard BAA offered; custom BAA evaluation; configured HIPAA account
- **Covered product and subprocessors:** Explicitly schedule selected Forms/Documents/Sign services; approved integrations by default, not every third party
- **Security and tracking limits:** Encryption/permissions/audits; SMTP/email/attachment restrictions; granular overrides can weaken defaults
- **Domain seo landing ab:** Embeddable mobile forms; external frontend domain/SEO/AB; standalone custom-domain capability not verified
- **Payments recurring rx:** Stripe/PayPal on default EDS allowlist; recurring/Rx underwriting not established
- **Consent:** Approvals/signatures; Suite docs/sign; version/audit exports demonstrate
- **Api webhook mcp:** API; EDS no submit actions/webhooks; API submissions no attachments; no official MCP verified
- **Export ownership migration:** Submission exports with proper account; public-share restrictions; full docs/signatures/API migration test required
- **Us coverage:** Healthcare HIPAA use; no clinician/pharmacy coverage
- **Public price usd:** $99/month Forms monthly or $83 annual; Suite299monthly/250annual; HIPAA add-on EXTRA quote
- **Additional fees:** All clinical/EHR/pharmacy plus HIPAA add-on quote
- **Legitscript evidence:** No certification included/verified
- **Unresolved questions:** EDS vs HIPAA SKU/BAA scope; API limits; granular settings; add-on cost; export completeness
- **Source ids:** FS-HIPAA;FS-PRICE;FS-EDS

### HIPAA Vault Managed WordPress Starter + custom build

- **Category:** Healthcare-secure host plus owned WordPress; not turnkey builder
- **Recommended use:** Ownership-first frontend with engineering/compliance ownership
- **Baa evidence:** BAA promised all customers; actual signed product/region scope obtain
- **Covered product and subprocessors:** Hosting/WP security management; does not automatically cover plugins/email/CRM/payments/analytics
- **Security and tracking limits:** Encryption/RBAC/2FA/logs/WAF/patches/backups claimed; audit plugin telemetry/logging and all external services
- **Domain seo landing ab:** Own domain/WP pages/SEO/LP; custom plugins Starter+; AB tooling separately assessed
- **Payments recurring rx:** Starter up to10WooCommerce products; checkout/recurring configuration not included; prescribing/backend separate
- **Consent:** Build secure intake or add covered service; EHR/consent audit and retention custom
- **Api webhook mcp:** WP API/custom webhooks possible; no official host MCP verified
- **Export ownership migration:** Own site/code/database and self-migration access described; portability subject to IP contract/plugin licenses
- **Us coverage:** US HIPAA host; exact US region/support scope confirm; no clinical coverage
- **Public price usd:** Essential120/month editor-only; Starter349admin/customplugins; Plus599; managed plugin/theme updates Starter from50/month
- **Additional fees:** Design/dev/licenses/forms/CRM/EHR/clinical/pharmacy/processing separate
- **Legitscript evidence:** Host is not clinic certification
- **Unresolved questions:** Starter plan table SSH/root vs FAQ noSSH conflict; signed BAA; plugin/update responsibility; dev scope
- **Source ids:** HV-WP

### Locke Bio white-label / own frontend

- **Category:** Telehealth ecommerce funnels/backend
- **Recommended use:** Competing backend quote; documented LS application partnership
- **Baa evidence:** No public customer BAA verified in opened site/privacy/website terms
- **Covered product and subprocessors:** Intake/EMR/clinicians/pharmacy/subscriptions claimed; platform MSA/BAA/subprocessors/US region obtain
- **Security and tracking limits:** Identity+selfie verification/EMR/clinician review and country-specific storage claims; patient analytics boundary not public
- **Domain seo landing ab:** Branded domain/funnels; own frontend APIs/webhooks claim; SEO/AB exact scope not verified
- **Payments recurring rx:** Subscriptions/billing/retries/pharmacy routing; clinician review before Rx ships; processor terms extra
- **Consent:** Intake/identity/EMR; exact consent/version/audit must demonstrate
- **Api webhook mcp:** Homepage says documented APIs/webhooks/own frontend; public schema not located; no official MCP verified
- **Export ownership migration:** Full EMR/subscription/pharmacy export and source rights not publicly verified
- **Us coverage:** Canadian HQ; homepage claims50state clinicians; product/state/residency verify
- **Public price usd:** Current quote required; old numeric press pricing excluded
- **Additional fees:** Setup/platform/provider/pharmacy/labs/processing/per-patient fees itemize
- **Legitscript evidence:** LegitScript official2023 announcement: expedited application review; not automatic or current-domain certification
- **Unresolved questions:** BAA/entity; current partnership; itemized quote; exit/export; API access; treatment/state matrix
- **Source ids:** LS-LOCKE;LB-HOME;LB-PRIV;LB-TERMS

## Primary-source register

All opened during this research on 2026-11-07 (PST; America/Los_Angeles). Vendor claims are not independent audits. Search-only snippets and guessed404 URLs are excluded as evidence.

- **HHS-CERT: [HIPAA certifications](https://www.hhs.gov/hipaa/for-professionals/faq/2003/are-we-required-to-certify-our-organizations-compliance-with-the-standards/index.html)** — HHS does not recognize private HIPAA certifications; no absolution of legal obligations.
- **HHS-TRACK: [Online tracking guidance](https://www.hhs.gov/hipaa/for-professionals/privacy/guidance/hipaa-online-tracking/index.html)** — Actual PHI disclosures; cookie consent is not HIPAA authorization; 2024 partial vacatur acknowledged.
- **LS-TELE: [Telemedicine certification](https://www.legitscript.com/certification/telemedicine/)** — Healthcare merchant certification; application and annual per-website fees.
- **LS-CHECK: [Healthcare application checklist](https://www.legitscript.com/wp-content/uploads/2025/10/Healthcare-Application-Checklist.pdf)** — Downloaded PDF; licensing, privacy, affiliates, compounding, product permissibility and portal access.
- **LS-STATUS: [Website status lookup](https://www.legitscript.com/certification/website-certification-status/)** — Landing opened; no exact vendor/domain certification independently verified.
- **LS-LOCKE: [Locke Bio partnership](https://www.legitscript.com/about/press/legitscript-lockebio-telehealth-partnership/)** — 2023-02-15 announcement of expedited customer application review; confirm current terms.
- **MD-PRICE: [MyDose pricing](https://mydose.ai/pricing/)** — Studio $499/month includes50 active; $15/extra; provider/medication extra.
- **MD-FAQ: [MyDose FAQ](https://mydose.ai/faq/)** — Keep website/funnel; clinical platform/security assertions; US coverage except New Jersey.
- **MD-ENT: [MyDose Enterprise](https://mydose.ai/enterprise/)** — Quoted enterprise platform/provider/pharmacy; marketing claim of LegitScript certification, not exact-domain verification.
- **MD-MCP: [Studio AI/MCP](https://docs.mydose.ai/studio/build-with-ai)** — Official MCP; storefront/operational data; no clinical-record access or sensitive payment actions.
- **MD-STFAQ: [Studio FAQ](https://docs.mydose.ai/studio/faq.md)** — No setup; active-patient definition; extra pass-through costs; no SMS marketing flows; no purchase/signup ad events.
- **MD-ADS: [Studio SEO/ad pages](https://docs.mydose.ai/studio/seo-and-ad-pages.md)** — General-page pageviews only; feed off by default/platform-gated; no signup/purchase/patient events.
- **MD-COMP: [Studio compliance](https://docs.mydose.ai/studio/compliance-for-brand-owners.md)** — Platform content restrictions and legal starter text requiring counsel.
- **HL-HIPAA: [HighLevel HIPAA](https://help.gohighlevel.com/support/solutions/articles/48000983084-hipaa-compliance-with-highlevel)** — BAA $297/month; per-location hardening; listed PHI objects; non-cancellable package.
- **HL-PRICE: [HighLevel pricing](https://www.gohighlevel.com/pricing)** — Starter FAQ $97/month; usage extras; website/funnel/CRM/API/payment tools.
- **HL-MCP: [HighLevel official MCP](https://help.gohighlevel.com/support/solutions/articles/155000005741-how-to-setup-and-use-the-highlevel-mcp-server)** — OAuth; >550 operations/38 domains in opened documentation; external-client BAA not established.
- **HL-SUB: [HighLevel subprocessors](https://www.gohighlevel.com/sub-processors)** — US GCP/AWS, communications/AI vendors and India support affiliate; not HIPAA product allowlist.
- **HL-TERMS: [HighLevel terms](https://www.gohighlevel.com/terms-of-service)** — HIPAA BAA tied to active paid add-on; third-party and domain-control boundaries.
- **HL-EXPORT: [HighLevel website export](https://help.gohighlevel.com/support/solutions/articles/155000007342-can-highlevel-websites-be-exported-)** — No supported externally editable 1:1 website export.
- **HL-CSV: [HighLevel contacts export](https://help.gohighlevel.com/support/solutions/articles/48001238482-contacts-export-as-csv-upgrade)** — CSV excludes automation/email/SMS history; latest note truncated at255 characters.
- **WX-HIPAA: [Wix HIPAA](https://support.wix.com/en/article/enabling-hipaa-compliance-for-your-wix-site)** — Eligible editors/plans; PHI enablement+BAA; old Forms, booking notes, apps/inbox/analytics restrictions.
- **WX-PRICE: [Wix plans](https://www.wix.com/plans)** — Dynamic page omitted Business amount; exact eligible-plan price not reliably extracted.
- **WX-PAY: [Wix Payments prohibited US services](https://support.wix.com/en/article/wix-payments-prohibited-products-and-services)** — Prohibits private medical practices/e-doctors/Rx; peptides/research chemicals separately listed.
- **WX-MCP: [Wix official MCP](https://dev.wix.com/docs/overview/ai-the-wix-platform/the-wix-mcp)** — Official docs/site API/account actions; external AI HIPAA coverage not established.
- **WX-EXPORT: [Wix standard hosting/export](https://support.wix.com/en/article/exporting-or-embedding-your-wix-site-elsewhere)** — Standard sites depend on Wix hosting; customer owns content.
- **WX-BETA: [Wix Studio Two beta export](https://dev.wix.com/docs/studio-two/code-your-site/export-your-site/host-an-exported-site-outside-wix)** — Beta Node hosting export still depends on Wix media/fonts/APIs; outside-host HIPAA coverage unverified.
- **PG-HOME: [PatientGain homepage](https://www.patientgain.com/)** — US DFY marketing; BAA; website headline $800-$4000/month.
- **PG-PRICE: [PatientGain transparency](https://www.patientgain.com/transparent-pricing)** — Custom $10k+ setup and typically $2500/month;12-month no-upfront plans; price inconsistencies; ownership conditions.
- **PG-OWN: [PatientGain ownership](https://www.patientgain.com/healthcare-website-that-i-can-own)** — Domain/patient data owned; website setup/buyout; proprietary applications do not transfer.
- **PG-API: [PatientGain EMR connector](https://www.patientgain.com/medical-marketing-ehr-emr-integration-api-pricing)** — EMR REST connector, BAA; OpenEMR included in PLATINUM; others/custom scope may cost extra.
- **PG-GLP: [PatientGain GLP1 marketing](https://www.patientgain.com/semaglutide-marketing)** — GLP1 support; conflicting headline/body price ranges, not fixed quote.
- **JF-PRICE: [Jotform HIPAA pricing](https://www.jotform.com/hipaa/pricing/)** — Gold129 monthly/99 monthly annual; single user; Enterprise quote, team/custom domain.
- **JF-FAQ: [Jotform HIPAA FAQ](https://www.jotform.com/hipaa/faq/)** — Activation/BAA, encrypted forms, PHI-free email notifications, payment integrations.
- **JF-BAA: [Jotform actual BAA](https://www.jotform.com/hipaa/baa/)** — Null if customer not Covered Entity; not EHR/record set; PHI labels/downstream agreements/export responsibility.
- **JF-API: [Jotform API](https://api.jotform.com/docs/)** — Dedicated HIPAA endpoint, API/webhook/export capabilities.
- **JF-MCP: [Jotform official MCP](https://www.jotform.com/developers/mcp/)** — HIPAA account+explicit PHI object scopes needed; no automatic external-client coverage.
- **FS-HIPAA: [Formstack healthcare forms](https://www.formstack.com/features/hipaa-friendly-forms)** — Standard BAA/custom evaluation; specifically configured account.
- **FS-PRICE: [Formstack pricing](https://www.formstack.com/pricing)** — Forms99 monthly/83 annual;Suite299 monthly/250 annual; HIPAA add-on extra quote.
- **FS-EDS: [Formstack enhanced security](https://help.formstack.com/hc/en-us/articles/44591882785043-Enhanced-Data-Security-Add-On-Overview)** — No submit actions/webhooks; API attachment restriction; limited integrations; granular overrides.
- **HV-WP: [HIPAA Vault Managed WordPress](https://www.hipaavault.com/hipaa-vault-managed-wordpress-hosting/)** — BAA; Essential120 editor;Starter349 admin/custom plugins;Plus599; optional updates50+; SSH contradiction.
- **LB-HOME: [Locke Bio platform](https://www.lockebio.com/)** — Funnels/clinical/pharmacy/subscriptions; own frontend APIs/webhooks claimed;50-state clinician claim.
- **LB-PRIV: [Locke Bio website privacy](https://lockebio.com/privacy.html)** — Marketing-site data policy, not patient-platform BAA.
- **LB-TERMS: [Locke Bio website terms](https://lockebio.com/terms.html)** — Marketing-site terms, not customer platform MSA/BAA.
- **WF-TERMS: [Webflow terms3.6](https://webflow.com/legal/terms)** — WebFetch500 then normal public curl succeeded; prohibits PHI; HTML/text retained.

## Access limits and evidence conflicts
- No authenticated product testing, signed BAA/MSA review, domain certification result or private pricing quote was obtained.
- MyDose `https://health.mydose.ai/privacy-policy` returned404 despite search indexing; not relied on as current BAA evidence.
- Locke `/privacy` returned404; working public policy is `/privacy.html`.
- A guessed LegitScript standards URL404 was not used; successful telemedicine page/checklist/lookup landing/official partnership provide evidence.
- Wix Business current amount not reliably extracted; exact eligible-plan price intentionally unknown.
- HIPAA Vault SSH plan-table/FAQ conflict and PatientGain pricing variations remain unresolved.
- Webflow WebFetch500 followed by successful public curl; retained HTML/text. LegitScript checklist downloaded and text-extracted.
