# Integration and responsibility inventory

2026-11-07 PST; capabilities documented/claimed, not production-tested.

## I01 — MyDose Studio / Entry/storefront
- **evidence status**: OBSERVED PUBLIC UI
- **capability**: Public entry describes branded telehealth storefront; parent browser encountered login; no production testing
- **access interface**: Public web and documented dashboard
- **input data**: Brand/content/program choices
- **output data**: Published branded pages
- **source of truth**: Own licensed brand assets + MyDose CMS
- **phi scope**: Keep marketing content non-PHI
- **responsibility and payer**: Brand owns marketing; platform hosting subscription
- **limits or unknowns**: No source-code ownership/export rights established; no authenticated tour
- **source urls**: https://studio.mydose.ai/ | https://mydose.ai/studio/ | https://docs.mydose.ai/studio/store-editor
- **access date**: 2026-11-07 PST

## I02 — MyDose catalog / Catalog/pricing
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Toggle catalog products; provider eligibility independent of product selection
- **access interface**: Products screen; no public SKU export/API specification
- **input data**: Product selections
- **output data**: Visible product pages/read-only editor prices
- **source of truth**: MyDose catalog and clinically authorized SKU version
- **phi scope**: Product interest tied to identity is sensitive
- **responsibility and payer**: MyDose controls underlying catalog; brand claims responsibility
- **limits or unknowns**: Marketing says set prices, guide says catalog/prices MyDose-owned; Set prices page401; need actual editable field/range rights
- **source urls**: https://docs.mydose.ai/studio/choose-products | https://mydose.ai/studio/ | https://mydose.ai/pricing/
- **access date**: 2026-11-07 PST

## I03 — MyDose MCP / AI/CMS
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Pages/themes/menus/media/discounts/team/brand; reads permitted business orders/patient lists/payout totals
- **access interface**: https://mcp.mydose.ai/hub/mcp; remote HTTP; OAuth or time-limited key
- **input data**: Authorized store context + content drafts
- **output data**: Read summaries and authorized storefront changes
- **source of truth**: MyDose store
- **phi scope**: Business patient/order data can still be PHI; clinical records excluded
- **responsibility and payer**: Operator authorizes least privilege; MyDose hosts; account price applies
- **limits or unknowns**: 82hub+104CMS tools is marketing count, not audited schemas; no headless clinical/export API proof; no payment/bank/signup/terms/go-live checkout; no clinical records; noSVG/>4MBuploads; destructive confirm5min
- **source urls**: https://docs.mydose.ai/studio/build-with-ai | https://mydose.ai/studio/
- **access date**: 2026-11-07 PST

## I04 — Stripe Connect / Payouts/payments
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Bank onboarding, card checkout and settlements; recurring billing in clinic docs/changelog
- **access interface**: Stripe Connect via MyDose; Stripe APIs not authorized through mere payout connection
- **input data**: Processor payment data and KYC through secure onboarding
- **output data**: Payments/payouts/status
- **source of truth**: Stripe account + MyDose operational ledger
- **phi scope**: No drug/diagnosis/intake in processor metadata
- **responsibility and payer**: MyDose payment orchestration; brand/medical entity financial responsibilities contract-dependent
- **limits or unknowns**: Exact connected-account type, charge model, MoR, token/customer/subscription owner, rate, reserves, disputes and exit support unknown
- **source urls**: https://docs.mydose.ai/studio/payouts | https://docs.mydose.ai/studio/faq | https://docs.mydose.ai/clinic-guide/billing | https://docs.mydose.ai/changelog | https://docs.stripe.com/connect | https://docs.stripe.com/connect/subscriptions
- **access date**: 2026-11-07 PST

## I05 — NVP Medical Group P.A. / Provider network
- **evidence status**: VENDOR CLAIM
- **capability**: Named medical-provider coverage on clinic-software page; independent review/prescribing
- **access interface**: MyDose managed clinical portal; no public provider-network API contract
- **input data**: Consent/intake/patient location/history
- **output data**: Clinical decision/care plan/prescription
- **source of truth**: Treating medical practice
- **phi scope**: PHI
- **responsibility and payer**: Clinical group responsible for care; consult pass-through cost; operator clinical independence
- **limits or unknowns**: Current entity agreement/roster/licenses/SLA/program matrix/continuity and ability to contract outside MyDose unknown; FAQ excludes NJ
- **source urls**: https://mydose.ai/clinical-software/ | https://mydose.ai/faq/ | https://docs.mydose.ai/clinic-guide/review-intakes
- **access date**: 2026-11-07 PST

