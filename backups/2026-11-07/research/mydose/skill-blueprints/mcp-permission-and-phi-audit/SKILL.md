---
name: Clinic MCP permission audit
description: Use before selecting or later enabling an MCP for clinic marketing, finance, identity, infrastructure or clinical development.
---

# Clinic MCP permission audit

DRAFT — generic local authoring artifact; not installed, legal advice, clinical authorization or a guarantee of platform approval.

## Universal boundaries
This is a local draft, not an installed skill or authorization to connect accounts. Refresh official documentation and policies at execution time. Record URLs, access dates, product/version, entity, environment and unknowns. Distinguish observed UI, vendor claim, documented capability, recommended substitute and unverified/private capability. Do not infer another vendor's technology adoption from an available MCP.

Use synthetic data first. No real PHI, credentials, payment tokens or private keys in prompts, screenshots, ordinary logs, repository files or research artifacts. A platform BAA does not automatically cover the AI client, MCP proxy, model provider or tracing. Do not widen access, install connectors, scrape authenticated apps, use undocumented APIs or enumerate hidden tools. Use sanctioned connectors with least privilege only after separately authorized setup.

Internal PASS / REVISE / BLOCKED is not legal approval. Record clinical, legal/privacy, platform and business-publication approval separately. User authorization to research or draft is not authorization to publish, spend, send, refund, alter access, migrate records or prescribe. No general agent may override a clinician or pharmacist. Stop before externally visible or clinical/financial mutations absent the exact required authorization and professional workflow.

## Workflow
1. Verify the first-party documentation/repository, exact endpoint or pinned package version, auth model, environment, role/tenant scopes and published read/write/destructive tools. Endpoint existence does not imply another company uses it.
2. Separate docs-only, content-only, operational business-data and clinical-record capabilities. Read-only can still expose PHI. Prefer no-auth public docs tools or synthetic tenants first.
3. Never rely on a marketing label such as read-only without inspecting the approved current manifest. Example as ofNov7,2026: Google Ads guide calls read-only while current official README includes asset/video/label writes enabled by default; configure strict allowlist. Refresh before acting.
4. Create a permission matrix: workflow → exact tools → resource/tenant → minimal scopes → data classification → allowed destination → human approver → audit retention/revocation. Exclude broad admin, patient lists, clinical writes, financial mutations, public publication and sends by default.
5. Confirm AI client/model/proxy/logging contract chain before any PHI. Platform BAA is not enough. Use secrets manager/OAuth, never chat/repo keys. Record credential lifetime/revocation; Stripe MCP legacy non-Agent full/restricted keys have a Nov30,2026 transition deadline documented at research time—recheck current policy.
6. Proposed sandbox setup requires separate authorization; do not install, authenticate or widen access during research. A later permission grant does not authorize every externally visible action.
7. For aggregate ad reports prohibit patient-list audiences and health purchase events. For Stripe use synthetic billing; for identity/cloud only sandbox design/read review. For clinical systems no autonomous medical decisions, eRx signing or pharmacy substitutions.

## Output
Versioned MCP inventory, least-privilege allowlist, denied/high-risk tool list, data-flow/BAA gap register, approval plan and exact remaining vendor questions. No connections or production actions.

## Sources to refresh
Use ../../SOURCES.md, ../../MCP-INVENTORY.md and ../../builder-comparison/sources.csv. Open the relevant official URLs again; do not treat this dated research as runtime policy.
