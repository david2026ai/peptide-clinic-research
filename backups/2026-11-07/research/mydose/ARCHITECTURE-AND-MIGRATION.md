# MyDose-first MVP → owned platform: architecture and migration specification

Research date: **November 7, 2026, PST**. This is a planning specification, not MyDose's actual internal architecture. No implementation, account creation, connector installation, clinical action, patient export or repository modification occurred.

## Recommendation

Start with a bounded MyDose Studio MVP only after clinical, privacy, ownership and export gates pass. Own the brand, registrar/domain, original content, creative and evidence register from day one. Do not automatically migrate at patient 51. Negotiate volume pricing or a cap, and compare total replacement cost with the fee being avoided. An owned marketing frontend that keeps MyDose's backend does not remove its contractual patient fees.

The strongest long-term candidate is an owned marketing workbench and integration layer over contracted clinical services. Fully internal software still requires licensed clinicians, medical-record custody, lawful eRx/EPCS, pharmacies, labs, payment underwriting, security operations and care support. Code does not replace those permissions or recurring costs.

## Verified product economics

Studio is free until the first live patient purchase, then **$499/month including 50 active patients**, plus **$15/month for each active above 50**. Active means a patient's live plan payment covers any part of the billing month, counted once/month; tests are excluded. Overage is deducted from payouts, oldest month first. The contract must resolve base-card versus payout collection wording, cancellation/proration and zero-patient post-activation billing.

Medication, provider consults, labs, prescriptions and shipping pass through at cost. Card-processing fees also apply. Numeric pass-through rates are not public. Do not substitute Hedonic's $27 consult or 4% processing for MyDose's actual costs.

| Active | Studio/month | Studio/year at constant count | Overage-only/month |
|---|---:|---:|---:|
|50|499|5,988|0|
|100|1,249|14,988|750|
|200|2,749|32,988|2,250|
|250|3,499|41,988|3,000|
|500|7,249|86,988|6,750|
|1,000|14,749|176,988|14,250|

Source: https://docs.mydose.ai/studio/billing-and-plan and https://docs.mydose.ai/studio/payouts .

## Verified identities and boundaries

- **Stripe Connect:** payment/payout documentation. Exact connected-account type, merchant of record, charge architecture, ownership and exit cooperation are unknown.
- **NVP Medical Group P.A.:** named on clinical-software marketing. Current contract/roster/service-state coverage and direct continuity require validation.
- **NewLife Pharmacy:** named in February 2026 changelog. Not proof it fulfills every current Studio product; precise licensed entity/current scope unknown.
- **WorkOS:** auth/directory sync named in January 2026 changelog. Not proof every Studio surface uses it or that MyDose uses WorkOS MCP.
- **Google Calendar:** connection shown in clinic Calendar guide; exact payload/sync/BAA plan unknown.
- **Calendly/Acuity:** marketing integration claims, not tested Studio entitlement.
- **AWS/Rybbit/Google Analytics:** public website disclosures, not a verified clinical-stack inventory.
- **Unestablished vendors:** eRx/EPCS intermediary, lab network/interface, video, email/SMS transport and AI model provider.

Studio documents no SMS marketing sequences, no care-message replies inside Studio, and no signup/purchase/patient events sent to ad platforms. General-page feeds are limited, off by default and may be platform-wide disabled. Clinical intake summaries are reading aids, not clinical conclusions. Product and pricing-control language conflicts across marketing and product guides. Complete clinical bulk export/API entitlement is not publicly documented.

See `integration-inventory.csv` for 29 detailed records: evidence class, inputs/outputs, source of truth, owner/payer, PHI and unknowns. Alternatives are explicitly labeled; no guessed Next.js/Supabase/Twilio stack.

## Owned-platform product modules (recommended design)

1. **Content and design system:** portable source/content blocks, theme tokens, original media, preview/version history, slugs, SEO and redirect manifests. Distinguish our licensed content from vendor proprietary code/templates.
2. **Claims/evidence register:** exact claim, molecule/formulation, indication, approval/compounded/off-label/unapproved status, geography, source/date, limitation and reviewer. Internal PASS/REVISE/BLOCKED is separate from clinical/legal/platform approval.
3. **Creative/CRO workbench:** campaign brief → website copy + editing OR video hook/storyboard/script → clinical claims filter → platform filter → client rules → specifically authorized publication. No fabricated reviews, guaranteed outcomes or dosing advice.
4. **Catalog presentation:** immutable clinically approved SKU and price versions; exact quantity/unit/formulation, consultation/lab/medication/shipping exclusions, recurring price and cancellation terms. A supplier listing is not treatment authority, and mg is not a month.
5. **Consent-aware lifecycle/support:** nonclinical marketing and clinical care separated. Names/emails/phones with a treatment inquiry may be PHI or consumer-health data. No blanket patient tracking imported from legal lead generation.
6. **Aggregate attribution:** approved campaign/spend/public-page reports. No patient lists, medication-purchase events or health-tagged conversions to ads or general AI. Small-cell suppression is a house safeguard, not legal deidentification by itself.
7. **Operations dashboard:** need-to-know financial/order/exception metadata, accountable escalation and links to the medical record. Do not duplicate full charts in a marketing warehouse.
8. **Integration hub:** versioned adapters, signed-webhook verification where documented, queues/outbox, idempotency, retries/backoff, dead letters, replay and source-system reconciliation.
9. **Identity/security:** MFA, least privilege, tenant separation, separate marketing/clinical origins, secret manager, log redaction, backups/restore, vendor/BAA register and incident coverage. No real PHI in development/sandbox.

