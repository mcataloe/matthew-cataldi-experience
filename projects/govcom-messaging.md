# Regulated Cloud Messaging Platform

## Context

A federal organization needed an API-driven messaging capability connecting regulated AWS GovCloud infrastructure with commercial communication providers while maintaining security, reliability, tenant separation, operational visibility, and cost accountability.

The verified delivery stage was test/integration. The platform did not reach production customer traffic or ATO approval during Matthew's approved scope.

## Matthew's contribution

Matthew served as solution architect and lead technical contributor.

He:

- Led REST API architecture and implementation, customer-facing API contracts, and provider integrations involving Ironbow Arrow, Twilio, WhatsApp, AWS Pinpoint, and AWS End User Messaging.
- Implemented API endpoints/controllers, provider adapters, authentication/token workflows, message-state/status workflows, cost and segment calculations, PostgreSQL/Prisma models, Redis-backed read behavior, SQS FIFO and related queue workflows, and S3 upload behavior.
- Led and implemented AWS GovCloud infrastructure and delivery automation across ECS/Fargate, ALB/NLB, WAF, VPC endpoints, DNS, routing/security groups, Terraform modules, GitLab pipelines, tests, load/reliability validation, deployment scripts, releases, and environment promotion.
- Implemented a persisted asynchronous workflow state model using queued, processing, complete, and error states with failure information.
- Implemented CQRS-style read/write separation using distinct data paths and Redis-backed read behavior without claiming formal CQRS architecture across the entire system.
- Applied idempotency, retry semantics, duplicate handling, ordering, visibility-timeout awareness, dead-letter and poison-message handling, reconciliation, and at-least-once/exactly-once tradeoff analysis without claiming exactly-once guarantees.
- Owned reconciliation and financial-correctness design for message segmentation, customer billing-period validation, usage, and communication-cost tracking.
- Built and exercised ARM64 and x86_64 container variants in test/integration and retained x86_64 after security-tool compatibility concerns.
- Evaluated EKS and rejected it as unnecessary complexity relative to ECS/Fargate; no GovCom Kubernetes implementation is claimed.
- Provisioned AWS toll-free numbers, implemented A2P SMS testing, and directly supported 10DLC brand/campaign registration and configuration for test/integration validation.
- Created and presented a tenant-aware Balsamiq prototype that stakeholders reviewed but did not fund or adopt.
- Scaffolded a Next.js frontend and then led the pivot to an Express.js API-only service when requirements changed.

## Technical environment

AWS GovCloud, ECS/Fargate, ECR, Docker, Terraform, GitLab CI/CD, TypeScript, JavaScript, Express.js, a limited Next.js scaffold, PostgreSQL/RDS, Prisma, Redis, SQS FIFO, S3, ALB/NLB, WAF, VPC endpoints, DNS, identity/security controls, AWS Pinpoint, AWS End User Messaging, Twilio, WhatsApp, and Ironbow Arrow.

## Evidence boundaries

- Matthew led the effort while collaborating with product, business-analysis, provider, messaging, infrastructure, security, and customer stakeholders.
- Most Dockerfile ownership and maintenance belonged to another engineer; Matthew modified Dockerfiles as needed.
- Do not claim formal domain-driven design or verified bounded contexts; the approved scope is modular/domain-oriented TypeScript class separation.
- Do not claim a transactional outbox, saga, blue/green deployment, canary deployment, EKS implementation, production multi-architecture deployment, production messaging traffic, ArchAngel implementation, or ATO approval.
- This public description omits customer-specific topology, account details, endpoints, credentials, internal evidence inventories, and security configurations.
