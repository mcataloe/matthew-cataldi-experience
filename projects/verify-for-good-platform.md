# VerifyForGood Platform Architecture

## Context

VerifyForGood is an independent nonprofit intelligence and verification platform intended to aggregate public compliance, financial, governance, operational, and registry data into explainable, API-accessible analysis.

## Matthew's contribution

As founder and platform architect, Matthew has designed and is building the platform's product, data, API, cloud, tenant, billing, and AI-assistance foundations.

Work includes:

- Multi-tenant SaaS architecture with organization-scoped access.
- Versioned API routes, API-key management, OAuth client credentials, usage metering, feature flags, and auditability.
- Data models for organizations, users, roles, subscriptions, sources, nonprofit profiles, filings, compliance status, and source attribution.
- Ingestion strategies for IRS bulk data, Form 990 XML, index files, state registries, sanctions data, and optional enrichment providers.
- Deterministic source discovery, manifest tracking, HTTP metadata checks, archive processing, malformed-data handling, schema-drift detection, and incremental reprocessing safeguards.
- Evaluation of AWS serverless and ECS/RDS architectures based on performance, cost, query needs, operational complexity, and maintainability.
- Architecture involving AWS, ECS/Fargate, RDS PostgreSQL, S3, Athena, DynamoDB, and worker-oriented ingestion.
- Explainable AI-assisted workflows with source grounding and transparent confidence boundaries.
- RAG-style retrieval for research and analyst-support use cases.
- Stripe-oriented subscription, entitlement, tax, trial, upgrade, and usage concepts.
- React/Vite frontend architecture with shared packages, administrative and customer portals, organization switching, and role-based rendering.

## Technical environment

AWS, ECS/Fargate, RDS PostgreSQL, S3, Athena, DynamoDB, React, Vite, Mantine UI, pnpm workspaces, Stripe, OAuth client credentials, API keys, public nonprofit datasets, RAG concepts, and explainable AI workflows.

## Evidence boundaries

- The platform is an active independent initiative. Planned capabilities are not automatically completed production features.
- Architecture decisions, prototypes, active implementation, and future roadmap items should be distinguished during evaluation.
- The repository does not claim proprietary access to public or third-party data sources beyond documented integrations and plans.
