# Distribution Models as Research Variables

**Status:** Draft. Working document for Phase 2 research design. Not a commercial plan or a commitment to any partner.
**Track:** Sovereignty track (primary). Relevant to the AI safety track where noted.
**Last updated:** 2026-09-28

## Purpose

The proof of concept tests one node in one home. Before Phase 2 (5 to 10 homes), we need to decide how nodes get into homes. That choice is not only logistics. Each distribution model assigns ownership, control, liability, and privacy obligations to different parties.

This draft treats the distribution model as a research variable and maps each option against the five governance domains in the framework.

## Research question

How does the choice of distribution model change who holds security, privacy, land-use, liability, and regulatory obligations for residential AI compute, and which model keeps operational control of that compute under Canadian, publicly accountable governance?

Sub-questions:

1. Who owns the hardware, who operates it, and who can change what it runs?
2. Who holds the personal information a node generates (energy use, network metadata, occupancy signals)?
3. What happens to obligations when the home is sold or rented, or the homeowner opts out?
4. Which existing rules already apply, and where are the gaps?

## The three models

### A. Builder-ready

Homebuilders make new homes node-ready rather than installing hardware: a dedicated circuit, a ventilated niche in the mechanical room, a network drop, and conduit. The node is added later, only if the homeowner opts in.

Why this version: a house lasts 50 years or more and GPU hardware is obsolete in 3 to 5. Pre-installing hardware creates an obsolescence problem and a consent problem for later buyers who never agreed to host it. Node-ready infrastructure avoids both.

| | |
|---|---|
| Infrastructure owner | Homeowner (part of the house) |
| Node owner | Homeowner or project, depending on the opt-in agreement |
| Operator | Project, or homeowner under project standards |
| Compensation | Not defined by the builder. Needs a separate mechanism (Model C or direct payment) |

What this model tests: whether building code and land-use rules can prepare housing stock for residential compute without committing any occupant to host it.

### B. ISP-managed

An ISP installs, manages, and supports the node as a second device next to its gateway, and discounts the homeowner's monthly bill in return.

The ISP brings install crews, billing relationships, remote device management, and permission to run server traffic, which residential terms of service usually prohibit. ISP gateways are low-power commodity hardware, so the node is a separate box either way.

| | |
|---|---|
| Node owner | ISP |
| Operator | ISP |
| Compensation | Service discount |
| Personal information | Held by the ISP under federal private-sector privacy law |

What this model tests: whether an existing regulated telecom relationship can absorb residential compute, and what happens to control when a national carrier operates the fleet. The compute stays in Canadian homes, but governance moves to the carrier. The ISP's revenue case is an open question.

### C. Utility-partnered

The City of Medicine Hat, which owns and operates its electric utility, meters node power draw separately and credits the homeowner's utility bill.

The city already has the meter, the billing relationship, and the energy data. Compensation matches the actual cost the homeowner carries, which is electricity. Rough estimate: a node averaging 150 W uses about 1,300 kWh a year. In winter, waste heat offsets some home heating. In summer it adds to the cooling load.

| | |
|---|---|
| Node owner | Project or homeowner (the utility meters and credits, it does not need to own the node) |
| Operator | Project |
| Compensation | Utility bill credit |
| Personal information | Energy data held by a municipal public body |

What this model tests: whether a publicly owned utility can act as the accountable partner for residential compute, and whether a bill credit is a workable and lawful compensation mechanism.

## Mapping against the five governance domains

| Domain | A. Builder-ready | B. ISP-managed | C. Utility-partnered |
|---|---|---|---|
| **Security standards** | Node security set by the project or homeowner. Builder responsible only for physical infrastructure. Risk: inconsistent standards across homes. | ISP applies its own device management and patching. Consistent, but standards are set privately and may not be disclosed. | Project sets node standards. Utility responsible for metering integrity. Split responsibility needs a written agreement. |
| **Privacy obligations** | Builder holds little or no personal information after sale. Node data governed by the operator. Alberta PIPA likely applies to private operators. | ISP holds node data alongside subscriber data. PIPEDA applies (federally regulated telecom). Risk of data being combined. | Energy data held by the city. POPA applies to the city as a public body. Node-level metering may reveal occupancy patterns. PIA needed. |
| **Zoning and land use** | Strongest link of the three. Node-ready spaces could be addressed in the building code and land-use bylaw. Open: is hosting a node a home occupation? | Treated like other telecom equipment in the home. Home occupation question still applies. | City is both regulator (land use) and partner (utility). Needs clear separation of roles. |
| **Liability allocation** | Split across builder (infrastructure), homeowner (premises), and operator (node). A property sale transfers the premises but not necessarily the node agreement. | ISP carries most device liability. Homeowner liability limited to the premises. Clearest allocation of the three. | Node liability sits with the project. City liability limited to metering and billing. |
| **Regulatory compliance pathways** | Building code, electrical code, land-use bylaw. No telecom or energy regulator involved. | CRTC and ISP terms of service. Residential terms need to change to allow server traffic. | Municipal utility rules and rate structure. Whether a bill credit for hosted compute is permitted under current rules is to be confirmed. |

Home insurance treatment of a hosted node is unresolved in all three models.

## Cross-cutting variables

These apply to every model and will be recorded for each Phase 2 home:

- **Ownership:** of the node and of the infrastructure it sits in
- **Operational control:** who can change the workload, firmware, and network configuration
- **Consent:** how the homeowner opts in, and how a later buyer or tenant is informed
- **Exit:** what happens when the homeowner opts out, moves, or sells
- **Compensation:** form, amount, and who pays
- **Data:** what the node and meter generate, who holds it, and under which privacy law
- **Workload control:** who schedules workloads, and from where

## Sovereignty note

Control of the fleet differs by model: homeowner or project (A), national carrier (B), municipal public body (C).

The workload scheduler is a separate issue that affects all three. The POC uses the Vast.ai marketplace, which is not Canadian-controlled. Phase 2 needs a plan for Canadian-controlled scheduling, or for restricting workloads to Canadian renters, before any sovereignty claim holds. Distribution model and scheduler control should be assessed together.

## Relevance to the AI safety track

Oversight depends on knowing who operates compute and being able to reach them. Model B concentrates operation in a regulated carrier. Model C places it with a public body. Model A spreads it across individual homeowners, which is the hardest case for oversight.

## Phase 2 approach

Phase 2 keeps scope realistic: one hardware spec, one distribution model, 5 to 10 homes. The other two models will be assessed through document review and interviews with builders, an ISP, and the City.

Proposed field model: utility-partnered, pending discussion with the City of Medicine Hat.

## Assumptions and limits

- Energy figures are estimates. Actual draw will come from POC metering.
- The POC node is the RTX 5080 desktop build in `homenodes-poc/BOM.md`. The enclosure concept (DGX Spark class) is a later-phase idea and a different hardware class. The distribution models are written to be hardware-neutral.
- Legal applicability (PIPA, PIPEDA, POPA, CRTC, municipal utility rules) is a working view, not a legal opinion. Each item needs confirmation.
- No partner has been approached. Nothing here reflects a partner's position.

## Open questions

1. Does hosting a node count as a home occupation under the Medicine Hat Land Use Bylaw?
2. How do standard Alberta home insurance policies treat a hosted compute node?
3. Can the City's utility credit a bill for hosted compute under current rate rules?
4. Would an ISP need to change its residential terms of service, or offer a separate agreement?
5. How is a later buyer or tenant told that a home is node-ready or hosting a node?
6. Who is accountable if a hosted workload is misused, and can the homeowner see what runs on their node?

## Revision history

- 2026-09-28: First draft.
