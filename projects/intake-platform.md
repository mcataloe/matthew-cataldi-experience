# AI-Assisted Enterprise Intake Platform

## Context

A federal enterprise needed a more consistent way to intake solution requests, recommend approved capabilities, reduce duplicated effort, and connect intake decisions to downstream enterprise systems.

The system was ATO'd and deployed to production on AWS ECS. Its production topology included a pre-existing monolith ECS service and a second ECS service that Matthew changed to operate as the worker service.

## Matthew's contribution

Matthew served as a senior technical contributor across architecture, implementation, integrations, developer workflow, and stakeholder translation.

He:

- Implemented functionality within an existing FastAPI, React/Vite, PostgreSQL, DynamoDB, and AWS stack.
- Owned API contracts, data models, ingestion patterns, migration strategy, and integration boundaries for assigned workstreams.
- Led and implemented major integration paths across Microsoft 365 / Power Platform, Jira, GitLab, and ServiceNow.
- Proposed an AWS SQS-based integration approach that became the adopted pattern and implemented the Jira and ServiceNow paths after the lead engineer established the reusable general implementation.
- Changed the second production ECS service to operate as the worker service; he did not create the original monolith or originate the two-service architecture.
- Applied FIFO SQS, idempotent design, duplicate prevention, retry strategy, ordering, visibility-period handling, dead-letter retention, and at-least-once processing tradeoffs.
- Architected and evaluated configuration/secrets placement across AWS Secrets Manager, AWS Systems Manager Parameter Store, GitLab-provided environment variables, and application/runtime configuration.
- Used ChatGPT, Codex, and GitHub Copilot as part of the daily engineering workflow, with ChatGPT and Codex used most heavily. At least some AI-assisted contributions entered the production delivery path after Matthew reviewed, modified as needed, tested, and approved them.

## Technical environment

FastAPI, React, Vite, PostgreSQL, DynamoDB, AWS ECS, SQS-oriented integrations, Pydantic, SQLAlchemy, Alembic, Jira, ServiceNow, Microsoft 365 / Power Platform, GitLab, structured logging, and correlation identifiers.

## Evidence boundaries

- Matthew did not create or select the original foundational stack and should not be represented as sole owner of the complete platform.
- He did not own the platform's Okta integration or personally own the ATO authorization.
- Do not infer AWS Fargate or a specific ECS launch type for Intake.
- Do not claim he created the worker service from scratch, extracted it from the monolith, or originated the two-service architecture.
- Production ECS application/service implementation does not establish deep ownership of the ECS cluster, task definitions, deployment pipeline, autoscaling, capacity, incidents, or cost optimization.
- Matthew proposed the SQS architecture but did not implement the first reusable general SQS pattern; he implemented the adopted pattern for Jira and ServiceNow.
- Do not claim exactly-once guarantees.
- Secrets/configuration placement was architecture/evaluation work; do not imply blanket implementation, credential-rotation ownership, or organization-wide policy ownership.
- AI-assisted engineering was human-reviewed and approved. Do not claim autonomous deployment, unreviewed generated code, or that every AI output entered production.
- Exact task distribution and per-product cadence among ChatGPT, Codex, and GitHub Copilot are not established.
- Customer-specific endpoints, credentials, environment details, internal stakeholder identities, and unnecessary operational mappings are intentionally omitted.