## I06 — MyDose clinical portal / Intake/consents
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Forms, records, e-consent, review queue and provider decisions
- **access interface**: Documented portal; no public general patient export API found
- **input data**: Questionnaires/consent versions/photos
- **output data**: Submission records, signed documents, decision
- **source of truth**: Medical entity chart
- **phi scope**: PHI including photos and signatures
- **responsibility and payer**: Medical practice defines lawful eligibility/consent; MyDose technology; operator access scoped
- **limits or unknowns**: Starter legal pages not ready counsel documents; exports of signed originals, timestamps/provenance and complete audit trail not demonstrated
- **source urls**: https://docs.mydose.ai/clinic-guide/review-intakes | https://docs.mydose.ai/clinic-guide/patient-profile | https://docs.mydose.ai/studio/store-editor
- **access date**: 2026-11-07 PST

## I07 — MyDose; downstream eRx vendor unnamed / Prescriber/eRx
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: NPI/DEA/state-license verification fields, personal signature, prescriber permissions
- **access interface**: Clinical Account Settings and prescribing workflow
- **input data**: Prescriber credentials, provider-signed clinical order
- **output data**: Prescription/treatment activation
- **source of truth**: Clinician/eRx system
- **phi scope**: PHI + sensitive clinician credentials
- **responsibility and payer**: Clinician personally signs; medical entity owns licensing/EPCS/PDMP obligations; vendor must evidence its eRx chain
- **limits or unknowns**: Signature image/DEA field is not proof of certified EPCS or legal authority; eRx intermediary/EPCS cert/vendor/pricing unknown
- **source urls**: https://docs.mydose.ai/clinic-guide/prescriber-credentials | https://mydose.ai/clinical-software/ | https://www.dea.gov/press-releases/2025/12/31/dea-extends-telemedicine-flexibilities-ensure-continued-access-care
- **access date**: 2026-11-07 PST

## I08 — NewLife Pharmacy / Pharmacy
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Named pharmacy integration in February2026 changelog
- **access interface**: Integration existence in release history; no public MyDose pharmacy API spec
- **input data**: Valid prescription and required fulfillment data
- **output data**: Pharmacy/order status
- **source of truth**: Dispensing pharmacy
- **phi scope**: PHI
- **responsibility and payer**: Pharmacy responsible for lawful dispensing; MyDose routing; per-order pass-through
- **limits or unknowns**: Precise legal entity/license/current brand access/formulary/states/API rights unknown; not all Studio drugs proven fulfilled by NewLife
- **source urls**: https://docs.mydose.ai/changelog | https://docs.mydose.ai/clinic-guide/orders-management | https://mydose.ai/faq/
- **access date**: 2026-11-07 PST

## I09 — Unnamed 503A partners; clinic marketing also503B / Pharmacy network
- **evidence status**: VENDOR CLAIM
- **capability**: Pharmacy routing/fulfillment/refills/tracking
- **access interface**: Managed integration; pharmacy and inventory guides incomplete
- **input data**: Valid order, quantities, shipping info
- **output data**: Fill/shipment/refill status
- **source of truth**: Pharmacy dispensing record
- **phi scope**: PHI
- **responsibility and payer**: Pharmacy licenses/quality; prescriber suitability; brand shipping/billing support
- **limits or unknowns**: No partner roster, stock/BUD/quality/recall/cold-chain SLA or lawful product-by-state matrix; 503A/503B scope differences require clarification
- **source urls**: https://mydose.ai/enterprise/ | https://mydose.ai/clinical-software/ | https://docs.mydose.ai/clinic-guide/orders-management
- **access date**: 2026-11-07 PST

