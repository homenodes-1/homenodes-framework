# Gap Analysis: Residential AI Compute Nodes

**Version:** v0.1 (preliminary)
**Last updated:** 2026-09-25
**Status:** Initial desk review. Findings to be validated against proof of concept evidence and expert input.

## Purpose

This analysis identifies what existing frameworks, laws, and proposals cover for residential AI compute nodes, and where they fall short. It informs the five domains of the HomeNodes Governance Framework.

## Method

Each source was reviewed against the framework's five domains. Coverage is rated as:

- **Applies:** directly addresses the issue for residential operators
- **Partial:** addresses the issue in general terms, or for a different type of operator
- **None:** does not address the issue

## Summary

| Source | Security | Privacy | Zoning | Liability | Compliance |
|---|---|---|---|---|---|
| NIST Cybersecurity Framework 2.0 | Partial | Partial | None | None | None |
| NIST SP 800-190 (container security) | Partial | None | None | None | None |
| NIST AI Risk Management Framework | None | Partial | None | None | Partial |
| IEEE 1547 (distributed energy interconnection) | None | None | Partial | Partial | Partial |
| PIPEDA and Alberta PIPA | None | Partial | None | None | Partial |
| Bill C-36 (proposed, 2026) | None | Partial | None | None | Partial |
| Municipal home-based business bylaws | None | None | Partial | None | Partial |
| Platform host agreements (e.g. Vast.ai) | Partial | Partial | None | Partial | None |
| Compute governance proposals (compute KYC, chip export controls, hardware-enabled mechanisms) | None | None | None | None | Partial |
| EU AI Act | None | None | None | None | Partial |

No source rated **Applies** in any domain.

## Findings by domain

### Security
NIST CSF 2.0 and SP 800-190 provide sound controls, but assume an organization with staff, policies, and a defined security function. A household operator has none of these. Platform host agreements require data isolation but leave implementation to the operator. No source defines a minimum security baseline for a single-operator residential node or addresses isolation from other household devices.

### Privacy
PIPEDA and Alberta PIPA apply to organizations collecting personal information in the course of commercial activity. It is unclear whether an individual hosting workloads becomes an "organization" under these laws, or whether the operator has any obligations for personal information inside a renter's workload that the operator cannot see. Bill C-36 does not address this scenario. No source considers privacy exposure of the household itself, such as occupancy patterns revealed through power and network data.

### Zoning and land use
Home-based business bylaws were written for offices, crafts, and services. They do not contemplate sustained high electrical loads, heat, or noise from compute equipment. IEEE 1547 offers a useful parallel: residential solar and batteries went through the same question of how private equipment interacts with the grid, and interconnection standards resulted. No equivalent exists for residential compute loads.

### Liability
Platform host agreements place most obligations on the operator, including uptime and data protection, while the operator has little visibility into workloads. Home insurance policies and residential ISP terms were not written for third-party compute hosting. No source allocates liability when a renter misuses a residential node.

### Regulatory compliance
Compute governance proposals, including know-your-customer requirements for compute providers, chip export controls, and hardware-enabled monitoring, target cloud providers, data centres, and chip manufacturers. The EU AI Act regulates models and their providers, not the infrastructure they run on. Canada has no comprehensive AI law in force. None of these reach an individual operator hosting workloads for renters who may be located in other countries.

## Cross-cutting gaps

1. **No operator category.** Existing frameworks recognize individuals, organizations, and facilities. A household running commercial compute fits none of them cleanly.
2. **Responsibility without visibility.** Operators carry obligations for workloads they cannot inspect.
3. **Platform as de facto regulator.** In the absence of law, platform host agreements are the only governance instrument that applies, and they are written to protect the platform.
4. **No scale threshold.** Nothing defines when residential compute becomes a commercial or regulated activity.

## Next steps

- Review Medicine Hat land-use bylaw provisions directly
- Review home insurance and residential ISP terms
- Validate privacy findings with a privacy professional
- Update ratings with proof of concept evidence
