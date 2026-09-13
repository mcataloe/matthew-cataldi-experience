# VerifyForGood

## Founder / Staff Software Engineer

**February 2026–Present | Independent product engineering | Local working prototype**

Matthew owns product, architecture, roadmap, budget, and technical decisions for a nonprofit-intelligence and verification product being developed into a business. The product is not yet incorporated.

## Implemented and working in local development

- Backend APIs and database models
- Multi-tenancy, organization scoping, roles, authorization, authentication, and tenant isolation
- API-key authentication
- Usage metering, subscription-domain controls, feature flags, and audit logs
- IRS Exempt Organizations Business Master File ingestion
- IRS Form 990 XML/index ingestion, manifests, HTTP metadata checks, archive processing, malformed-data handling, schema-drift detection, and incremental reprocessing
- Real IRS and nonprofit data ingestion and querying
- React/Vite/Mantine customer and administrative portals
- End-to-end local UI/API demonstration for the previously validated product surface
- PostgreSQL-, object-storage-, and worker/queue-oriented behavior at local-prototype depth

## Conversational-assistant implementation

A local conversational-assistant implementation is merged into the current product codebase at **implemented-code / validation-pending** depth. It includes:

- persistent user- and organization-scoped conversations and message history;
- an authenticated FastAPI Chat API and portal Chat UI;
- an LLM-provider abstraction with deterministic test-provider behavior and an Ollama provider for local-model integration;
- application-owned `low | medium | high` model-routing tiers;
- bounded tool orchestration with iteration limits and diagnostics;
- allowlisted read-only tools over existing nonprofit, organization, usage, subscription, and settings services;
- server-owned user/organization authority so model or client input cannot elevate tenant scope;
- schema validation and policy enforcement for model-requested tool calls;
- application-level output-authority controls that prevent the model from presenting unsupported trust, fraud, compliance, eligibility, donation, procurement, or endorsement conclusions as authoritative determinations;
- deterministic failure-path test coverage in committed code.

Repository-side implementation review is complete, but executable local validation, including database/frontend validation and a real Ollama smoke test, remains pending. This is not represented as a fully validated runtime or production AI system.

## Partial implementation

- Stripe/payment behavior
- Infrastructure as code

## Designed, documented, evaluated, or roadmap only

- OAuth client credentials
- State-registry, sanctions, federal-award, Charity Navigator, Candid, and other enrichment integrations
- Semantic/vector retrieval, embeddings, vector-database integration, and RAG
- Source-grounded citation behavior beyond current application policy
- Long-term conversational memory beyond persisted chat history
- Graph intelligence
- Bedrock and Bedrock Guardrails
- MCP integration
- Autonomous or broader agentic workflows
- ECS/Fargate, DynamoDB, CI/CD, monitoring, and operational tooling

The current product has no AWS deployment, staging or production environment, public application URL, external customers, paying customers, revenue, or production users.

Matthew is the sole human software/code contributor for the current product, excluding AI tools. Domain requirements, business logic, use cases, and internal pilot feedback include material advisor contribution. AI-assisted code or architecture is attributed to Matthew only where he reviewed, tested, modified as needed, and accepted the resulting implementation.

See [VerifyForGood Platform Architecture](../projects/verify-for-good-platform.md).
