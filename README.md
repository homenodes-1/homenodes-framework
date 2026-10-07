# HomeNodes

Research on the risks of AI compute moving into homes.

## Purpose

Consumer hardware can now rent out GPU time on distributed compute marketplaces and run AI workloads from a residential connection. Current compute oversight assumes compute sits in data centres, where cloud provider checks, hardware reporting, and energy monitoring can reach it. None of those tools were designed for compute in a house on a residential street.

HomeNodes studies what changes when AI compute is spread across many homes: what a host can see about the workloads on their hardware, whether power and network data can identify those workloads, and where existing rules stop applying. Phase 1 measures this on a single live node (see the [measurement protocol](https://github.com/homenodes-1/homenodes-poc/blob/main/PROTOCOL.md)).

This repository holds the governance side of that work: the gap analysis, the risk register, and the findings organized by domain.

## Scope

Findings are organized under five governance domains:

1. **Security standards.** Minimum technical controls for a node on a residential network.
2. **Privacy obligations.** Data handled by the node, the household, and neighbours.
3. **Zoning and land use.** Whether and how residential compute fits municipal bylaws.
4. **Liability allocation.** Who is responsible when something goes wrong.
5. **Regulatory compliance pathways.** How existing Canadian law applies and where it falls short.

## Status

**Current version:** v0.1 (outline)

Drafts are in early development and are informed by a proof of concept node in Medicine Hat, Alberta. See [homenodes-poc](../../../homenodes-poc) for build and configuration details.

## Versioning

Documents use v0.x numbering during drafting. Each revision is recorded in CHANGELOG.md.

## Related

- Phase 1 budget and milestones: [BUDGET.md](https://github.com/homenodes-1/homenodes-poc/blob/main/BUDGET.md) in homenodes-poc
- Project site: [homenodes.ca](https://homenodes.ca)
- Contact: research@homenodes.ca

## License

This work is licensed under [CC BY 4.0](LICENSE).
