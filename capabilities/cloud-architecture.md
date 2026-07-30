# Cloud and Hybrid Architecture

## Cloud platforms and contribution depth

Matthew has documented cloud experience across AWS, AWS GovCloud, Azure, GCP, and Equinix. The depth varies by project:

- Direct architecture and implementation: AWS GovCloud ECS/Fargate messaging infrastructure, Terraform, load balancing, network/security components, relational/caching/object-storage services, and delivery automation.
- Direct and shared implementation: non-production AWS Direct Connect, Equinix/Terraform modules, stamped-account IPsec, DNS/routing design, and multi-cloud enablement.
- Design with implementation retained by another team: Azure ExpressRoute, Google Cloud Interconnect, Azure resource design, and enterprise MACsec advisory work.
- Initial architecture or advisory work: GitLab HA successor architecture, Jira-to-EKS research, and later GitLab EKS runner governance advice.
- Proof-of-concept/test implementation: DIN AWS/GCP resources, Terraform, Direct Connect, ExpressRoute, Equinix Fabric, Stratozone, Cloud9 within SE-Tools, and Packer proof of concept.
- Designed or evaluated but not deployed: VerifyForGood AWS container/serverless, DynamoDB, CI/CD, monitoring, and related operational architecture.

## Strongest direct evidence

### AWS GovCloud application architecture

Matthew led and implemented infrastructure and delivery automation for a test/integration regulated messaging platform using ECS/Fargate, Terraform, GitLab CI/CD, ALB/NLB, WAF, VPC endpoints, DNS, routing/security groups, PostgreSQL/RDS, Redis, SQS FIFO, S3, and security controls.

EKS was evaluated and rejected for that platform rather than implemented.

Source: [Regulated Cloud Messaging Platform](../projects/govcom-messaging.md)

### Hybrid and multi-cloud connectivity

Matthew served as Technical Product Owner and engineering lead for non-production interconnection across AWS, Azure, GCP, Equinix, vendors, customer organizations, governance, and Terraform-supported provisioning.

Source: [Hybrid-Cloud Interconnection Modernization](../projects/equinix-modernization.md)

### Enterprise platform modernization

Matthew led technical/evidence work for a production singleton GitLab authorization and initial architecture for a later HA successor. He implemented or supported AWS/Terraform/identity/backup/DR/runner/platform work at documented shared depths.

Jira/EKS and later GitLab EKS runner contributions were research and advisory work, not implementation or operations.

Source: [GitLab and Engineering Platform Modernization](../projects/gitlab-platform-modernization.md)

### Modernization proof of concept

Matthew wrote Terraform, created AWS and GCP resources, designed Azure resources, configured/tested hybrid connectivity, and installed/troubleshot Stratozone in proof-of-concept/test environments.

Source: [DIN Modernization Proof of Concept](../projects/din-modernization.md)

### Independent product architecture

Matthew has implemented local PostgreSQL-, object-storage-, and worker/queue-oriented product behavior and evaluated/documented future AWS architectures for VerifyForGood. AWS infrastructure is not deployed.

Source: [VerifyForGood Platform Architecture](../projects/verify-for-good-platform.md)

## Boundaries

A technology's appearance in this repository does not imply equal depth or direct configuration.

Preserve distinctions among:

- architecture, implementation, evaluation, research, advisory work, and operation;
- proof of concept, test/integration, non-production, and production;
- direct configuration and use-only context;
- Matthew-owned work and implementation retained by platform, networking, vendor, or successor teams.
