# Phase 2 Budget: Planning Estimate

**Status:** Planning estimate. Not a final budget. Revised once Phase 1 data shows actual costs, and before any household is recruited.
**Last updated:** 2026-10-09
**Currency:** CAD. USD shown at roughly 1 CAD = 0.73 USD.
**Related:** [PHASE-2.md](PHASE-2.md), [Phase 1 budget](https://github.com/homenodes-1/homenodes-poc/blob/main/BUDGET.md), [BOM](https://github.com/homenodes-1/homenodes-poc/blob/main/hardware/BOM.md)

## At a glance

| | Five homes | Ten homes |
|---|---|---|
| Per-home costs | $34,404.20 | $68,808.40 |
| Fixed costs | $4,100.00 | $4,100.00 |
| Subtotal | $38,504.20 | $72,908.40 |
| Contingency (10%) | $3,850.42 | $7,290.84 |
| **Total (CAD)** | **$42,354.62** | **$80,199.24** |
| Total (USD, approximate) | $30,900 | $58,500 |

The Phase 1 reference node is already paid for under the Phase 1 budget and is not counted here.

## Per-home costs

| Item | Per home | Basis |
|---|---|---|
| Node hardware, on loan | $5,523.00 | Phase 1 BOM estimate, including GST. Same build in every home |
| Dedicated internet line, three months | $1,007.84 | Phase 1 pricing, including GST. Breakdown below |
| Electricity reimbursement | $150.00 | Phase 1 planning figure: up to about 1,000 kWh at CAD $0.15 per kWh |
| Payment to household | $200.00 | Placeholder. Set by the ethics review |
| **Per home** | **$6,880.84** | |

**Internet line breakdown.** One line per home, on terms that permit hosting, from install to close-out.

| Item | Amount |
|---|---|
| Static public IPv4 address (one-time) | $600.00 |
| Service, static IP, and modem rental ($119.95 x 3 months) | $359.85 |
| Subtotal | $959.85 |
| GST (5%) | $47.99 |
| **Total** | **$1,007.84** |

## Fixed costs

| Item | Amount | Basis |
|---|---|---|
| Independent ethics review of the Phase 2 protocol | $4,100.00 | Estimate. No quote yet |

## Not yet costed

| Item | Note |
|---|---|
| Insurance for loaned equipment and liability in participants' homes | To be quoted |
| Legal review of the loan agreement and consent form | To be quoted |
| Electrician check where a home's circuit is in doubt | Per home, only where needed |
| Research time | Provided by the project lead, unpaid |

## Assumptions

1. **Hardware prices hold.** The per-home figure is the Phase 1 estimate. GPU and memory prices in Canada are volatile. Phase 1 actual costs replace this figure once known.
2. **The same internet pricing is available at each address.** This depends on service availability. Homes outside the provider's coverage need a separate quote.
3. **Each home needs its own static address.** If the chosen platform does not need one, the line cost falls by about $660 per home including GST.
4. **Three months of service.** Install, two weeks of baseline, eight weeks of operation, and close-out.
5. **Hardware is returned.** The loaned nodes keep resale or reuse value at the end of the study. That value is not deducted here. See open decision 4 in [PHASE-2.md](PHASE-2.md).

## What changes the total most

| Change | Effect per home |
|---|---|
| Run the project's own test workloads only, with no public listing and no dedicated line | About $1,008 less |
| Use a lower-cost GPU | Depends on the build. Reduces comparability with Phase 1 |
| Each additional home | $6,880.84 plus 10% contingency |