## Proposed entities and events—not discovered MyDose schemas

Entities: Brand/Domain; CatalogSKUVersion/PriceVersion; EvidenceClaim/Review/ConsentVersion; PatientLink; MedicalEntity/Practitioner/License; Intake/Encounter/CarePlan; LabOrder/Result; Prescription/Fill/Shipment; Subscription/Invoice/Payment/Refund; SupportTask; IntegrationEvent; MigrationLedger.

Every mapping preserves vendor-native IDs, tenant, actor, version/time and lawful purpose. Clinical entities stay within the restricted record/PHI boundary. A public marketing workspace receives only authorized non-PHI content or approved aggregates.

Proposed events include intake.submitted, review.approved/denied/needs_information, prescription.authorized, pharmacy.accepted/rejected/backordered, fill.dispensed, shipment.updated, lab.resulted/amended/critical, subscription.paid/failed/cancelled, consent.withdrawn and task.escalated. These names are not claims about MyDose APIs. Payment success must not automatically authorize a prescription or dispense.

## Edge handling

| Failure | Required control |
|---|---|
| Duplicate/out-of-order callback | Vendor event ID/idempotency, version/time check and source requery; never duplicate charge/fill |
| Clinical denial after charge | Independent clinical decision; transparent contractually valid finance/refund workflow |
| Changed patient state/expired credential | Clinical routing hold and authorized eligibility review; payment cannot override |
| Pharmacy rejection/backorder/cold-chain/recall | Pharmacist-owned exception and secure patient notice; no unilateral substitution |
| Critical/amended result/unread urgent message | Named clinician acknowledgement, escalation and backup coverage |
| Failed payment/cancellation/outage | Track billing, paid-through and care separately; secure fallback/replay; no automatic abandonment |
| PHI leak/tenant misroute | Quarantine and approved incident process; do not paste sensitive payload into general chat |

## Portability and acceptance

`PORTABILITY.md` and CSV/JSON cover 18 asset groups. Require a synthetic full-export acceptance test before live patients: identities, raw intake/question versions, signed original consent/audit, signed chart notes/addenda, labs/units/reference ranges/original PDFs, prescription/fill history, pending orders/shipments, messages/files, operational tasks, financial identifiers and audit manifest. Counts/hashes and clinical custodian review should establish completeness. PDF export, CSV import and contact download are not equivalent.

The medical entity's record custody and patient access rights do not grant the marketing/MSO unrestricted bulk export. Contract for post-termination read access, retention, formats, attachments, migration assistance/fees and response SLA. Website-only terms are not the commercial MSA/BAA. Do not scrape private interfaces or use undocumented APIs as an exit route.

Do not assume clinician relationships, pharmacy contracts, remaining prescription fills, EPCS identities, certificates, payment mandates/subscriptions, email domains or SMS reputation move automatically. Prescriber/pharmacist determines lawful transfer or a new prescription/visit; same partners can continue only if contracts and law permit. Never delete regulated records to reduce a usage fee.

## Stripe cutover

First establish exact account/merchant/charge topology and source owner cooperation. Stripe's authorized customer-data copy supports eligible customers/payment methods, not charges, invoices, plans, subscriptions, coupons, events/logs or guests through that tool. Payment-method IDs change. Subscription recreation/import is separate: anchors, paid-through, credits, cancellations, mandates/payee scope and pricing must reconcile. Some patients may need to re-enter payment information or consent.

Disconnect does not automatically cancel subscriptions; direct charges/application fees can continue and destination-charge workflows can fail. Connected-account cloning has restrictions. Use processor-mediated supported migration, never raw card/token exports. Keep historical dispute/refund access and reserves responsibilities. One financial collection owner per obligation; do not charge both platforms.

Official references: https://docs.stripe.com/get-started/data-migrations/pan-copy-self-serve?copy-method=full ; https://docs.stripe.com/billing/subscriptions/migrate-subscriptions ; https://docs.stripe.com/connect/subscriptions ; https://docs.stripe.com/billing/multi-entity-business .

## Stage gates

