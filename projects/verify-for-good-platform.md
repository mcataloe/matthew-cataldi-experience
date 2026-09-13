# VerifyForGood Platform Architecture

## Context

VerifyForGood is an independent nonprofit-intelligence and verification product being developed into a business. The current stage is local development with a working end-to-end prototype for the previously validated product surface. It has no AWS deployment, staging/production environment, public application URL, external customers, revenue, or production users.

## Matthew's contribution

As Founder / Staff Software Engineer, Matthew owns product, architecture, roadmap, budget, and technical decisions. He is the sole human software/code contributor for the current product, excluding AI tools. Domain requirements, business logic, use cases, and internal pilot feedback include material advisor contribution.

## Implemented and working

- Backend APIs and database models
- Multi-tenancy, organization scoping, roles, authorization, authentication, and tenant isolation
- API-key authentication
- Usage metering, subscription-domain controls, feature flags, and audit logs
- IRS Exempt Organizations Business Master File ingestion
- IRS Form 990 XML/index ingestion
- Manifest tracking, ETag/Last-Modified checks, archive processing, malformed-XML handling, drift detection, and incremental reprocessing
- Ingestion and querying of real IRS and nonprofit data
- React/Vite/Mantine customer and administrative portals
- End-to-end local UI/API demonstration for the previously validated product surface
- PostgreSQL-, object-storage-, and worker/queue-oriented behavior at local-prototype depth

## Implemented code with executable validation pending

The merged local conversational-assistant architecture includes:

- persistent tenant-scoped conversations and messages;
- authenticated FastAPI Chat API and portal Chat UI/history;
- provider abstraction with a deterministic test provider and Ollama provider;
- application-owned `low | medium | high` routing tiers independent of provider-specific identifiers;
- bounded tool orchestration with maximum iteration limits and diagnostics;
- allowlisted read-only tools over existing nonprofit and organization services;
- server-owned user and active-organization context;
- schema validation and policy enforcement for model-requested tool calls;
- application-level output-authority policy preventing unsupported platform-owned trust, fraud, safety, compliance, eligibility, donation, procurement, or endorsement determinations;
- committed deterministic failure-path coverage for provider and tool-policy failures.

Repository-side implementation review is complete. Executable pytest/Alembic/frontend validation and a real local Ollama round trip remain pending, so the repository does not claim a fully working Chat runtime, production answer quality, or production operational readiness.

## Partially implemented

- Stripe/payment behavior
- Infrastructure as code

## Designed, documented, evaluated, or roadmap only

- OAuth client credentials
- State-registry, sanctions, federal-award, Charity Navigator, Candid, and other enrichment integrations
- Semantic/hybrid retrieval, embeddings, vector databases, and RAG
- Long-term conversational memory beyond persisted history
- Graph-oriented relationship intelligence
- Bedrock and Bedrock Guardrails
- MCP integration
- Autonomous or broader agentic workflows
- ECS/Fargate, DynamoDB, CI/CD, monitoring, and operational tooling

Athena was evaluated and not pursued.

## Technical environment

Python/FastAPI-oriented APIs, React, Vite, Mantine UI, PostgreSQL-oriented persistence, object-storage-oriented behavior, worker/queue-oriented ingestion, API keys, IRS public nonprofit datasets, partial Stripe/payment work, partial infrastructure as code, and a provider-independent conversational-assistant layer with bounded read-only tool use.

## Evidence boundaries

- Do not claim incorporation, production, staging, public application availability, AWS deployment, external customers, paying customers, revenue, or production users.
- Do not describe the conversational assistant as fully runtime-validated until executable local validation and Ollama smoke testing are completed and recorded.
- Do not claim semantic/vector retrieval, embeddings, vector database, RAG, Bedrock, MCP, autonomous agents, or broader agentic workflows as implemented.
- Do not claim arbitrary SQL, HTTP, shell, code execution, web browsing, or write-capable model tools; the current model-facing surface is explicit, allowlisted, and read-only.
- Do not erase advisor/domain contribution to nonprofit and CSR requirements.
- AI-assisted code or architecture may be attributed to Matthew only where he reviewed, tested, modified as needed, and accepted the implementation.
- Current repository visibility is evidence access, not a long-term open-source or product-publication strategy.
