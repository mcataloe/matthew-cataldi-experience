# Distributed Systems and Reliability

## Direct evidence areas

Matthew has applied distributed-systems reasoning across regulated messaging, enterprise integrations, cloud migration, healthcare modernization, public-data ingestion, and payroll-sensitive operations.

Documented patterns include:

- Idempotency and idempotency-key considerations
- Retry semantics and duplicate handling
- Ordering guarantees
- At-least-once and exactly-once tradeoffs
- Dead-letter and poison-message handling
- Visibility-timeout awareness
- Reconciliation-oriented processing
- Workflow boundaries and compensating actions
- Command/write separation from reporting and analytics reads
- Cost and financial correctness
- Capacity and operational-readiness tradeoffs

## Strongest project evidence

### Regulated cloud messaging

Messaging workflows required reliable provider integration, duplicate avoidance, ordering, reconciliation, usage tracking, and cost correctness.

Source: [Regulated Cloud Messaging Platform](../projects/govcom-messaging.md)

### Enterprise intake and integration

Multi-step enterprise workflows required consistent state transitions, downstream integration, error handling, duplicate protection, and separation of operational and reporting concerns.

Source: [AI-Assisted Enterprise Intake Platform](../projects/intake-platform.md)

### Personnel and payroll-support workflows

Repeated administrative actions required protection against duplicate or inconsistent personnel, attendance, mileage, contract, and payroll-support records.

Source: [Personnel Operations Platform](../projects/personnel-operations-platform.md)

### Public-data ingestion

The VerifyForGood design includes manifests, source metadata, archive processing, malformed-data handling, schema-drift detection, and incremental reprocessing safeguards.

Source: [VerifyForGood Platform Architecture](../projects/verify-for-good-platform.md)

## Boundaries

The repository distinguishes applied reliability reasoning from claims that every named pattern was implemented as a dedicated framework. Interview discussion should focus on the concrete problem, failure mode, tradeoff, and implemented or proposed mitigation for each project.
