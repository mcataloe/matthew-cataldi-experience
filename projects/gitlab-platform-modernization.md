# GitLab and Engineering Platform Modernization

## Context

An enterprise engineering environment needed to modernize manually managed and singleton tooling toward more available, repeatable, identity-integrated, authorized, and supportable platform patterns.

## Matthew's contribution

Matthew supported production singleton GitLab operations and broader modernization across GitLab, AWS infrastructure, identity, Terraform, Cloud9, Packer, Jira/EKS research, documentation, and platform governance.

### Production singleton GitLab

- Led substantial technical and evidence portions of the singleton GitLab authorization effort, including system-boundary definition, network/data-flow diagrams, evidence gathering, remediation planning, control narratives, backup/restore demonstrations, security coordination, and submission support.
- The production singleton received its ATO while Matthew led the technical/evidence work; he did not unilaterally grant the authorization.
- Implemented or supported Terraform-managed infrastructure, AWS account segmentation, EC2/autoscaling, load balancing, database/storage components, DNS, certificates, security groups, Okta SSO, PIV authentication, GitLab runners, backup/restore, upgrades, releases, incident response, DR exercises, and operational troubleshooting at documented shared depths.

### Later GitLab HA successor

- Led initial self-managed HA architecture and approximately 3,000-user sizing direction.
- Established early Terraform structure and planning involving capacity, recovery, vendor coordination, timeline, rough-order estimates, and operational ownership.
- Transitioned implementation leadership to another engineer and remained periodically involved.
- The later HA implementation, development/test and production deployment, validation, DR/failover testing, and separate authorization occurred after Matthew left the team under the successor owner.

### Wider engineering platform work

- Implemented and enabled Cloud9 adoption within SE-Tools as an alternative to provisioning jump boxes for development environments; created installation guidance used by team members and projects.
- Contributed directly to a HashiCorp Packer proof of concept without claiming a complete production image factory.
- Led initial Jira-to-EKS research and architectural advice; other engineers later owned implementation and operations.
- Advised against a later GitLab EKS runner sandbox at that stage because ownership, tenancy, chargeback, and cost-attribution mechanisms were unresolved. Another engineer implemented it after Matthew left.
- Produced platform documentation, architecture maps, onboarding material, and installation guidance.

## Technical environment

GitLab, AWS, Terraform, EC2, autoscaling, load balancing, relational data/storage components, S3/EFS, Okta, PIV, GitLab runners, Cloud9, HashiCorp Packer proof of concept, Jira/EKS research, Kubernetes/EKS advisory work, Docker/container concepts, AWS WorkSpaces, and multi-account cloud patterns.

## Evidence boundaries

- Do not conflate the production singleton authorization with the later HA authorization.
- Matthew led initial HA architecture and remained periodically involved but did not implement, deploy, validate, DR-test, operate, or secure the later HA environment's separate ATO.
- Matthew did not implement or operate Jira on EKS or the later GitLab EKS runner infrastructure.
- Use of the later runner sandbox by production systems did not resolve its ownership, tenancy, chargeback, or cost-attribution gaps.
- Cloud9 adoption was within SE-Tools, not department-wide, and no quantified savings are claimed.
- Packer remained a proof of concept.
- Rebuild and onboarding improvements are observational ranges, not instrumented or audited metrics.