## I10 — Google Calendar / Scheduling
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Connect Google shown in clinic Calendar guide
- **access interface**: Documented UI OAuth-style connection; API scopes not specified
- **input data**: Provider availability and booking
- **output data**: Appointments/calendar updates
- **source of truth**: Chosen clinical scheduler
- **phi scope**: Visit title/date/identity may be PHI
- **responsibility and payer**: Clinical operator manages clinician schedule; Workspace contract/BAA scope must be checked
- **limits or unknowns**: Calendar payload fields, conflict resolution, timezone/DST and consumer-vs-Workspace account support not documented
- **source urls**: https://docs.mydose.ai/clinic-guide/calendar | https://www.hhs.gov/hipaa/for-professionals/special-topics/cloud-computing/index.html
- **access date**: 2026-11-07 PST

## I11 — Calendly; Acuity / Scheduling
- **evidence status**: VENDOR CLAIM
- **capability**: Named calendar integration options
- **access interface**: Marketing claim, connector contract not published
- **input data**: Availability/bookings
- **output data**: Calendar sync
- **source of truth**: Chosen scheduler
- **phi scope**: PHI possible
- **responsibility and payer**: Clinic contracts appropriate plan/BAA if used; integration payer unknown
- **limits or unknowns**: Availability in Studio versus clinic/Enterprise, sync direction, plan eligibility and scope unknown
- **source urls**: https://mydose.ai/clinical-software/
- **access date**: 2026-11-07 PST

## I12 — Vendor unnamed / Video
- **evidence status**: VENDOR CLAIM
- **capability**: Protected synchronous consultations and join links
- **access interface**: In-app flow; no named video SDK/API
- **input data**: Patient/provider session metadata and audiovisual encounter
- **output data**: Consult completion
- **source of truth**: Clinical encounter record
- **phi scope**: PHI
- **responsibility and payer**: Clinical group owns encounter and escalation; platform video vendor requires applicable BAA
- **limits or unknowns**: No vendor, pricing, recording retention/consent, device fallback or uptime commitment supplied
- **source urls**: https://mydose.ai/clinical-software/ | https://mydose.ai/safety/ | https://docs.mydose.ai/clinic-guide/review-intakes
- **access date**: 2026-11-07 PST

## I13 — Vendor/lab network unnamed / Labs
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Order Blood Test, view results, charts; marketing also manual result upload
- **access interface**: Clinic health/labs UI; no public external lab contract
- **input data**: Signed lab order/patient/location
- **output data**: Results and original reports
- **source of truth**: Performing lab + clinical chart
- **phi scope**: PHI
- **responsibility and payer**: Ordering clinician owns indication/critical results; platform routes; labs billed at cost
- **limits or unknowns**: No evidence of automatic Labcorp/Quest integration; analyte mappings, lab partner/CLIA, coverage, alerts and perpanel price unknown
- **source urls**: https://docs.mydose.ai/clinic-guide/patient-health | https://docs.mydose.ai/studio/payouts | https://mydose.ai/clinical-software/
- **access date**: 2026-11-07 PST

## I14 — MyDose; underlying vendor unnamed / Secure care messaging
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Clinical portal inbox/attachments; Studio Support metadata only
- **access interface**: Clinical Messages; Open MyDose handoff
- **input data**: Secure care/support message and attachment
- **output data**: Thread and reply
- **source of truth**: Clinical/support record
- **phi scope**: PHI even in some nonmedical conversations
- **responsibility and payer**: Care team handles medical queries; brand shipping/billing replies in clinic dashboard
- **limits or unknowns**: Retention, secure delegation, emergency/after-hours SLA, complete export and underlying provider unknown
- **source urls**: https://docs.mydose.ai/studio/patients-and-orders | https://docs.mydose.ai/clinic-guide/messaging
- **access date**: 2026-11-07 PST

## I15 — MyDose branded platform email; ESP unnamed / Email/lifecycle
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Daily operator summaries; optional abandoned-signup reminder off by default
- **access interface**: Notification switches; test mode suppresses patient emails
- **input data**: Enrollment/status event
- **output data**: Branded platform email
- **source of truth**: MyDose notification history
- **phi scope**: Even abandoned intake can be sensitive
- **responsibility and payer**: Operator responsible for permitted marketing; platform operational notifications
- **limits or unknowns**: Studio explicitly noSMS/no marketing sequences; cannot claim full lifecycle CRM; sender-domain ownership/delivery/export unknown
- **source urls**: https://docs.mydose.ai/studio/patients-and-orders | https://docs.mydose.ai/studio/faq | https://docs.mydose.ai/studio/test-mode-and-go-live
- **access date**: 2026-11-07 PST

