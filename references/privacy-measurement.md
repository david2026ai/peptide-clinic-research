# Privacy and measurement boundary

Read with AGENTS and S11–S12/S18–S19. **No default import of a generic ecommerce or legal-lead tracking stack.** This reference does not declare any named product inherently unlawful or approved; the actual contract, data, role, use and configuration matter.

## Classify first
Determine treating entity, MSO/marketing entity, pharmacy, portal and each vendor's role. Cash-pay does not alone settle HIPAA coverage; covered transactions and business-associate roles matter. Other federal/state privacy/consumer-health and breach rules may apply outside HIPAA. The FTC HBNR applies to qualifying PHR vendors/apps and related entities, not automatically every non-HIPAA clinic; unauthorized disclosure can be a breach, not only hacking. Washington illustrates consumer-health protections and health inferences; counsel maps actual covered geography, exclusions, consent and rights. [S11–S12]

HHS tracking guidance includes a June 2024 partial vacatur: an IP address plus an unauthenticated public health-page visit is not automatically enough to trigger HIPAA as described in the vacated interpretation. Don't generalize every public visit into PHI. Equally, booking/registration/intake/portal data can be identifiable health information. A privacy-policy paragraph or cookie banner is not automatically HIPAA authorization; a BAA alone does not authorize every purpose. HHS guidance is not itself a replacement for applicable law. [S11]

## House launch architecture
- Public marketing education and minimal service/state availability checks are separated from secure clinical intake, booking detail, portal, prescriptions and health-linked payment flows.
- No third-party ad pixels, generic session replay, form-recording certificates or broad attribution scripts on clinical/booking/portal/payment flows by default. No patient-data auctions, resale, buyer ping-post or lead-list cloning.
- No medical-patient Customer Match/lookalike/exclusion uploads or health-derived retargeting audiences. Uploading an exclusion list is still data sharing. Don't infer sexual/fertility/hormonal status from behavior for ad audiences.
- No diagnoses, medications, health answers, labs, appointment reasons, patient/order IDs or sensitive combinations in URL/query, campaign names, referrers, custom events, page titles, logs, CAPI or analytics exports. A neutral label doesn't cleanse the underlying transaction/context.
- Hashing emails/phones, server-side forwarding, consent banners or replacing Purchase with Lead are not universal fixes. Google prohibits sensitive medical conversions for enhanced-conversion/store-sales measurement uploads; inspect current policy before proposals for other mechanisms. [S19]
- No disabling CSP, relaxing security headers or bypassing platform restrictions to restore attribution. No unapproved call recordings/transcripts or model uploads containing patient data. Synthetic tests only in this pack.
- No blanket guarantee “HIPAA compliant” or “we never share anything” unless reviewed and true for the actual operation.

## Event-by-event review matrix
For each proposed event/document: origin page; exact data/identifiers; health context/inferences; destination/vendor; purpose; role; contract/BAA where applicable; legal basis/authorization; state consent/rights; platform permission and account classification; retention; access; deletion; security; tests; reviewer/date. Clinical/legal/privacy approval and applicable platform permission are independent. If any material column is UNKNOWN, keep that transmission disabled for launch.

## Privacy-safe learning options — conditional, not automatic clearance
Prefer synthetic usability sessions, manually reconciled internal finance/care totals and properly designed aggregate/cohort reporting under access controls. Evaluate contextual advertising and permitted predefined audiences rather than health remarketing. Aggregation thresholds, suppression of small cells and whether data are genuinely de-identified require privacy review; “anonymous” is not self-proving. Keep identifiable clinical data in appropriate secure systems, not creative spreadsheets or this future repo.

For performance analysis use spend → privacy-permitted public engagement → internally measured attended evaluations → fully costed contribution, with clear attribution limits. No patient-level data need be sent back to an ad platform merely because a media buyer wants ROAS. Missing measurement is a design constraint, not permission to overcollect.

## Release tests
Check real assembled pages and event payloads using approved synthetic data: browser requests, server logs/exports, redirects, query/referrer handling, embedded scheduling/payment frames, email/SMS link tags, call tools and access roles. Do not claim a clean text audit verifies implementation. Log each approved event and regression-test after new widgets/SDKs. An incident triggers the established privacy/security response and counsel review; do not improvise public notification or delete evidence.
