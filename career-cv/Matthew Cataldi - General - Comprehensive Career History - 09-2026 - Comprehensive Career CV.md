# Matthew Cataldi

**Staff Software Engineer - Platform, Cloud, Distributed Systems & Enterprise Modernization**

Glenview, Illinois | Active Top Secret clearance (no SCI), current through February 2029  
linkedin.com/in/matthew-cataldi | github.com/mcataloe

## PROFESSIONAL PROFILE

Staff-level software engineer, platform architect, and senior technical consultant with 8+ years of professional software/IT experience from a canonical November 2017 career anchor, plus earlier paid professional software development embedded in an operations role. Experience spans cloud-native architecture, API platforms, distributed systems, enterprise integrations, infrastructure as code, internal developer platforms, data systems, engineering analytics, regulated delivery, and AI-assisted engineering.

## CORE CAPABILITY AREAS

- **Architecture & Systems:** Cloud-native and hybrid-cloud architecture, API platforms, enterprise integrations, distributed workflow design, multi-tenant systems, internal platforms, system decomposition, architecture tradeoff analysis
- **Cloud & Infrastructure:** AWS, AWS GovCloud, Azure, GCP, ECS/Fargate at project-specific depths, Terraform, Docker, GitLab, AWS networking, Equinix Fabric, Direct Connect, ExpressRoute, Cloud Interconnect, Kubernetes/EKS architecture and advisory work
- **Languages & Frameworks:** C#, JavaScript, TypeScript, Python, Node.js, Express.js, FastAPI, React/Vite, AngularJS, ASP.NET WebForms, .NET Core WebAPI, SQL/T-SQL, Prisma, Entity Framework, VBA
- **Data, Reliability & Operations:** PostgreSQL, SQL Server, DynamoDB, S3, Redis, SQS FIFO, ThingWorx, ETL/ELT, idempotency, retries, exponential backoff, replay/lookback, bounded concurrency, duplicate handling, ordering, reconciliation, migration/rollback, production readiness, incident analysis, DR planning
- **Leadership & Delivery:** Technical project leadership, solution architecture, Technical Product Owner scope, scoped formal engineering management, mentoring, onboarding, candidate evaluation, build-versus-buy analysis, vendor coordination, documentation, compliance-aware delivery
- **AI & Analytics:** Human-reviewed AI-assisted production engineering, provider-independent conversational-AI orchestration, engineering analytics, DevEx/DORA research, metadata ingestion, source-grounded AI workflow design, bounded coding-agent methodology

## PROFESSIONAL EXPERIENCE

### Improvix Technologies

**Senior Technical Consultant | January 2025 - May 15, 2026**

**Intake@State**

- Implemented functionality in an existing FastAPI, React/Vite, PostgreSQL, DynamoDB, and AWS platform deployed to production on AWS ECS.
- Owned API contracts, data models, ingestion patterns, migration strategy, and integration boundaries for assigned workstreams.
- Proposed the SQS-based integration architecture and implemented the adopted Jira and ServiceNow paths after the lead engineer established the reusable general implementation.
- Changed a second production ECS service to operate as the worker service alongside the pre-existing monolith; no Fargate or deep ECS platform-operations claim is made for Intake.
- Applied FIFO ordering, idempotent design, duplicate prevention, retries, visibility handling, DLQ behavior, and at-least-once processing tradeoffs.
- Architected configuration/secrets placement across Secrets Manager, Systems Manager Parameter Store, GitLab-provided environment variables, and application/runtime configuration.
- Used ChatGPT, Codex, and GitHub Copilot in the daily engineering workflow; at least some AI-assisted contributions entered the production delivery path after review, modification as needed, testing, and approval.

**Engineering Analytics / Metrics Platform**

- Served as technical lead and primary architectural driver for an engineering analytics initiative aggregating delivery, operational, and metadata signals across enterprise systems.
- Owned ingestion, normalization, reporting architecture, and an Express.js backend API layer.
- Redirected the initiative away from heavily customized low-code approaches after identifying firewall/WAF, scalability, extensibility, maintainability, and operational-ownership concerns.
- Led build-versus-buy analysis and direct evaluation of Jellyfish, DX, and Oobeya; no evaluated platform was purchased, piloted, implemented, deployed, or operated.

**GovCom Contract Transition**

- Continued technical leadership during the Acuity-to-Improvix transition, preserving platform architecture, infrastructure planning, reliability, financial-correctness design, stakeholder coordination, and compliance-aligned delivery within the verified test/integration boundary.

### Acuity

**Senior Technical Consultant | April 2022 - January 2025**

**SE-ECCS / GovCom**