## I16 — Google Ads/Analytics; Meta; TikTok / Analytics/ad feeds
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: UTM/funnel aggregate reports; general nonhealth page visits only; no signup/purchase events to platforms
- **access interface**: Integrations IDs/keys; feed off by default and may be platform-wide disabled
- **input data**: Allowlisted consented generic-page visit + opaque campaign IDs
- **output data**: Page visits to eligible platform; internal aggregate funnel
- **source of truth**: First-party governed aggregate reporting
- **phi scope**: Do not classify patient rows/order details as anonymous
- **responsibility and payer**: Operator owns law/policy/consent; MyDose feed restrictions
- **limits or unknowns**: No conversion-optimization workaround; public website policy broader than Studio docs—request product-specific payload/event map; not evidence of breach
- **source urls**: https://docs.mydose.ai/studio/seo-and-ad-pages | https://docs.mydose.ai/studio/patients-and-orders | https://mydose.ai/privacy-policy/ | https://www.hhs.gov/hipaa/for-professionals/privacy/guidance/hipaa-online-tracking/index.html
- **access date**: 2026-11-07 PST

## I17 — WorkOS / Identity/SSO
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: WorkOS-backed auth/directory sync in January2026 clinic release history
- **access interface**: Historical documented integration; no current Studio tenant config inspected
- **input data**: Authorized identity/org claims
- **output data**: Sessions/provisioning
- **source of truth**: Identity provider + clinic role model
- **phi scope**: Identity can be sensitive/PHI-linked
- **responsibility and payer**: MyDose upstream vendor agreement; future internal buyer needs own suitable plan/BAA
- **limits or unknowns**: Does not prove every Studio surface uses WorkOS or uses WorkOS MCP; tenant mapping/MFA defaults/SCIM/BAA unknown
- **source urls**: https://docs.mydose.ai/changelog | https://docs.mydose.ai/studio/team-and-roles | https://workos.com/security
- **access date**: 2026-11-07 PST

## I18 — MyDose / RBAC/audit/multi-tenant
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Separate dashboard/editor roles; clinical role permissions; multi-storefront
- **access interface**: Admin configuration; audit claims
- **input data**: Roles/actions/version changes
- **output data**: Authorized UI and audit events
- **source of truth**: Identity/tenant authorization and append-only audit
- **phi scope**: PHI access and operational metadata
- **responsibility and payer**: Platform enforces isolation; operator approves least privilege; clinical entity controls clinician permissions
- **limits or unknowns**: Need cross-tenant test, MFA enforcement, emergency access/export, security audit and retention evidence
- **source urls**: https://docs.mydose.ai/studio/team-and-roles | https://docs.mydose.ai/clinic-guide/overview | https://mydose.ai/safety/
- **access date**: 2026-11-07 PST

## I19 — AWS named for public website only / Hosting/security
- **evidence status**: VENDOR CLAIM
- **capability**: Website privacy names AWS service provider; safety claims TLS/encryption/backups
- **access interface**: No clinical architecture or cloud-service inventory published
- **input data**: Website data; clinical scope unverified
- **output data**: Hosted service
- **source of truth**: Actual deployment configuration unknown
- **phi scope**: Website nonPHI boundary; clinical vendor scope unknown
- **responsibility and payer**: MyDose supplies subprocessor/BAA and security evidence; internal buyer owns shared responsibility
- **limits or unknowns**: Do not infer Studio/clinical AWS stack or Next/Supabase/Twilio; SOC2TypeII in progress, not achieved
- **source urls**: https://mydose.ai/privacy-policy/ | https://mydose.ai/safety/ | https://www.hhs.gov/hipaa/for-professionals/special-topics/cloud-computing/index.html
- **access date**: 2026-11-07 PST

