# Changelog

All notable changes to the HomeNodes Governance Framework are recorded here.

Versions follow v0.x numbering during drafting. Dates use YYYY-MM-DD.

## [Unreleased]

### Planned


## 2026-10-09

### Added
- Phase 2 plan (PHASE-2.md): purpose, questions, design, schedule, limits, cost, open decisions
- Phase 2 planning estimate (PHASE-2-BUDGET.md): five-home and ten-home scenarios with assumptions
- Phase 2 overview diagram (diagrams/phase-2-overview.svg and .png)
- Threat model draft (drafts/threat-model-v0.1.md): what compute oversight assumes, four ways residential compute could weaken it, what the project is not claiming, and what Phase 1 will show

### Changed
- ROADMAP: Phase 1 renamed "Single-node study". Phase 2 renamed "Multi-home study" and rewritten as a fixed research sample with milestones. Links added to the phase documents
- ETHICS: Phase 2 participants section revised. Hardware is project-owned and loaned, the project operates the nodes, households are reimbursed for electricity. Previously participants were to own the hardware and receive host earnings
- Risk register R15: updated to match
- README: phases summarized with links
- README: purpose section links to the threat model

## 2026-10-07

### Changed
- README: purpose rewritten around studying the risks of residential AI compute. The five domains are now described as how findings are organized
- ROADMAP and risk register R2: Phase 1 length corrected from 12 to 16 weeks to match the Phase 1 budget

## 2026-09-28

### Added
- Distribution models draft (drafts/distribution-models.md)
- Risk register: R16 (acceleration risk) and R17 (findings that could help avoid oversight)
- Ethics statement: acceleration risk section linking to RESEARCH-LIMITS.md in homenodes-poc
- README: link to the Phase 1 budget in homenodes-poc
- Risk register: R7 confirmed (incumbent residential terms prohibit hosting) and mitigated with a separate line from a provider that permits it. R18 added (dependence on a single compute platform)
- Risk register: R8 closed. The dedicated line has a static public IPv4 address with no blocked inbound ports

### Fixed
- Ethics statement: completed the security incident procedure, which was cut off
- Risk register: completed R15, which was cut off

## [v0.1] - 2026-09-25

### Added
- Repository created
- README with project purpose, scope, and status
- CC BY 4.0 license
- Gap analysis against NIST, IEEE, and Canadian privacy law
- Framework outline with five domain headings (drafts/HomeNodes-Framework-v0.1.md)
- Literature review of existing compute governance proposals
- Project roadmap (ROADMAP.md)
- Risk register (RISK_REGISTER.md)
- Ethics statement (ETHICS.md)
- Governance framework map (diagrams/)