- Served as solution architect and lead technical contributor for a regulated API-driven AWS GovCloud messaging platform validated in test/integration.
- Led REST API architecture and implementation across provider integrations including Ironbow Arrow, Twilio, WhatsApp, AWS Pinpoint, and AWS End User Messaging.
- Implemented APIs, provider adapters, authentication/token workflows, message-state workflows, cost/segment calculations, PostgreSQL/Prisma models, Redis integration, SQS FIFO workflows, and S3 behavior.
- Implemented AWS SDK application integration for SQS and the AWS Pinpoint/End User Messaging path.
- Led and implemented AWS GovCloud infrastructure across ECS/Fargate, ALB/NLB, WAF, VPC endpoints, DNS, routing/security groups, Terraform, GitLab pipelines, testing, deployment, and environment promotion.
- Implemented GitLab SAST, DAST, SCA/dependency scanning, container scanning, and contributed to AWS Security Hub findings review/remediation with the security engineer.
- Applied idempotency, retries, duplicate handling, ordering, DLQ/poison-message handling, reconciliation, persisted asynchronous state, and processing-guarantee tradeoff analysis.
- Provisioned toll-free numbers, implemented A2P SMS testing, and supported 10DLC registration/configuration in test/integration.
- The platform did not reach production customer traffic or ATO approval.

**Equinix / Consular Affairs Modernization**

- Served as Technical Product Owner and engineering lead; one engineer officially reported to Matthew for the project.
- Led non-production interconnection across AWS, Azure, GCP, and Equinix.
- Led and co-implemented AWS Direct Connect, led ExpressRoute and Cloud Interconnect designs, established Terraform structure, completed remaining shared modules, and implemented stamped-account IPsec.
- Led Online Passport Renewal network architecture through late non-production integration without claiming live traffic operations.

**SE-Tools Platform Modernization**

- Led substantial technical/evidence work for the production singleton GitLab authorization and performed production operational work including upgrades, releases, incident response, monitoring, backup/restore, DR testing, identity troubleshooting, and after-hours support.
- Led initial architecture and approximately 3,000-user sizing direction for the later GitLab HA successor and established early Terraform structure before implementation leadership transitioned.
- Implemented Terraform-managed infrastructure, account segmentation, DNS, certificates, security groups, Okta SSO, PIV authentication, pre-EKS GitLab runners, backup/restore, and Cloud9 adoption.
- Led initial Jira-to-EKS research and advised on a later GitLab EKS runner sandbox; later implementation/operations belonged to other owners.

**DIN Modernization Team**

- Served as lead engineer and senior individual contributor for proof-of-concept modernization across AWS, Azure, GCP, Terraform, Equinix, hybrid connectivity, and Stratozone.
- Wrote Terraform modules, created AWS/GCP infrastructure, designed Azure resources implemented by the Azure team, and configured/tested Direct Connect, ExpressRoute, and Equinix Fabric approaches.
- Installed/troubleshot Stratozone discovery and identified a security blocker where scanning behavior could resemble attack traffic.
- Work remained proof-of-concept/test; no production deployment or customer adoption is claimed.

## INDEPENDENT PRODUCTS AND PUBLIC WORK

### VerifyForGood

**Founder / Staff Software Engineer | February 2026 - Present | Local development**

- Owns product, architecture, roadmap, budget, and technical decisions for a nonprofit-intelligence and verification product being developed into a business.
- Implemented backend APIs, database models, multi-tenancy, tenant isolation, API keys, usage controls, IRS EO BMF/Form 990 ingestion, and React/Vite/Mantine customer/admin portals.
- Implemented and merged a provider-independent conversational-assistant layer with tenant-scoped conversation persistence, authenticated Chat API/UI, Ollama-provider integration, application-owned model routing, bounded allowlisted read-only tools, tenant-safe authority, diagnostics, schema validation, and application-level output-authority controls.
- Conversational AI remains implemented-code / executable-validation-pending; semantic/vector retrieval, RAG, Bedrock, MCP, and autonomous/broader agentic workflows are not implemented.
- No AWS deployment, staging/production environment, public application, external customers, revenue, or production users.

### LEAP Framework

- Public software-delivery framework for converting rough intent into pressure-tested, source-grounded plans and bounded coding-agent handoffs.
- Organizes work through Charter, Recon, Prompt, Implementation, and Validation/Handoff stages.
- Application-safe proof of work for requirements clarification, dependency reasoning, bounded AI-assisted execution, and validation-oriented engineering workflows.
- No sole-authorship, external-adoption, commercial-traction, or measured-effectiveness claim is made.

## EARLIER PROFESSIONAL EXPERIENCE

### IronArch Technology

**Senior Full-Stack Developer | February 2022 - April 2022**  
**Full-Stack Developer | August 2020 - February 2022**

