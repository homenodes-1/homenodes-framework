# Risk Register

**Last updated:** 2026-09-25
**Review cycle:** Monthly during Phase 1, then at each phase transition

Likelihood and impact are rated Low, Medium, or High.

## Project delivery

| ID | Risk | Likelihood | Impact | Mitigation | Status |
|---|---|---|---|---|---|
| R1 | Hardware prices rise or stock is unavailable due to GPU and memory shortages | High | Medium | Fixed budget ceiling. Alternative GPU options identified (used RTX 4090). Buy critical components first when stock appears. | Open |
| R2 | Project lead capacity is limited by a full-time role | Medium | Medium | Phase 1 scoped to 12 weeks with part-time effort. Documentation built incrementally. Milestones reviewed monthly. | Open |
| R3 | Expert interviewees are slow to respond or unavailable | Medium | Medium | Begin outreach before hardware arrives. Draw on professional and IEEE section networks. Accept written responses as an alternative. | Open |
| R4 | Phase 2 households cannot be recruited | Medium | High | Recruit through the website intake form and local networks. Proceed with fewer homes if needed and document the limitation. | Open |

## Proof of concept operation

| ID | Risk | Likelihood | Impact | Mitigation | Status |
|---|---|---|---|---|---|
| R5 | Node is rarely rented, producing little workload data | Medium | High | Competitive pricing, VM support, and verification. If rentals are low, run documented benchmark workloads to generate load and energy data. Low demand is itself a reportable finding. | Open |
| R6 | Node does not achieve Vast.ai verification | Medium | Medium | Meet published requirements before listing. Unverified machines remain rentable. Document the verification process either way. | Open |
| R7 | Residential ISP terms prohibit hosting third-party workloads | Medium | High | Review terms before listing. Contact the ISP if unclear. Record the outcome as evidence for the liability and compliance domains. | Open |
| R8 | Connection is behind carrier-grade NAT, which the platform does not support | Low | High | Confirm public IPv4 address before purchasing hardware. | Open |
| R9 | Platform changes host terms, requirements, or supported OS | Medium | Medium | Version all documentation. Treat platform changes as evidence of platform-as-regulator dynamics. | Open |

## Security and safety

| ID | Risk | Likelihood | Impact | Mitigation | Status |
|---|---|---|---|---|---|
| R10 | A renter workload compromises the node or attempts to reach other household devices | Low | High | Dedicated firewall, isolated network segment, no inbound access to household network, logging and alerting. Incident response procedure in the ethics statement. | Open |
| R11 | A renter uses the node for illegal or harmful activity | Low | High | Rely on platform terms and enforcement. Retain logs. Suspend hosting and report through the platform if activity is suspected. | Open |
| R12 | Fire, electrical, or water damage linked to the node | Low | High | Operate within circuit capacity. UPS with surge protection. Equipment elevated off basement floor. Smoke detection nearby. Confirm insurance coverage before operation. | Open |

## Research integrity and privacy

| ID | Risk | Likelihood | Impact | Mitigation | Status |
|---|---|---|---|---|---|
| R13 | Published data or configuration reveals household location, patterns, or network details | Medium | High | Measure only the node circuit. Sanitize all configuration files and diagrams. No street address or identifying photos published. | Open |
| R14 | Energy measurements are inaccurate | Medium | Medium | Document measurement method and device accuracy. Cross-check against the utility meter over a fixed period. | Open |
| R15 | Perceived conflict of interest from host earnings | Low | Medium | Disclose earnings in project reporting. Apply
