# Portability acceptance inventory

2026-11-07 PST. Research only. No connections, installations, PHI handling or migrations. Public capability does not prove another company's adoption; full commercial/export/clinical authority requires contract evidence.

## Brand/domain/content
- **status**: CONDITIONAL
- **required export or evidence**: Own registrar/admin, source assets/license, authored page versions, routes/SEO/redirect map. Proprietary template/source rights unknown.
- **acceptance owner and gate**: Business/IP counsel: signed ownership/export rights; clinical portal DNS cutover tested.
- **access date**: 2026-11-07 PST

## Catalog/prices
- **status**: UNRESOLVED
- **required export or evidence**: Molecule/form/strength/concentration/quantity/unit, pharmacy SKU, lawful formulary/states, consult/labs/shipping inclusions. MyDose says catalog/prices owned while marketing says set prices.
- **acceptance owner and gate**: Clinical director/pharmacist + contract specify actual control and new formulary. mg is not month.
- **access date**: 2026-11-07 PST

## Consented CRM
- **status**: CONDITIONAL
- **required export or evidence**: Purpose/source/consentversion/time/entity, unsubscribe/suppression. Health-related names/emails/phone inquiries may bePHI or regulated healthdata.
- **acceptance owner and gate**: Privacy counsel: authorizedpurpose/transfer, no patientlist audienceuploads; no simple non-PHI assertion.
- **access date**: 2026-11-07 PST

## Patient identity
- **status**: FULL EXPORT NOT VERIFIED
- **required export or evidence**: Stable source patient/org/brand/medical entity IDs, securely transferred verified demographics, duplicate mapping.
- **acceptance owner and gate**: Medical custodian authorizes export; identity-safe matching and exceptions reviewed.
- **access date**: 2026-11-07 PST

## Intakes/photos
- **status**: PARTIAL FEATURE ONLY
- **required export or evidence**: Raw answers +questionnaire versions, times/signatures, source IDs, original uploads. PDF export release note is not complete structuredexport.
- **acceptance owner and gate**: Counts/hashes/manifest and clinical equivalence accepted; lawful documented export only, no scraping.
- **access date**: 2026-11-07 PST

## Consents
- **status**: FULL EXPORT/NEWENTITY VALIDITY UNKNOWN
- **required export or evidence**: Signed originals/textversion, signer, timestamp/timezone, verification/audit, withdrawals, entity/purpose.
- **acceptance owner and gate**: New notices/consents where required; no silent carry-forward to different clinician/controller.
- **access date**: 2026-11-07 PST

## Charts/SOAP/treatmentplans
- **status**: FULL EXPORT/API NOT VERIFIED
- **required export or evidence**: Notes/signatures/addenda, problems/allergies/medhistory, treatmentprotocolversions, authors/dates and original files.
- **acceptance owner and gate**: Clinical custodian signs off completeness, retention/access, lawful patient notification and continuity.
- **access date**: 2026-11-07 PST

## Labs/criticalalerts
- **status**: PARTNER/INTERFACE UNKNOWN
- **required export or evidence**: Orders/accessions, analyteunits/ranges/status/amendments, original PDFs, acknowledgement and outstanding critical tasks.
- **acceptance owner and gate**: Ordering clinician owns outstandingresults and handoff; no result lost during transition.
- **access date**: 2026-11-07 PST

## Rx/refills/EPCS
- **status**: NOT AUTOMATIC
- **required export or evidence**: Prescriber/pharmacy IDs, prescription/fill IDs, remaining fills/validity/days supply/last dispense, pending changes. EPCS identities/tokens not transferable by app.
- **acceptance owner and gate**: Prescriber/pharmacist determine lawful transfer or new Rx/consult; actual EPCS vendor proof; never copy credential keys.
- **access date**: 2026-11-07 PST

## Medicalgroup/pharmacy contracts
- **status**: NOT AUTOMATIC
- **required export or evidence**: State/service coverage, record custody/retention, malpractice/continuity, non-solicit/exit/provideravailability.
- **acceptance owner and gate**: Same clinicians/pharmacies only if lawful and contracts allow; software ownership does not grant practice rights.
- **access date**: 2026-11-07 PST

## Orders/shipping
- **status**: FULL EXPORT/REPLAY UNKNOWN
- **required export or evidence**: PaidThrough, order/Rx/fill/shipment IDs/status, exactSKU/quantity/costs/refill due/tracking/exceptions.
- **acceptance owner and gate**: One fulfillment owner per authorized fill/cycle, reconcile in-flight orders; clinical changes require clinician.
- **access date**: 2026-11-07 PST

## Messages/support
- **status**: FULL THREAD EXPORT UNKNOWN
- **required export or evidence**: Participants/thread content/files, unread/open tasks, urgency/clinical escalation, timestamps/IDs. Studio shows metadata, care dashboard handles messages.
- **acceptance owner and gate**: Securehandoff and after-hours/escalation coverage; no email PHI export or duplicate outreach.
- **access date**: 2026-11-07 PST

## Customers/payment methods
- **status**: STRIPE CONDITIONAL COPY
- **required export or evidence**: Exact account type/charge model/customer and payment method maps, consent/mandate/payee scope. Processor-mediated transfer only.
- **acceptance owner and gate**: Sourceaccountowner +destination authorization; underwriter approves; no rawPAN exported. May require patient re-entry.
- **access date**: 2026-11-07 PST

## Subscriptions/billing
- **status**: SEPARATE MIGRATION
- **required export or evidence**: Subscriptions excluded from Stripe customer copy. Preserve anchor/paid-through, prices/discounts/credits/cancel/pause/delinquency/tax/refund obligations.
- **acceptance owner and gate**: Dryrun schedule then one collectionowner perobligation, authorizednew mandate/source cancellation confirmation. Disconnect is not automaticcancellation.
- **access date**: 2026-11-07 PST

## Financialhistory/disputes
- **status**: RETAIN SOURCE
- **required export or evidence**: Invoices/charges/events/logs not customer-copy objects. Historical ledger/receipts/reserves/negativebalance responsibilities.
- **acceptance owner and gate**: Keep required source access/retention; no premature account closing or deletion.
- **access date**: 2026-11-07 PST

## Audit/security/RBAC
- **status**: EXPORT/SURVIVAL UNKNOWN
- **required export or evidence**: Tenant/actor/time/action/version, consent/e-sign/clinical audit provenance, accessroles, incidents ascontracted.
- **acceptance owner and gate**: MFA/tenant isolation/log redaction/backups/restore tested; legal retention, noPHI in dev/AI.
- **access date**: 2026-11-07 PST

## Email/SMS/sender
- **status**: CONDITIONAL; NO STUDIO SMS
- **required export or evidence**: Owned sending domain/DKIM/SPF/DMARC, delivery/suppression, supportrouting. SMS sender reputation/registration not automatically portable; Studio has no SMS feature.
- **acceptance owner and gate**: Reverifyapproved sender/consent; no assumption third-party transport/AIcovered.
- **access date**: 2026-11-07 PST

## LegitScript/ads/merchant
- **status**: NOT AUTOMATIC
- **required export or evidence**: Exact legalentity/root domain/business model/certifier listing, advertiserpermissions, processorunderwriting and renewed affiliates/product scope.
- **acceptance owner and gate**: Written entity/domain/account-specific transition confirmation; agency certification not blanket transferable.
- **access date**: 2026-11-07 PST