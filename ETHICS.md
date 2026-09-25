# Ethics Statement

**Last updated:** 2026-09-25
**Contact:** research@homenodes.ca

## Principles

HomeNodes studies residential compute in a real home, running real workloads for third parties. That creates obligations to the household, to renters whose workloads run on the node, to future research participants, and to the public reading the results. This statement sets out how those obligations are met.

1. Collect only what the research needs.
2. Never inspect renter workloads.
3. Protect the household from exposure through published data.
4. Be transparent about methods, funding, and limitations.
5. Handle incidents openly and report them where required.

## Data collected

| Data | Purpose | Collected |
|---|---|---|
| Power draw of the node circuit | Energy analysis | Yes |
| System metrics (GPU and CPU use, temperature, uptime) | Operations and energy correlation | Yes |
| Network traffic volume and connection metadata at the firewall | Security domain analysis | Yes |
| Rental records from the platform (start, end, GPU hours) | Utilization analysis | Yes |
| Renter workload contents, files, or network payloads | Not needed | **No** |
| Renter identity or personal information | Not needed | **No** |
| Whole-home energy use | Would reveal household patterns | **No** |
| Other household network activity | Not in scope | **No** |

## Renter workloads

Renter workloads run in isolated containers managed by the platform. HomeNodes does not access, inspect, copy, or retain workload contents. Storage used by a rental is cleared according to platform procedures when the rental ends. Network monitoring records volume and metadata only, not content.

## Household

All adult members of the household are informed about the project and agree to the node operating in the home. The node sits on an isolated network segment and cannot reach other household devices. Published materials exclude the street address, identifying photos of the home, and network details that could be used to locate or target it.

## Publication

- Energy and operations data are published in aggregated or time-shifted form where needed to avoid revealing daily routines.
- Configuration files and diagrams are sanitized. IP addresses, credentials, and device identifiers are removed.
- Limitations, failures, and negative findings are published alongside positive ones.

## Phase 2 participants

Before any additional households take part:

- Independent ethics review will be sought for the research protocol.
- Participants will give written informed consent and may withdraw at any time, with their data removed on request.
- Participant data will be de-identified before publication. No participant addresses will be published.
- Participants will own their hardware and receive any host earnings directly.

## Security incidents

If a security incident is suspected on the node:

1. **Contain.** Suspend the platform listing and disconnect the