## I20 — Rybbit; Google Analytics / Website analytics
- **evidence status**: VENDOR CLAIM
- **capability**: Named in public website privacy policy
- **access interface**: Website disclosure, not verified Studio runtime
- **input data**: Site activity/cookies
- **output data**: Site analytics
- **source of truth**: Website analytics
- **phi scope**: Potential health inferences; do not send patient data
- **responsibility and payer**: Website operator law/consent duties
- **limits or unknowns**: Site scope not proof of clinical platform vendor or permissions
- **source urls**: https://mydose.ai/privacy-policy/
- **access date**: 2026-11-07 PST

## I21 — MyDose; AI engine/model vendor unnamed / AI summary
- **evidence status**: DOCUMENTED AVAILABLE
- **capability**: Intake summary explicitly not clinical conclusion; full responses must be reviewed
- **access interface**: Clinical review screen; public site chatbot separate
- **input data**: Submitted patient answers
- **output data**: AI reading aid
- **source of truth**: Original intake/clinician decision, not AI summary
- **phi scope**: PHI
- **responsibility and payer**: Medical prescriber verifies; vendor discloses model/subprocessor/BAA/no-training/de-identification practices
- **limits or unknowns**: Safety describes deidentified data for AI improvement; actual method/rights/retention/model/version/validation unknown
- **source urls**: https://docs.mydose.ai/clinic-guide/review-intakes | https://mydose.ai/safety/ | https://mydose.ai/privacy-policy/
- **access date**: 2026-11-07 PST

## I22 — MyDose general clinical API/webhooks/FHIR / Clinical integration/export
- **evidence status**: UNKNOWN/NEEDS CONTRACT ACCESS
- **capability**: Enterprise integration/custom frontend claims, not public callable API/export contract
- **access interface**: Not documented in reviewed public Studio/clinic guides
- **input data**: Desired patient/consent/chart/order deltas
- **output data**: Desired complete export/status callbacks
- **source of truth**: Medical entity/provider records + vendor systems
- **phi scope**: PHI
- **responsibility and payer**: Medical entity authorizes export; vendor supplies contractual interface; buyer funds migration
- **limits or unknowns**: MCP cannot read clinical records; CSVimport/intakePDF/billingexports do not prove complete clinical export. Need schemas, signed webhooks, pagination/replay/rate/version limits and posttermination access
- **source urls**: https://mydose.ai/enterprise/ | https://mydose.ai/faq/ | https://docs.mydose.ai/studio/build-with-ai | https://docs.mydose.ai/clinic-guide/patient-profile | https://docs.mydose.ai/changelog
- **access date**: 2026-11-07 PST

## A01 — Beluga Health / Alternative managed backend
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: Hosted intake or direct clinical API/network/pharmacy; no revenue share claim
- **access interface**: Public integration overview; full API documentation by contract
- **input data**: Clinically approved intake and patient location
- **output data**: Visit decision/Rx/status and pharmacy events
- **source of truth**: Beluga medical/EHR/pharmacy records
- **phi scope**: PHI
- **responsibility and payer**: Own marketing; Beluga contracted clinical scope; platform monthly+pervisit+coordination charges quoted
- **limits or unknowns**: Not confirmed MyDose vendor. Own frontend does not eliminate provider/pharmacy/API fees or legal role. No numeric public rates
- **source urls**: https://belugahealth.com/platform | https://belugahealth.com/pricing
- **access date**: 2026-11-07 PST

## A02 — Healthie / Alternative EHR/headless
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: GraphQL EHR, scheduling/forms/chat and webhooks; API Group/Enterprise add-on
- **access interface**: Public GraphQL docs; sandbox requires access; signed webhook docs
- **input data**: Synthetic development fixtures; later authorized PHI
- **output data**: Clinical records/events with controlled API scope
- **source of truth**: Healthie EHR if selected
- **phi scope**: PHI production only under suitable contracts; sandbox no PHI
- **responsibility and payer**: Medical practice EHR buyer; separate licensed clinicians/pharmacies still needed
- **limits or unknowns**: No automatic MyDose data import; API price quote; webhook retries can disable after3days; eRx integration contract separately
- **source urls**: https://help.gethealthie.com/article/943-healthies-api | https://docs.gethealthie.com/guides/quick-start/ | https://docs.gethealthie.com/guides/webhooks/
- **access date**: 2026-11-07 PST

