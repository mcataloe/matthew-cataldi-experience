# VerifyForGood Platform Architecture

## Context

VerifyForGood is an independent nonprofit-intelligence and verification product being developed into a business. The current stage is a working local prototype with no AWS deployment, staging/production environment, public application URL, external customers, revenue, or production users.

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
- End-to-end local UI/API demonstration
- PostgreSQL-, object-storage-, and worker/queue-oriented behavior at local-prototype depth

## Partially implemented

- Stripe/payment behavior
- Infrastructure as code

## Designed, documented, evaluated, or roadmap only

- OAuth client credentials
- State-registry, sanctions, federal-award, Charity Navigator, Candid, and other enrichment integrations
- Working AI-assisted analysis, explainability, source-confidence logic, RAG, embeddings, vector search, conversational memory, and graph intelligence
- ECS/Fargate, DynamoDB, CI/CD, monitoring, and operational tooling

Athena was evaluated and not pursued.

## Technical environment

Python/FastAPI-oriented APIs, React, Vite, Mantine UI, PostgreSQL-oriented persistence, object-storage-oriented behavior, worker/queue-oriented ingestion, API keys, IRS public nonprofit datasets, partial Stripe/payment work, partial infrastructure as code, and documented AWS/AI architecture not yet deployed or implemented.

## Evidence boundaries

- Do not claim incorporation, production, staging, public availability, AWS deployment, external customers, paying customers, revenue, or production users.
- Do not claim working AI/RAG, explainability, embeddings, vector search, graph intelligence, completed billing, OAuth client credentials, or deployed operational tooling.
- Do not erase advisor/domain contribution to nonprofit and CSR requirements.
- AI-assisted code or architecture may be attributed to Matthew only where he reviewed, tested, modified as needed, and accepted the implementation.
- Current repository visibility is evidence access, not a long-term open-source or product-publication strategy.
