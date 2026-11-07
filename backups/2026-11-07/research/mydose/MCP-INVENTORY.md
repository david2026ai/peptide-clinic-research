# Documented MCP inventory

2026-11-07 PST. Research only. No connections, installations, PHI handling or migrations. Public capability does not prove another company's adoption; full commercial/export/clinical authority requires contract evidence.

## MyDose Studio
- **classification**: COMPANY-CONFIRMED MCP
- **documented endpoint or repo**: https://mcp.mydose.ai/hub/mcp
- **tools and scope**: Pages/themes/menus/media/redirects/discounts/team/brand; business orders/patients/payout/funnel reads. Marketing82 hub + 104 CMS tool count not independently enumerated.
- **auth and permissions**: Remote HTTP; OAuth store selection + read-only/full; Owner/Admin writes; Staff read; keys1–30 days (default 7), sign-in access token 1 hour renewing; destructive confirm 5 minutes.
- **phi boundary**: No clinical records. Business patient/order lists still potentially PHI; no payment/bank/card/signup/terms/go-live checkout.
- **recommended inhouse workflow**: Read public content/config only initially; produce claims-audited website draft diffs, preview, human approve publication.
- **limits**: Does not remove subscription fees; not a clinical export API; no endpoint invocation/tool enumeration done.
- **source urls**: https://docs.mydose.ai/studio/build-with-ai | https://mydose.ai/studio/
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Healthie Dev Assist
- **classification**: COMPANY-CONFIRMED DEVELOPMENT MCP
- **documented endpoint or repo**: https://github.com/healthie/healthie-dev-assist
- **tools and scope**: DevAssist2.0 execute_healthie_code; healthie.search/introspect/query/mutate documented in vendor guide.
- **auth and permissions**: Local Node/stdio-style client; schema discovery without key; sandbox key for query/mutate; production API subscription separate.
- **phi boundary**: Synthetic sandbox only by default; no real PHI in sandbox/prompts.
- **recommended inhouse workflow**: Discover actual GraphQL schemas, create synthetic onboarding/booking fixtures, test mapping and access denials.
- **limits**: Not evidence MyDose or Hedonic use Healthie; not a production clinician agent.
- **source urls**: https://www.gethealthie.com/blog/build-on-healthie-faster-with-ai-coding-agents-and-mcp | https://help.gethealthie.com/article/943-healthies-api
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Medplum
- **classification**: COMPANY-CONFIRMED MCP; ALTERNATIVE BACKEND
- **documented endpoint or repo**: https://api.medplum.com/mcp/stream
- **tools and scope**: fhir-request full FHIR CRUD; search/fetch compatibility tools.
- **auth and permissions**: OAuth2; membership/access policies; remote MCP; explicit synthetic test project/scoped credentials.
- **phi boundary**: Real PHI requires entire approved AI/data/BAA chain; earlier vendor preview warning and current direct-access cautions.
- **recommended inhouse workflow**: FHIR modeling and synthetic export/import validation; no live chart writes.
- **limits**: FHIR datastore is not physician network/pharmacy/EPCS authority; no MyDose adoption evidence; no broad CRUD production access.
- **source urls**: https://www.medplum.com/docs/ai/mcp | https://www.medplum.com/docs/building-with-ai-coding-assistants
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Hedonic Digital
- **classification**: UNKNOWN: NO COMPANY-CONFIRMED MCP IDENTIFIED
- **documented endpoint or repo**: No endpoint/schema identified in supplied public offers
- **tools and scope**: Offer describes business integrations; no verified operational MCP inventory.
- **auth and permissions**: Unknown
- **phi boundary**: Unknown; require service/clinical/marketing boundary and actual subprocessor roster.
- **recommended inhouse workflow**: Ask for actual vendor names, documented contracts/APIs/MCP scopes and owned assets/export rights.
- **limits**: Do not infer Lovable hosting means access to production clinical integrations or their development accounts.
- **source urls**: https://hedonic-digital-peptides.lovable.app/HDpeptides/delivery/wholesale-pricing | https://hd-roadmap.lovable.app/hedonic-digital | https://hedonic-digital-peptides.lovable.app/HDpeptides/delivery/scope-of-work-partnerships
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Beluga Health
- **classification**: PUBLIC API PATH; OPERATIONAL MCP NOT VERIFIED
- **documented endpoint or repo**: https://belugahealth.com/platform
- **tools and scope**: Clinical API and pharmacy event overview; full docs through commercial process.
- **auth and permissions**: Partner contract/API credentials; public MCP endpoint not verified.
- **phi boundary**: PHI only contracted clinical integration.
- **recommended inhouse workflow**: Evaluate as managed clinical backend; first build thin webhook adapter using supplied official schemas.
- **limits**: Third-party support vendor connector claims are not proof Beluga publishes/uses a native MCP.
- **source urls**: https://belugahealth.com/platform | https://belugahealth.com/pricing
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## MD Integrations
- **classification**: PUBLIC API/WHITE-LABEL PATH; OPERATIONAL MCP NOT VERIFIED
- **documented endpoint or repo**: https://docs.mdintegrations.com/public/integration-paths
- **tools and scope**: API, white-label apps, Shopify/WooCommerce plugins; partner reference details may require registration.
- **auth and permissions**: Commercial partner access; no confirmed vendor operational MCP in reviewed page.
- **phi boundary**: Clinical intake/fulfillment PHI boundary required even if commerce plugin used.
- **recommended inhouse workflow**: Compare API-first exit path with managed clinical backend, not all-internal medicine.
- **limits**: Documentation-site MCP if offered is not automatically clinical production API. No MyDose adoption evidence.
- **source urls**: https://docs.mdintegrations.com/public/integration-paths
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## OpenLoop
- **classification**: PLATFORM/API INTEGRATION CLAIM; MCP NOT VERIFIED
- **documented endpoint or repo**: https://openloophealth.com/technology-platform
- **tools and scope**: Launchpad managed platform; supports own existing website/portal and clinical integrations.
- **auth and permissions**: Commercial scope; no public MCP schema identified.
- **phi boundary**: Clinical network boundary; exact BAAs/export contracts required.
- **recommended inhouse workflow**: Alternative managed provider backend quote and export diligence.
- **limits**: No numerical price assumed; marketing claims not service guarantees.
- **source urls**: https://openloophealth.com/technology-platform
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Bask Health
- **classification**: PUBLIC REPOSITORY SIGNAL; PRODUCTION MCP UNVERIFIED
- **documented endpoint or repo**: https://github.com/Bask-Health/mcp-server
- **tools and scope**: Public repository accessible but README.md absent; hosted production schema/permissions/support not established.
- **auth and permissions**: Not verified; do not connect unverified Vercel deployment from search.
- **phi boundary**: Unknown—no clinical access recommended.
- **recommended inhouse workflow**: Ask vendor for supported current MCP docs/security/BAA and feature scope; API/headless platform separately documented.
- **limits**: Not treated as proven production server or evidence of MyDose/Hedonic adoption; no code checkout or execution.
- **source urls**: https://github.com/Bask-Health/mcp-server | https://bask.health/integrations
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## GenHealth.ai
- **classification**: COMPANY-DOCUMENTED WORKFLOW MCP; IDENTITY CAVEAT
- **documented endpoint or repo**: https://api.umpa.genhealth.ai/developer/mcp
- **tools and scope**: Workflow capability/action discovery, validation, authoring/publish/run; names include get_workflow_capabilities_v2/search_workflow_actions/get_workflow_action.
- **auth and permissions**: StreamableHTTP bearer organization-bound key; workflow:read versus write/publish/run + workflows-plan feature.
- **phi boundary**: Synthetic workflow only until clinical integration rights/BAAs established.
- **recommended inhouse workflow**: Optional non-PHI workflow validation; low priority for cash-pay MVP.
- **limits**: Prior-authorization/workflow platform; not verified same legal entity as similarly named GEN Health telehealth network; no adoption inference.
- **source urls**: https://genhealth.ai/docs/workflows/agent-quickstart
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Stripe
- **classification**: OFFICIAL SERVICE MCP; NOT ADOPTION EVIDENCE
- **documented endpoint or repo**: https://mcp.stripe.com
- **tools and scope**: stripe_api_search/details/read/write; documentation search/planning, analytics; payment/refund/subscription writes possible.
- **auth and permissions**: OAuth scoped account/sandbox or Agent API key; connected-account context has separate restrictions; existing full-access/restricted non-Agent keys stop accepted Dec2026, migrate byNov30.
- **phi boundary**: Do not expose patient-linked invoice lines/customer rows or Rxmetadata; sandbox/aggregate business reports only by default.
- **recommended inhouse workflow**: Read sandbox billing model, validate subscription/cancel/refund test cases; human approval before financial changes.
- **limits**: MCP access does not grant MyDose platform-account rights; no PHI/BAA presumption; some actions have additional Stripe confirmation.
- **source urls**: https://docs.stripe.com/mcp | https://docs.stripe.com/connect/subscriptions
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Twilio
- **classification**: OFFICIAL DOCS MCP ONLY; NOT ADOPTION EVIDENCE
- **documented endpoint or repo**: https://mcp.twilio.com/docs
- **tools and scope**: twilio__search and twilio__retrieve public docs/OpenAPI; does NOT execute API calls or send messages.
- **auth and permissions**: StreamableHTTP; no authentication; public beta/no supportSLA.
- **phi boundary**: Never send PHI in a documentation query; no production account needed.
- **recommended inhouse workflow**: Find exact eligible messaging API and schemas, draft synthetic notification adapters and consent matrix.
- **limits**: SendGrid/Segment documentation presence is not HIPAA eligibility; future execution requires separately contracted API/BAA/product scope.
- **source urls**: https://www.twilio.com/docs/ai/mcp | https://www.twilio.com/en-us/hipaa
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## WorkOS
- **classification**: OFFICIAL MANAGEMENT MCP; NOT ADOPTION EVIDENCE
- **documented endpoint or repo**: https://mcp.workos.com/mcp
- **tools and scope**: Manage organizations/users/SSO connections/branding and enabled dashboard operations.
- **auth and permissions**: StreamableHTTP OAuth; role inherited; sandbox default; admin production/write disables; destructive confirmation; no credential mint/rotate/readout.
- **phi boundary**: Identity linked to care can be sensitive; synthetic organizations only by default.
- **recommended inhouse workflow**: Review sandbox tenant isolation and staff onboarding/offboarding design; no real invitations/access changes.
- **limits**: MyDose changelog names WorkOS auth, NOT use of this MCP; product/AI BAAs remain separate.
- **source urls**: https://workos.com/docs/mcp | https://docs.mydose.ai/changelog | https://workos.com/security
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## AWS
- **classification**: OFFICIAL SERVICE MCP; NOT ADOPTION EVIDENCE
- **documented endpoint or repo**: https://aws-mcp.us-east-1.api.aws/mcp
- **tools and scope**: Knowledge docs/skills/regions; authenticated run_script AWS API, tasks, presigned URLs.
- **auth and permissions**: Docs without auth; OAuth or IAM/SigV4 for actions; IAM least privilege, CloudTrail; SigV4 option supports hiding write tools.
- **phi boundary**: Docs-only first; no PHI logs/object retrieval; AWS service eligibility does not cover AI client by itself.
- **recommended inhouse workflow**: Research eligible architecture/cost inputs; later read-only sandbox inventory and IaC plan review.
- **limits**: Can mutate infrastructure/share data via presigned URLs; approval gates required; no credentials provisioning/install now.
- **source urls**: https://docs.aws.amazon.com/agent-toolkit/latest/userguide/mcp-server.html | https://docs.aws.amazon.com/agent-toolkit/latest/userguide/getting-started-aws-mcp-server.html | https://aws.amazon.com/compliance/hipaa-eligible-services-reference/
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Google Ads
- **classification**: OFFICIAL MARKETING MCP; VERSION CONFLICT
- **documented endpoint or repo**: https://github.com/googleads/google-ads-mcp
- **tools and scope**: Guide calls read-only search/get_resource_metadata/list_accessible_customers; current README additionally documents asset/video/label writes with propose+checksum+confirm.
- **auth and permissions**: Local stdio or own StreamableHTTP deployment; OAuth/service-account permissions; pin reviewed version; disable assets and labels namespaces for read-only.
- **phi boundary**: Ad-report aggregates only; no patient conversions/audience lists/clinical identifiers into agent/ad platform.
- **recommended inhouse workflow**: Read aggregate spend/campaign metrics; generate draft campaign brief and anomaly report.
- **limits**: Do not rely on read-only guide alone; latest README says all tools enabled by default. Self-host auth must be secured. Publication/medical ad eligibility separate.
- **source urls**: https://developers.google.com/google-ads/api/docs/developer-toolkit/mcp-server | https://github.com/googleads/google-ads-mcp/blob/main/README.md
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Meta Ads
- **classification**: OFFICIAL MARKETING MCP; NOT ADOPTION EVIDENCE
- **documented endpoint or repo**: https://mcp.facebook.com/ads
- **tools and scope**: Reporting, campaign/ad creation/editing, catalogs, signals, experiments, activity logs; official announcement also custom audiences.
- **auth and permissions**: OAuth or appropriately scoped token; MCP account rules can withhold write/budget/creative changes; app review for some other-business access; rollout varies.
- **phi boundary**: No patient lists, health custom audiences, Rxpurchase events or sensitive-attribute inference.
- **recommended inhouse workflow**: Aggregate ad reporting and approved creative draft review; begin rules-enforced read-only.
- **limits**: MCP availability is not permission to advertise drugs; no health retargeting/CAPI loophole. Primary overview500 in WebFetch but200 public fallback; official announcement readable.
- **source urls**: https://developers.facebook.com/blog/post/2026/07/16/meta-ads-mcp-server/ | https://developers.facebook.com/documentation/ads-commerce/ads-ai-connectors/ads-mcp-server/ads-mcp-server-overview
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## FuzeRx / Junction / DoseSpot
- **classification**: PUBLIC OFFICIAL API DOCS; OPERATIONAL MCP NOT VERIFIED
- **documented endpoint or repo**: https://rxdocs.fuzehealth.com/ | https://docs.junction.com/lab/overview/introduction | https://docs.dosespot.com/
- **tools and scope**: Pharmacy/labs/eRx API scopes documented; no native production MCP established from reviewed docs.
- **auth and permissions**: Partner/API access; least privilege per vendor.
- **phi boundary**: PHI/EPCS high risk; no clinical writes through general agent.
- **recommended inhouse workflow**: Contract-tested server-side adapters/webhooks; optional custom MCP wrapper is NEW engineering, not an existing vendor capability.
- **limits**: Not MyDose vendor identities. Clinical licenses/BAA/pharmacy relationships not supplied by protocol wrappers.
- **source urls**: https://docs.junction.com/lab/overview/introduction | https://rxdocs.fuzehealth.com/ | https://docs.dosespot.com/
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## HighLevel / LeadConnector
- **classification**: OFFICIAL BUILDER MCP; NOT EVIDENCE OF MYDOSE/HEDONIC ADOPTION
- **documented endpoint or repo**: https://services.leadconnectorhq.com/mcp/cursor/v2
- **tools and scope**: Official MCP, client-specific OAuth endpoints; four tools list_locations/search_operations/describe_operation/execute_operation;550+ operations across 38 domains in Oct29guide.
- **auth and permissions**: OAuth subaccount/scopes; singleaccount available, multiactor rollout; read/write/delete/message/payment/publish operations require scope and approval.
- **phi boundary**: No real PHI in initial skills; platform BAA does not cover external AI client automatically.
- **recommended inhouse workflow**: Synthetic tenant, funnel content/schema QA and aggregate reports; not clinical charts. BAA package and agent/client coverage separate; no sends or workflow enrollment.
- **limits**: No connection/install made. Available tools/product plans/role/scopes must be rechecked at runtime; publishing and externallyvisible actions need explicit approval.
- **source urls**: https://help.gohighlevel.com/support/solutions/articles/155000005741-how-to-setup-and-use-the-highlevel-mcp-server
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Wix
- **classification**: OFFICIAL BUILDER MCP; NOT EVIDENCE OF MYDOSE/HEDONIC ADOPTION
- **documented endpoint or repo**: https://mcp.wix.com/mcp
- **tools and scope**: Official remote MCP: public docs, code assistance, real site API actions and site/account/project creation/publishing.
- **auth and permissions**: Interactive account sign-in or scoped API key/accountID; remoteHTTP.
- **phi boundary**: No real PHI in initial skills; platform BAA does not cover external AI client automatically.
- **recommended inhouse workflow**: Documentation and synthetic marketing-page drafts; no PHI/admin access by default. Wix PHI product enablement does not establish AI client coverage; payments restrictions remain.
- **limits**: No connection/install made. Available tools/product plans/role/scopes must be rechecked at runtime; publishing and externallyvisible actions need explicit approval.
- **source urls**: https://dev.wix.com/docs/overview/ai-the-wix-platform/the-wix-mcp
- **access date**: 2026-11-07 PST
- **connected or installed**: NO

## Jotform
- **classification**: OFFICIAL BUILDER MCP; NOT EVIDENCE OF MYDOSE/HEDONIC ADOPTION
- **documented endpoint or repo**: https://mcp.jotform.com
- **tools and scope**: Official StreamableHTTP/OAuth; forms/submissions text server plus separate form/app/Sign/FormBackend MCP endpoints.
- **auth and permissions**: OAuth; account permissions; PHI enabled plan PLUS explicit PHI object scopes; Enterprise features not mandatory for baselineMCP.
- **phi boundary**: No real PHI in initial skills; platform BAA does not cover external AI client automatically.
- **recommended inhouse workflow**: Create synthetic intake form drafts and audit field/consent schema. Never read patient responses or send sign requests without separate approved workflow/BAA chain.
- **limits**: No connection/install made. Available tools/product plans/role/scopes must be rechecked at runtime; publishing and externallyvisible actions need explicit approval.
- **source urls**: https://www.jotform.com/developers/mcp/
- **access date**: 2026-11-07 PST
- **connected or installed**: NO