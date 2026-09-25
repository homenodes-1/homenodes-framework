# HomeNodes Governance Framework

**Version:** v0.1 (outline)
**Status:** Working draft, structure only
**Last updated:** 2026-09-25

---

## 1. Introduction

### 1.1 Purpose

This framework sets out governance expectations for residential AI compute nodes: privately owned hardware in a home that runs AI workloads for third parties through a distributed compute platform.

### 1.2 Problem statement

Current compute governance proposals assume compute sits in identifiable, regulated facilities with known operators. Residential nodes fall outside those assumptions. No existing framework sets minimum security standards, privacy obligations, land-use classification, liability allocation, or compliance pathways for them.

### 1.3 Scope

In scope:
- Single-household nodes running third-party AI workloads through a distributed compute marketplace
- Canadian federal, Alberta provincial, and municipal context, with principles intended to apply elsewhere

Out of scope:
- Personal AI use on household hardware with no third-party workloads
- Commercial data centres and colocation facilities
- Cryptocurrency mining, except where it shares infrastructure with AI workloads

### 1.4 Definitions

| Term | Definition |
|---|---|
| Residential compute node | GPU-equipped hardware in a dwelling that runs workloads for third parties |
| Operator | The person or household that owns and runs the node |
| Platform | The marketplace that matches renters to nodes and handles payment |
| Renter | The party whose workload runs on the node |
| Household | Everyone who lives in or shares the network of the dwelling |

### 1.5 Method

Framework provisions are informed by:
- A gap analysis of existing frameworks (see `gap-analysis`)
- A literature review of compute governance proposals (see `literature-review`)
- Evidence from the HomeNodes proof of concept node

---

## 2. Domain 1: Security Standards

### 2.1 Scope
Technical and physical controls for the node and the household network it sits on.

### 2.2 Key questions
- What minimum controls should an operator have in place before accepting workloads?
- How is the node isolated from other household devices?
- Who is responsible for patching the host OS, drivers, and platform software?
- How are security incidents detected and reported, and to whom?
- What visibility does the operator have into what a workload is doing?

### 2.3 Current coverage
*To be completed from gap analysis.*

### 2.4 Gaps
*To be completed.*

### 2.5 Draft provisions
*To be completed.*

### 2.6 Proof of concept evidence
*To be completed from build and operation.*

---

## 3. Domain 2: Privacy Obligations

### 3.1 Scope
Personal information handled by the node, the operator, the platform, and the renter, and the privacy of the household and neighbours.

### 3.2 Key questions
- Does an individual operator become subject to private-sector privacy law (PIPEDA, Alberta PIPA) by hosting workloads?
- What obligations apply if a renter's workload processes personal information?
- What household data (network activity, power use, occupancy patterns) is exposed to the platform?
- Where is renter data stored, and how is it removed at the end of a rental?
- How are cross-border data flows handled when renters are outside Canada?

### 3.3 Current coverage
*To be completed from gap analysis.*

### 3.4 Gaps
*To be completed.*

### 3.5 Draft provisions
*To be completed.*

### 3.6 Proof of concept evidence
*To be completed from build and operation.*

---

## 4. Domain 3: Zoning and Land Use

### 4.1 Scope
Whether and how residential compute fits municipal land-use rules, building and electrical codes, and neighbourhood impact.

### 4.2 Key questions
- Is hosting compute for third parties a home-based business under municipal land-use bylaws?
- At what scale does a residential node become a commercial use?
- What electrical code and permitting requirements apply?
- How should noise, heat, and grid load on residential circuits and transformers be managed?
- Should municipal utilities be notified of sustained high loads?

### 4.3 Current coverage
*To be completed from gap analysis.*

### 4.4 Gaps
*To be completed.*

### 4.5 Draft provisions
*To be completed.*

### 4.6 Proof of concept evidence
*To be completed from build and operation.*

---

## 5. Domain 4: Liability Allocation

### 5.1 Scope
Who is responsible when something goes wrong: hardware failure, property damage, misuse of compute, or harm caused by a workload.

### 5.2 Key questions
- Does home insurance cover hardware used for third-party compute?
- Who is liable if a renter uses the node for illegal or harmful activity?
- What do platform terms place on the operator versus the renter?
- Do residential ISP terms of service permit hosting third-party workloads?
- How is liability handled for fire, electrical, or water damage linked to the node?

### 5.3 Current coverage
*To be completed from gap analysis.*

### 5.4 Gaps
*To be completed.*

### 5.5 Draft provisions
*To be completed.*

### 5.6 Proof of concept evidence
*To be completed from build and operation.*

---

## 6. Domain 5: Regulatory Compliance Pathways

### 6.1 Scope
How existing law applies to residential nodes, where it falls short, and what a workable compliance path looks like.

### 6.2 Key questions
- Do export controls on advanced compute apply when a node serves renters in other countries?
- How would proposed compute reporting or monitoring requirements reach residential operators?
- What tax and business registration obligations apply to host income?
- Is operator identity verification needed, and who should perform it?
- What should a proportionate, low-burden compliance path for individual operators include?

### 6.3 Current coverage
*To be completed from gap analysis.*

### 6.4 Gaps
*To be completed.*

### 6.5 Draft provisions
*To be completed.*

### 6.6 Proof of concept evidence
*To be completed from build and operation.*

---

## 7. Cross-Domain Considerations

- **Energy use.** Measured consumption informs zoning, grid impact, and compliance provisions.
- **Scale thresholds.** At what point should obligations change as node count or power draw increases?
- **Platform responsibility.** Which obligations should sit with platforms rather than individual operators?

---

## Appendices (planned)

- A. Gap analysis
- B. Literature review
- C. Proof of concept summary
- D. Energy data summary
- E. References