## A03 — FuzeRx / Alternative pharmacy rails
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: REST patient/Rx/fill/refill/shipment APIs and sandbox simulations
- **access interface**: Public official API docs; contract provisions sandbox/production keys
- **input data**: Valid prescriptions, patient/shipping/payment references
- **output data**: Fill/shipping/exception webhooks
- **source of truth**: Dispensing pharmacy records
- **phi scope**: PHI
- **responsibility and payer**: Authorized licensed prescriber/pharmacy; operator coordinates only permitted commerce
- **limits or unknowns**: Not MyDose vendor; do not infer compounding/formulary/control availability; pharmacy access/pricing/BAA contract-specific
- **source urls**: https://rxdocs.fuzehealth.com/
- **access date**: 2026-11-07 PST

## A04 — Junction / Alternative lab rails
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: Order collection, results JSON/PDF, redraw/order lifecycle; coverage ZIP check
- **access interface**: Documented REST/webhooks/sandbox
- **input data**: Authorized lab orders + patient + collection location
- **output data**: Structured results, PDFs, order statuses
- **source of truth**: Performing lab plus EHR
- **phi scope**: PHI
- **responsibility and payer**: Clinical owner ordering/critical-result escalation; buyer contracts and pays labs/API
- **limits or unknowns**: Not MyDose vendor; modality/ZIP/test and physician workflow constraints; no quoted price assumed
- **source urls**: https://docs.junction.com/lab/overview/introduction
- **access date**: 2026-11-07 PST

## A05 — DoseSpot / Alternative eRx/EPCS
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: Official API portal; Healthie documents sandbox DoseSpot eRx testing
- **access interface**: Partner onboarding + product-specific API scope
- **input data**: Clinician-signed prescription; licensed prescriber identity
- **output data**: eRx transmission/status
- **source of truth**: Certified eRx records plus EHR
- **phi scope**: PHI + clinician identity
- **responsibility and payer**: Clinical practice and prescriber; separate eRx contracts/EPCS/PDMP configuration
- **limits or unknowns**: Not MyDose vendor. Need exact EPCS certification/identityproofing/2FA/state/policy fit; never automate clinical signing through general agent
- **source urls**: https://docs.dosespot.com/ | https://help.gethealthie.com/article/943-healthies-api | https://www.dea.gov/press-releases/2025/12/31/dea-extends-telemedicine-flexibilities-ensure-continued-access-care
- **access date**: 2026-11-07 PST

## A06 — Twilio HIPAA-eligible services / Alternative communication
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: Eligible communications under BAA and Security/Enterprise Edition
- **access interface**: Official APIs; official MCP currently public docs search only
- **input data**: Minimized operational notification data
- **output data**: Delivery status; secure care UI link
- **source of truth**: Clinical/notification ledger
- **phi scope**: PHI only permitted covered service/workflow
- **responsibility and payer**: Buyer contracts BAA and funds messages/edition; clinical support owner separate
- **limits or unknowns**: Not MyDose vendor; SMS is not a patient portal; no automatic SendGrid/Segment HIPAA eligibility; no send actions authorized
- **source urls**: https://www.twilio.com/en-us/hipaa | https://www.twilio.com/docs/ai/mcp
- **access date**: 2026-11-07 PST

## A07 — AWS eligible services / Alternative hosting
- **evidence status**: RECOMMENDED SUBSTITUTE
- **capability**: API Gateway/Lambda/RDS/S3/KMS/queues/logging/backup eligible service set
- **access interface**: Cloud service APIs after BAA/configuration; infrastructure proposal only
- **input data**: Authorized app data under approved boundary
- **output data**: Secure application and audit
- **source of truth**: Selected source systems, not duplicated marketing warehouse
- **phi scope**: PHI only eligible services/configuration
- **responsibility and payer**: Buyer engineering/security ownership and BAA; clinical entity authorization
- **limits or unknowns**: Not proof MyDose clinical stack. Cloud/endpoint/AI/support systems each need scoped review; SOC2 claim not substituted by AWS compliance
- **source urls**: https://aws.amazon.com/compliance/hipaa-eligible-services-reference/ | https://www.hhs.gov/hipaa/for-professionals/special-topics/cloud-computing/index.html
- **access date**: 2026-11-07 PST