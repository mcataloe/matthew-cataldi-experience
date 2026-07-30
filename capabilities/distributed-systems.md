# Distributed Systems and Reliability

## Direct evidence areas

Matthew has applied distributed-systems and reliability reasoning across regulated messaging, enterprise integrations, healthcare migration and operations, and public-data ingestion.

Documented patterns include:

- Idempotency and idempotency-key considerations
- Retry semantics and duplicate handling
- Ordering guarantees
- At-least-once and exactly-once tradeoff analysis without claiming exactly-once guarantees
- Dead-letter and poison-message handling
- Visibility-timeout awareness
- Reconciliation-oriented processing
- Persisted asynchronous workflow state
- Operational-write separation from reporting and analytics reads
- Message segmentation, usage, billing-period, and cost correctness
- Migration, fallback, rollback, validation, recovery, and operational-readiness planning
- Manifest tracking, HTTP metadata checks, archive processing, malformed-data handling, schema-drift detection, and incremental reprocessing

## Strongest project evidence

### Regulated cloud messaging

Test/integration messaging workflows required provider integration, duplicate avoidance, ordering, persisted state, reconciliation, usage tracking, segmentation, and cost correctness.

Source: [Regulated Cloud Messaging Platform](../projects/govcom-messaging.md)

### Enterprise intake and integration

Multi-step enterprise workflows required consistent state transitions, downstream integration, error handling, duplicate protection, ordering, visibility-timeout awareness, correlation, and separation of operational and reporting concerns.

Source: [AI-Assisted Enterprise Intake Platform](../projects/intake-platform.md)

### XW100 healthcare migration and operations

Production readiness, migration, database copying, validation, fallback/rollback, incident analysis, DR testing, runbooks, and operational support required correctness across regulated healthcare workflows.

Source: [Earlier Career](../experience/earlier-career.md)

### Public-data ingestion

VerifyForGood implements manifests, ETag/Last-Modified checks, archive processing, malformed-data handling, schema-drift detection, and incremental reprocessing in a local working prototype.

Source: [VerifyForGood Platform Architecture](../projects/verify-for-good-platform.md)

## Boundaries

The repository distinguishes applied reasoning and bounded implementation from claims that every named pattern was implemented as a dedicated framework.

Do not claim:

- exactly-once guarantees;
- a transactional outbox or saga where not approved;
- production behavior for GovCom or VerifyForGood;
- formal CQRS across an entire system merely because read/write paths were separated;
- detailed Rockford reliability or financial-correctness implementation until the deeper technical platform receives separate review.

Interview discussion should focus on the concrete failure mode, system stage, tradeoff, and implemented or proposed mitigation for each project.