0. Own domain/assets and sign appropriate clinical/MSA/BAA/export/retention contracts; confirm merchant/certification and exact fee scope.
1. Build/test only with synthetic data; test denial/refund, state block, failure, cancellation, pharmacy/lab/support exceptions and export/restore.
2. Bounded first cohort; up to 50 active is a planning assumption, not account splitting or active-status manipulation. Measure contribution, retention, clinical/fill times, support cost and actual fees.
3. Negotiate volume cap/Enterprise and competing managed-backend quotes. Replace model assumptions with real net costs.
4. Validate independent stack in sandbox; new patients first after clinical/legal/security/payment/certification gates.
5. Consented clinically appropriate cohorts; migration ledger tracks identities, custody, consent, paid-through/next bill, remaining fills, open tasks/results/messages and shipments.
6. Parallel run and daily reconciliation. One collection owner per billing obligation and one fulfillment owner per authorized fill. Clinician decides legitimate treatment changes. Source billing cancellation confirmed before destination charges.
7. Proposed house gate: two full billing/refill cycles without unresolved safety/financial discrepancies before retiring operational dependencies; legal record retention continues. Software/DNS rollback cannot reverse an encounter, charge or dispensed medication. Keep clinical continuity and source access.

## Economics and sensitivity—assumptions, not quotes

Default lean managed-partner replacement: M=$60,000 one-time, O=$3,500/month fixed incremental replacement cost, v=$5/patient/month net incremental cost, T=24 months. This is not a fully staffed internal medical practice. Unchanged clinical/drug/lab/shipping/processing costs cancel only if truly unchanged; add real differences.

For N>50: Studio=15N−251; replacement steady cost=O+vN. Positive full-exit savings including build amortization require N>(O+M/T+251)/(15−v), when v<15. Default positive threshold626; at12months876. At500 steady savings1249/month but payback48.04months; at1000 savings6249/month and9.60months. At250 replacement costs1251/month more, before build. Sensitivity v0/5/10 with sameO/M/T gives417/626/1251 active. Higher O7000/M80000/v5/T24 gives1059. Not a forecast or guaranteed migration threshold. A retained base/backend fee needs its own different model.

Illustrative engineering bounds: own frontend + managed clinical API240–600h ×125–175/h =30k–105k engineering; full assembly1000–2400h ×125–175/h =125k–420k engineering, plus illustrative30k–100k legal/security/transition. Not quotes, caps or timelines. Full-time engineering/care/security support can substantially exceed3500/month. Add payment re-entry losses, new visits, parallel systems, record access, churn and disputes. No CAC/revenue uplift assumed.

## MCP and reusable skills

See `MCP-INVENTORY.md` and19-record CSV/JSON. Confirmed MyDose MCP is storefront/business automation, not full clinical export. Builder MCPs HighLevel/Wix/Jotform are available first-party capabilities, not proof of adoption by MyDose/Hedonic. Healthie Dev Assist/Medplum are alternatives. Stripe/WorkOS/AWS/Meta/Google official MCPs are available services; Twilio is docs-only. API-only dependencies still need adapters; a custom MCP wrapper is new engineering. Private endpoints are unknown, not guessed.

Pin/refresh actual manifest and scopes. Google Ads documentation versus current README differs on write capabilities; enforce read-only allowlist rather than trust a label. Stripe current non-Agent legacy-key transition deadline isNov30,2026. No keys/PHI/PAN in chat/repo. All live mutations need separate authorization and professional approval where applicable. Six local neutral draft skills and audit template are uninstalled specifications only.

## Builder/privacy/legal gates

Included builder research covers8offerings/44primaryrefs. HighLevel394 or WPStarter349+JotformGold129=478 is not a MyDose clinical replacement. HighLevel permanent HIPAA add-on/export limits; Wix current PHI option but payment prohibitions; Jotform contracting entity/single-user/record-system limits; Formstack EDS webhook/attachment restrictions; PatientGain buyout/proprietary-app limitations; HIPAA Vault host scope; Locke expedited application review, not automatic certification.

No private HIPAA badge substitutes for correct entities/BAAs/configuration/security. Cash-pay alone does not establish HIPAA scope; state consumer-health/FTC rules may apply. HHS acknowledges2024 partial tracking vacatur: not every anonymous public health-page visit automatically PHI; identifiable intake/appointments differ. Cookie banners, hashing and server-side routing are not automatically legal authorization/deidentification. Separate public marketing and clinical origins; review actual referrers/URLs/logs/payloads.

State counsel must resolve PC/MSO control, fee-splitting and records custody; CA§2400/650 are examples, not nationwide rules. Controlled-drug telemedicine extension currently endsDec31,2026 subject to conditions; not general async-only TRT authority. LegitScript entity/domain/product/affiliate scope, advertiser permission and payment underwriting are independent; no automatic transfer from an agency.

## Documents still needed

Signed product-specific MSA/BAA/subprocessors; medical/provider/pharmacy/eRx/lab roster and service/state matrix; exact all-in rate card and retail controls; active/base/cancellation/volume terms; owned-domain/content/source rights; complete export/exit/record retention SLA; direct partner continuity and restrictive covenants; exact Stripe topology/mandates/subscription cooperation/reserves; certification scope; approved event payloads; AI/eRx/EPCS/security evidence. Ask Hedonic which creative/media/lifecycle/IP work its40k build fee supplies beyond a MyDose storefront, and who actually owns underlying accounts/contracts.

Do not launch if lawful record/PHI authority, clinical coverage or continuity/export rights are unresolved. Do not migrate until real quotes and safe reconciliation justify it.