- Developed and supported production-facing CloudKey workflows and deployed changes with the lead.
- Built a non-production AWS Commercial sandbox with structure-preserving database copying/obfuscation.
- Modernized source control to GitHub Enterprise while manual deployment remained.
- Directly configured API Gateway, Lambda, CloudFormation, IAM, Secrets Manager, RDS, EC2, and S3.
- Used Node.js directly within AWS Lambda functions in the server-side layer.
- Evaluated approximately 12 candidates and mentored one junior developer.

### Sysmex America, Inc.

**Developer / Analyst | February 2019 - August 2020**

**XW100**

- Held XW100-specific production readiness, incident/RCA, on-call, runbook, DR-testing, operational-support, migration, database, rollback, and QA/regulatory-coordination responsibility.
- Planned and implemented .NET Framework to .NET Core WebAPI/Entity Framework modernization work with production code, prototypes, database/migration/fallback scripts, validation, mirroring/replication, and isolated database-copy behavior.

**SNCS**

- Supported broader production SNCS/ThingWorx integration and a file-ingestion workflow through monitoring, failed-file recovery/reprocessing, defect resolution, deployment support, and reliability improvements without end-to-end subsystem ownership.

**Analyzer Usage Billing / Pay-Per-Sample Initiative**

- Served as technical project lead for a fleet-wide distributed system spanning thousands of analyzers and tens of millions of centralized records.
- Designed the architecture and personally implemented ThingWorx orchestration, T-SQL extraction, ETL/ELT, centralized SQL processing, bounded concurrency, exponential-backoff retries, one-day replay/lookback, composite-key idempotency, missing-device detection, reconciliation, edge-side data minimization, and monthly usage calculation.
- Another engineer implemented the analyzer-local .NET API; enterprise-billing integration and full business validation were incomplete at departure.

### APICS / ASCM

**.NET Developer | February 2018 - January 2019**

- Individual-contributor/service-desk developer using ASP.NET WebForms, VB.NET, C#, T-SQL, stored procedures, SSRS, and SSIS with some production reporting/database support.
- Planned/scaffolded React components for a portal that did not reach production.
- Tuned SQL/reporting workflows, collaborated with product/business stakeholders, coordinated with outsourced overseas contributors, and delivered a WebForms modernization lunch-and-learn/peer coaching session.

### Associated Global Systems

**Junior .NET Developer | November 2017 | Short contract**

- Performed DB2/AS400 SQL query tuning, SQL support for RPG developers, indexing recommendations, early non-production SAP reporting work, brief C#.NET optimization recommendations, and proposed website UX/UI mockups.

### Rockford Symphony Orchestra

**Personnel Manager / Software Developer | March 2013 - April 2018**

- Official role was personnel management; work evolved to roughly a 50/50 personnel/software split.
- Independently built and operated a live internal production-use Access/VBA platform supporting payroll calculation/preparation, attendance, contracts, staffing, auditions, travel/mileage/cartage rules, reporting, Office/Dropbox/Google API workflows, permissions, and season/cycle/service domain rules.
- Managed cycle staffing across a cumulative 1,200+ musician database, with the largest active cycle around 110 people; 1,200 is not a direct-report count.
- Implemented unique constraints, transaction/rollback behavior, duplicate prevention, and post-payroll reconciliation.
- This is valid earlier paid professional software-development evidence at mixed-role/internal-platform depth, not conventional software-title duration or software-engineering management.

### Independent Event-Based String Ensemble Business

**Owner / Contractor-Organizer | 1998 - Present**

- Selects musicians for engagements, coordinates availability/scheduling, manages event staffing and client expectations, and ensures performance delivery.
- This is non-IT contractor/event-operations leadership, not corporate HR or software-engineering management.

## EDUCATION

- Dev Bootcamp - Web Development, 2017 (19-week intensive program)
- Northwestern University - Master of Music, Violin Performance, 2005-2007
- Indiana University Bloomington - Bachelor of Arts, Music, 2000-2004

## CERTIFICATIONS, CLEARANCES & PROFESSIONAL DEVELOPMENT

- Active Top Secret clearance (no SCI), current through February 2029
- AWS Certified Solutions Architect - Associate
- AWS Certified Developer - Associate
- ITIL Foundation v4
- Microsoft Certified Professional; Exam 70-461, Querying Microsoft SQL Server 2012/2014
- Preparing for AWS Certified Generative AI Developer - Professional (AIP-C01) - not yet certified

## EXTENDED PROFESSIONAL EVIDENCE

- Professional profile: `../PROFILE.md`
- Project narratives: `../projects/`
- Capability evidence: `../capabilities/`
- Structured public claims: `../evidence/claims.yaml`
- Disclosure and interpretation policy: `../DISCLOSURE.md`

---

This document is a comprehensive public career publication based on currently approved records. It is not a substitute for a targeted application resume, interview, reference check, background check, or credential verification.
