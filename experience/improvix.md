# Improvix Technologies

## Senior Technical Consultant

**January 2025–May 15, 2026 | Remote**

Matthew supported Department of State modernization initiatives spanning cloud-native applications, enterprise integrations, engineering analytics, AI-assisted engineering, and compliance-aligned delivery. His final day with Improvix was May 15, 2026; none of the work below should be interpreted as current employment after that date.

## Intake@State

Matthew served as a senior technical contributor on an ATO'd enterprise intake platform deployed to production on AWS ECS.

Documented contributions included:

- Implementing functionality in an existing FastAPI, React/Vite, PostgreSQL, DynamoDB, and AWS stack.
- Owning API contracts, data models, ingestion patterns, migration strategy, and integration boundaries for assigned workstreams.
- Leading and implementing integration paths across Microsoft 365 / Power Platform, Jira, GitLab, and ServiceNow.
- Proposing an AWS SQS-based integration architecture and implementing the adopted pattern for Jira and ServiceNow after the lead engineer established the reusable general implementation.
- Changing a second production ECS service to operate as the worker service alongside the pre-existing monolith service.
- Applying FIFO queueing, idempotent design, duplicate prevention, retries, ordering, visibility-period handling, DLQ behavior, and at-least-once processing tradeoffs.
- Architecting and evaluating secrets/configuration placement across AWS Secrets Manager, AWS Systems Manager Parameter Store, GitLab-provided environment variables, and application/runtime configuration.
- Using ChatGPT, Codex, and GitHub Copilot as part of the daily engineering workflow; at least some AI-assisted contributions entered the production delivery path after Matthew reviewed, modified as needed, tested, and approved them.

The original platform stack and monolith predated Matthew. He did not own the Okta integration, the ATO approval itself, or deep ECS platform operations. The verified record does not establish AWS Fargate as the Intake ECS launch type.

See [AI-Assisted Enterprise Intake Platform](../projects/intake-platform.md).

## Engineering analytics platform

Matthew was the technical lead and primary architectural driver during an engineering analytics initiative aggregating delivery and operational signals across enterprise tooling.

Documented contributions included:

- Establishing architecture, ingestion, normalization, reporting, and backend direction.
- Building an Express.js API layer.
- Redirecting the initiative away from heavily customized low-code approaches after identifying scalability, firewall, extensibility, maintainability, and operational-ownership risks.
- Leading build-versus-buy analysis across internal and commercial approaches, including direct evaluation of Jellyfish, DX, and Oobeya.
- Evaluating DevEx/DORA concepts, metadata boundaries, AI usage, outbound telemetry, SaaS retention, security posture, operational ownership, and adoption risk.
- Preserving that funding reductions stopped procurement and no evaluated product was purchased, piloted, implemented, deployed, or operated.

See [Engineering Analytics and Build-versus-Buy Evaluation](../projects/engineering-analytics.md).

## Messaging-platform contract transition

From January through July 2025, Matthew continued technical leadership for the regulated GovCom messaging platform during the Acuity-to-Improvix contract transition.

He led platform architecture, infrastructure planning, stakeholder coordination, compliance-aligned delivery, continuity, and preservation of reliability and financial-correctness design while the platform remained within its verified test/integration boundary.
