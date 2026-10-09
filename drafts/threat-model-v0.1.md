# Residential AI Compute: Threat Model

**Status:** Draft v0.1
**Last updated:** 2026-10-09
**Related:** [PROTOCOL.md](https://github.com/homenodes-1/homenodes-poc/blob/main/PROTOCOL.md), [RESEARCH-LIMITS.md](https://github.com/homenodes-1/homenodes-poc/blob/main/RESEARCH-LIMITS.md), [RISK_REGISTER.md](../RISK_REGISTER.md)

**Summary.** AI oversight is being designed around data centres. If a meaningful share of AI compute moves into homes, several of the tools being proposed may not see it. Nobody has measured whether they do. HomeNodes exists to measure it.

## What oversight assumes

Most compute governance proposals rely on three things:

1. **A provider to regulate.** Cloud companies can check who their customers are and report large users.
2. **Thresholds.** Rules apply above a set amount of compute. The EU AI Act, for example, presumes systemic risk for models trained with more than 10^25 floating point operations.
3. **A physical footprint.** Large clusters draw megawatts, need cooling, and sit in known buildings.

All three assume compute is concentrated.

## What is changing

Marketplaces already rent out consumer GPUs located in people's homes. Separately, researchers are working on training methods that spread one job across many loosely connected machines. Two recent papers conclude this could weaken compute governance. Kryś, Sharma, and Egan (2025) identify risks to detectability and shutdownability, and the risk of structuring compute to stay under thresholds. Rahman (2026) concludes that rules must be designed to detect distributed training.

## How residential compute could matter

**1. Use without a provider relationship.** One consumer GPU is enough to run or fine-tune many open-weight models. On a marketplace, the customer deals with a platform and a homeowner, not a regulated cloud company. If the platform's checks are thin and the host can see little, nobody is positioned to notice misuse. The same applies if the customer is an AI agent acting on its own.

**2. Structuring.** Work split across many small nodes may never look like a cluster to any rule written around cluster size.

**3. Detection.** A node sits behind an ordinary household meter, mixed in with a furnace, a dryer, and an electric vehicle. Whether its workload can be picked out of that signal is unknown.

**4. Shutdown.** There is no operator to call. Capacity is spread across thousands of households and many jurisdictions, and hosts have limited control over a rental once it starts.

## What this project is not claiming

- One consumer GPU adds nothing to frontier capability.
- Frontier training on home hardware is not practical today. Home upload speeds and the lack of fast interconnect are real limits, and they may hold.
- Nobody knows how large residential hosting will become. The concern is the trend, and it is worth measuring before policy depends on tools that may not reach it.
- Distributed compute has benefits, including less concentration of control. This project does not argue for or against it.

## What the research will show

Phase 1 runs one node at a home in Medicine Hat, Alberta, under a [pre-registered protocol](https://github.com/homenodes-1/homenodes-poc/blob/main/PROTOCOL.md).

- **If a host can see what runs on their hardware,** hosts are a possible point of oversight. If not, responsibility has to sit with platforms.
- **If power data can identify AI workloads at utility-meter resolution,** energy-based oversight can reach homes, at a privacy cost that needs its own rules. If it only works at 1-second resolution, it cannot reach them with today's meters.

Either result is useful. One node is a small sample, and Phase 2 extends the study to no more than ten homes.

Findings that could help someone avoid oversight will go to compute governance researchers before publication. See the [research limits](https://github.com/homenodes-1/homenodes-poc/blob/main/RESEARCH-LIMITS.md).

## Sources

- Kryś, Sharma, Egan. [Distributed and Decentralised Training: Technical Governance Challenges in a Shifting AI Landscape](https://arxiv.org/abs/2507.07765). 2025.
- Rahman. [Does Distributed Training Undermine Compute Governance?](https://arxiv.org/abs/2605.29359) 2026.

Contact: research@homenodes.ca
