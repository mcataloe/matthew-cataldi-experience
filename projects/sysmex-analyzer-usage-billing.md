# Sysmex Analyzer Usage Billing / Pay-Per-Sample Initiative

## Context

During approximately the final four months of Matthew's Sysmex employment, Sysmex was developing an initiative to automate usage-based billing from real analyzer activity rather than relying only on customer-submitted reports.

The system collected analyzer sample/run information across the fleet, centralized and reconciled the data, calculated monthly usage values, and supported comparison against customer-reported usage. Fleet-wide collection was running against real analyzers, but integration with the existing enterprise billing system and full business validation were not complete when Matthew left.

The title used here is descriptive; the official historical internal project name is not currently established.

## Matthew's contribution

Matthew was the technical project lead. He designed the distributed architecture, made major technical decisions within the project scope, led implementation, personally implemented substantial portions of the system, and coordinated the cross-system effort.

He personally implemented:

- ThingWorx scripting/orchestration and scheduled jobs;
- T-SQL extraction from analyzer-local SQL Server instances;
- data-type mapping and ETL/ELT logic;
- centralized SQL Server processing and reconciliation;
- bounded-concurrency / connection-throttling behavior;
- retry logic with exponential backoff;
- replay/lookback logic using a one-day overlap after the last successful run;
- analyzer-ID plus run-ID composite-key idempotency / duplicate prevention;
- missing-analyzer detection and last-seen analysis;
- monthly usage/billing calculation logic before enterprise-billing integration;
- edge-side data minimization so only data required for billing/reconciliation was transmitted;
- an interim SQL Server backup file as a limited recovery measure.

Another engineer implemented the analyzer-local C#/.NET REST API. Matthew designed and consumed the integration but should not be represented as the author of that edge API.

## Scale and distributed-systems evidence

Approved public scale language includes:

- fleet-wide analyzer scope;
- thousands of analyzer instruments;
- tens of millions of accumulated centralized records.

The project is direct distributed-systems design and implementation evidence. The scheduler evaluated work on roughly a 10-second cycle and selected the next eligible analyzer when connection capacity became available. The exact maximum concurrent-connection count is not established.

## Reliability and correctness

The system used:

- bounded concurrency;
- retries with exponential backoff;
- next-cycle/day retry for unavailable analyzers;
- last-successful-run tracking;
- deliberate one-day replay/lookback to reduce delayed-write boundary gaps;
- composite-key idempotency to prevent duplicate inserts;
- reconciliation against customer-reported usage;
- missing-device detection;
- monthly usage calculation.

These mechanisms should not be upgraded into formal exactly-once processing, distributed transactions, two-phase commit, saga, or compensating-transaction claims.

## Data minimization

Filtering occurred on analyzer-local SQL Server instances before transmission. The project collected only the minimum usage data needed for billing/reconciliation and did not transmit patient-identifying information as part of the usage dataset.

This supports data-minimization / privacy-by-design framing, not formal HIPAA ownership, privacy-officer authority, threat-model ownership, or measured security-risk reduction.

## Outcomes and boundaries

By Matthew's departure, fleet-wide daily collection was operating against real analyzers, tens of millions of records had accumulated centrally, connection-pressure controls were working, replay/idempotency reduced missing/duplicate usage records, and monthly usage calculations were functioning under active business validation.

Do not claim:

- completed commercial billing rollout or enterprise-billing integration;
- completed customer/business validation;
- measured billing-accuracy percentages or revenue impact;
- production-grade DR, off-host backup, tested restore, HA, replication, or formal RPO/RTO;
- a formal handoff/documentation package;
- formal personnel management or direct reports;
- an exact maximum connection count.
