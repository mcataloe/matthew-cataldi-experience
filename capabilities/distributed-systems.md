# Distributed Systems and Reliability

## Direct evidence areas

Matthew has applied distributed-systems and reliability reasoning across regulated messaging, enterprise integrations, fleet-scale healthcare data collection, healthcare migration/operations, and public-data ingestion.

Documented patterns include:

- Idempotency and composite-key duplicate prevention
- Retry semantics and exponential backoff
- Replay/lookback windows
- Bounded concurrency / connection throttling
- Duplicate handling and ordering
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

### Sysmex analyzer usage billing

As technical project lead, Matthew designed and implemented a fleet-wide distributed ThingWorx/SQL Server workflow operating across thousands of analyzers and tens of millions of centralized records. Direct implementation included bounded concurrency, exponential-backoff retries, one-day replay/lookback, analyzer-plus-run composite-key idempotency, missing-device detection, reconciliation, edge-side data minimization, and monthly usage calculation.

Source: [Sysmex Analyzer Usage Billing](../projects/sysmex-analyzer-usage-billing.md)

### Regulated cloud messaging

Test/integration messaging workflows required provider integration, duplicate avoidance, ordering, persisted state, reconciliation, usage tracking, segmentation, and cost correctness.

Source: [Regulated Cloud Messaging Platform](../projects/govcom-messaging.md)

### Enterprise intake and integration

Production enterprise workflows used AWS ECS and SQS-oriented integration patterns requiring consistent state transitions, downstream integration, error handling, duplicate protection, ordering, visibility-period awareness, DLQ behavior, and at-least-once processing tradeoffs.

Source: [AI-Assisted Enterprise Intake Platform](../projects/intake-platform.md)

### XW100 healthcare migration and operations

Production readiness, migration, database copying, validation, fallback/rollback, incident analysis, DR testing, runbooks, and operational support required correctness across regulated healthcare workflows.

Source: [Earlier Career](../experience/earlier-career.md)

### Rockford internal operations platform

A live internal Access/VBA platform used database keys and unique constraints, transaction/rollback behavior, duplicate prevention, and post-payroll reconciliation to protect payroll, attendance, and scheduling correctness.

Source: [Personnel Operations Platform](../projects/personnel-operations-platform.md)

### Public-data ingestion

VerifyForGood implements manifests, ETag/Last-Modified checks, archive processing, malformed-data handling, schema-drift detection, and incremental reprocessing in a local working prototype.

Source: [VerifyForGood Platform Architecture](../projects/verify-for-good-platform.md)

## Boundaries

The repository distinguishes applied reasoning and bounded implementation from claims that every named pattern was implemented as a dedicated framework.

Do not claim:

- exactly-once guarantees where not explicitly established;
- transactional outbox, saga, two-phase commit, distributed transaction protocols, or compensating transactions where not approved;
- production behavior for GovCom or VerifyForGood;
- formal CQRS across an entire system merely because read/write paths were separated;
- distributed exactly-once or messaging semantics for Rockford's local-database correctness patterns;
- completed commercial billing integration or measured revenue impact for the Sysmex analyzer-usage initiative.

Interview discussion should focus on the concrete failure mode, system stage, tradeoff, and implemented or proposed mitigation for each project.
