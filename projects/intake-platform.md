# AI-Assisted Enterprise Intake Platform

## Context

A federal enterprise needed a more consistent way to intake solution requests, recommend approved capabilities, reduce duplicated effort, and connect intake decisions to downstream enterprise systems.

## Matthew's contribution

Matthew served as a senior technical contributor across architecture, implementation, integrations, developer workflow, and stakeholder translation.

He:

- Implemented functionality within an existing FastAPI, React/Vite, PostgreSQL, DynamoDB, and AWS stack.
- Owned API contracts, data models, ingestion patterns, migration strategy, and integration boundaries for assigned workstreams.
- Led and implemented major integration paths across Microsoft 365 / Power Platform, Jira, GitLab, and ServiceNow.
- Proposed an AWS SQS-based integration approach that became a reusable pattern and implemented the Jira and ServiceNow paths after the lead engineer established the general implementation.
- Applied reliability concepts involving idempotency, retries, duplicate handling, ordering, visibility timeouts, dead-letter handling, reconciliation, workflow state, and at-least-once processing tradeoffs.
- Helped distinguish operational writes, workflow transitions, reporting access, and analytics-oriented reads without claiming a formal standalone CQRS implementation.
- Led branching and environment strategy for cloud-coupled development and created a visual process separating routine changes from work requiring isolated implementation.
- Supported structured logging, correlation identifiers, performance/load testing, environment promotion, and regulated-delivery concerns.

## Technical environment

FastAPI, React, Vite, PostgreSQL, DynamoDB, AWS, SQS-oriented integrations, Pydantic, SQLAlchemy, Alembic, Jira, ServiceNow, Microsoft 365 / Power Platform, GitLab, structured logging, and correlation identifiers.

## Evidence boundaries

- Matthew did not create or select the original foundational stack and should not be represented as sole owner of the complete platform.
- He did not own the platform's Okta integration or claim implementation of every listed system component.
- RAG, saga, CQRS, outbox, and exactly-once language must not be converted into claims of independently built frameworks or guarantees where the approved record supports only design discussion or bounded patterns.
- Customer-specific endpoints, credentials, environment details, internal stakeholder identities, and operational mappings are intentionally omitted.
