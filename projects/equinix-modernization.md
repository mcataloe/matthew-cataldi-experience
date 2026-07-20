# Hybrid-Cloud Interconnection Modernization

## Context

A large federal organization was modernizing non-production connectivity among on-premises environments, AWS, Azure, GCP, and Equinix cloud-interconnection services.

## Matthew's contribution

Matthew served as Technical Product Owner and engineering lead across customer solution development, architecture direction, backlog and sprint priorities, acceptance criteria, stakeholder coordination, Terraform standards, delivery planning, and operating-model design.

He:

- Led and co-implemented AWS Direct Connect connectivity.
- Led Azure ExpressRoute and Google Cloud Interconnect designs while another engineer performed primary configuration.
- Established the broad Terraform structure, transitioned implementation during onboarding, and later completed remaining work across reusable AWS-, Azure-, GCP-, and Equinix-oriented modules.
- Coordinated cloud, networking, security, business, engineering, executive, customer, and vendor stakeholders.
- Led DNS and routing designs while implementation was shared or performed by the relevant engineering teams.
- Designed and configured stamped-account IPsec connectivity.
- Advised on enterprise MACsec while the networking organization owned planning and implementation.
- Worked within existing BGP foundations rather than claiming ownership of BGP configuration.
- Advanced the Online Passport Renewal network path through late non-production integration toward production readiness without operating live traffic.
- Created architecture, onboarding, Terraform, governance, and implementation documentation.
- Proposed a multi-tenant governance model that was not officially adopted or implemented.
- Supported a secure large-dataset-transfer capability that was only partially implemented and whose final decision remained customer-owned.

## Technical environment

Equinix Fabric, Equinix Network Edge, AWS Direct Connect, Azure ExpressRoute, Google Cloud Interconnect, AWS, Azure, GCP, BGP context, IPsec, MACsec advisory work, Terraform, GitLab, object storage, DNS, routing, and enterprise networking technologies.

## Evidence boundaries

- Customer connectivity was verified in non-production environments, not production.
- Terraform ownership was shared and sequenced; Matthew did not solely implement every module.
- Another engineer owned the GitLab pipeline definitions and performed principal configuration for several connectivity components.
- Equinix Network Edge virtual devices were pre-established through the contract vehicle; Matthew did not create or procure them.
- Matthew did not own or personally configure BGP, perform primary hands-on ExpressRoute/Cloud Interconnect configuration, operate live Online Passport Renewal traffic, or implement enterprise MACsec.
- The proposed governance model remained a proposal, and the large-data-transfer capability remained partial.
- Customer-specific topology, internal account details, colleague identities, and security-sensitive implementation detail are intentionally omitted.
