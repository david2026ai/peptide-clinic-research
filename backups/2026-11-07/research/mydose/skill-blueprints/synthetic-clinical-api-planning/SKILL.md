---
name: Synthetic clinic API planning
description: Use when designing or testing a future clinic integration against official sandbox APIs, without live patients or implementation authorization.
---

# Synthetic clinic API planning

DRAFT — generic local authoring artifact; not installed, legal advice, clinical authorization or a guarantee of platform approval.

## Universal boundaries
This is a local draft, not an installed skill or authorization to connect accounts. Refresh official documentation and policies at execution time. Record URLs, access dates, product/version, entity, environment and unknowns. Distinguish observed UI, vendor claim, documented capability, recommended substitute and unverified/private capability. Do not infer another vendor's technology adoption from an available MCP.

Use synthetic data first. No real PHI, credentials, payment tokens or private keys in prompts, screenshots, ordinary logs, repository files or research artifacts. A platform BAA does not automatically cover the AI client, MCP proxy, model provider or tracing. Do not widen access, install connectors, scrape authenticated apps, use undocumented APIs or enumerate hidden tools. Use sanctioned connectors with least privilege only after separately authorized setup.

Internal PASS / REVISE / BLOCKED is not legal approval. Record clinical, legal/privacy, platform and business-publication approval separately. User authorization to research or draft is not authorization to publish, spend, send, refund, alter access, migrate records or prescribe. No general agent may override a clinician or pharmacist. Stop before externally visible or clinical/financial mutations absent the exact required authorization and professional workflow.

## Workflow
1. Confirm selected product/API entitlement, signed commercial scope, sandbox isolation, documented schema version, test credentials through sanctioned setup and BAA/PHI boundary. No keys collected in chat or copied from example documentation.
2. Derive a capability map from official schemas. Healthie development MCP and Medplum FHIR MCP are alternatives; MyDose Studio MCP is not a clinical export API. A docs-only MCP cannot send messages or run APIs.
3. Propose an adapter contract, not production code: required inputs/outputs, source IDs, data owner, auth/scopes, rate limits, signed-webhook validation, pagination, schema version, retry/replay and dead-letter handling. Document every unknown instead of inventing fields/events.
4. Keep paid-invoice, clinician approval, prescription, pharmacy fill, shipment, lab result and patient consent states independent. Financial success must not automatically prescribe or dispense.
5. Produce synthetic fixtures for denial, changed patient state, duplicate/out-of-order events, canceled plans, failed charges, backorders, amended/critical lab results, expired prescriber credentials, missing attachments and tenant-isolation failure.
6. Define idempotency and reconciliation before enabling writes. Record native IDs, version/time, actor/tenant, event signature and one owner per billing obligation and authorized fill. No autonomous clinical interpretation or signing.
7. Validate eligible vendor/AI scope and contract chain before real data. Sandbox-only keys and role-restricted fake patients; never assume production PHI is allowed because sandbox queries work.

## Output
Schema/source map, synthetic test plan, adapter/event specification, failure/escalation matrix and gated implementation estimate. Do not install/deploy/connect or execute API writes under this planning skill.

## Sources to refresh
Use ../../SOURCES.md, ../../MCP-INVENTORY.md and ../../builder-comparison/sources.csv. Open the relevant official URLs again; do not treat this dated research as runtime policy.
