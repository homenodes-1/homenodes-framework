# Literature Review: Compute Governance and Residential Nodes

**Version:** v0.1 (preliminary)
**Last updated:** 2026-09-25
**Status:** Initial review. Sources to be expanded as the framework develops.

## Purpose

This review summarizes the compute governance proposals HomeNodes builds on, the assumptions they make about where compute is located, and what those assumptions mean for residential nodes.

## 1. Compute as a governance lever

Compute is detectable, excludable, and quantifiable, which makes it a practical point of control for AI oversight. This body of work establishes why compute governance matters and what it can achieve.

- Sastry, G., Heim, L., Belfield, H., Anderljung, M., Brundage, M., et al. (2024). *Computing Power and the Governance of Artificial Intelligence.* arXiv:2402.08797.
- Anderljung, M., Barnhart, J., Korinek, A., et al. (2023). *Frontier AI Regulation: Managing Emerging Risks to Public Safety.* arXiv:2307.03718.
- Hendrycks, D., Mazeika, M., & Woodside, T. (2023). *An Overview of Catastrophic AI Risks.* Center for AI Safety. arXiv:2306.12001.
- Heim, L., & Koessler, L. (2024). *Training Compute Thresholds: Features and Functions in AI Regulation.* arXiv:2405.10799.

**Assumption:** Compute is concentrated enough to be identified and measured.
**Relevance:** Residential nodes are individually small, geographically dispersed, and operated by people outside any regulated sector. Their aggregate capacity is what matters, and it is not currently measured.

## 2. Compute providers as intermediaries

Cloud providers are proposed as enforcement points, using know-your-customer checks and usage reporting to identify who is training or running high-risk models.

- Heim, L., Fist, T., Egan, J., et al. (2024). *Governing Through the Cloud: The Intermediary Role of Compute Providers in AI Regulation.* arXiv:2403.08501.
- Egan, J., & Heim, L. (2023). *Oversight for Frontier AI through a Know-Your-Customer Scheme for Compute Providers.* arXiv:2310.13625.

**Assumption:** Compute providers are identifiable firms that can carry compliance obligations.
**Relevance:** On distributed marketplaces, the platform is the intermediary, but the hardware belongs to thousands of individual hosts. It is unclear whether obligations fall on the platform, the host, or neither.

## 3. Hardware-enabled mechanisms

Proposals to build verification and governance features into AI chips themselves, including usage reporting, location verification, and licensing.

- Shavit, Y. (2023). *What Does It Take to Catch a Chinchilla? Verifying Rules on Large-Scale Neural Network Training via Compute Monitoring.* arXiv:2303.11341.
- Aarne, O., Fist, T., & Withers, C. (2024). *Secure, Governable Chips.* Center for a New American Security.
- Kulp, G., Gonzales, D., Smith, E., Heim, L., et al. (2024). *Hardware-Enabled Governance Mechanisms.* RAND Corporation.

**Assumption:** Mechanisms target data centre accelerators and large clusters.
**Relevance:** Consumer GPUs used by residential hosts are generally outside the scope of these proposals.

## 4. Data centre infrastructure

Work characterizing the data centre industry as the physical home of AI compute.

- Pilz, K., & Heim, L. (2023). *Compute at Scale: A Broad Investigation into the Data Center Industry.* arXiv:2311.02651.

**Assumption:** Large-scale compute lives in facilities with known operators, locations, and power contracts.
**Relevance:** Residential nodes have none of these characteristics, which is the core of the blind spot.

## 5. Decentralized training

Technical work showing that models can be trained across poorly connected, geographically distributed machines. This weakens the assumption that meaningful training requires a single facility.

- Douillard, A., Feng, Q., Rusu, A. A., et al. (2023). *DiLoCo: Distributed Low-Communication Training of Language Models.* arXiv:2311.08105.
- Jaghouar, S., Ong, J. M., Basra, M., et al. (2024). *INTELLECT-1 Technical Report.* Prime Intellect. arXiv:2412.01152.

**Relevance:** If training can be distributed across many small nodes, residential compute becomes relevant to training oversight, not only inference.

## 6. Standards and frameworks

- National Institute of Standards and Technology. (2023). *Artificial Intelligence Risk Management Framework (AI RMF 1.0).* NIST AI 100-1.
- National Institute of Standards and Technology. (2024). *The NIST Cybersecurity Framework (CSF) 2.0.* NIST CSWP 29.
- Souppaya, M., Morello, J., & Scarfone, K. (2017). *Application Container Security Guide.* NIST SP 800-190.
- IEEE. (2018). *IEEE 1547-2018: Standard for Interconnection and Interoperability of Distributed Energy Resources with Associated Electric Power Systems Interfaces.*

**Relevance:** These provide control and risk vocabulary, but assume organizational operators. IEEE 1547 is a useful precedent for governing privately owned equipment that interacts with shared infrastructure.

## Gaps in the literature

1. No work examines residential hosts on distributed compute marketplaces as a governance category.
2. Compute governance proposals do not address consumer GPUs in aggregate.
3. No empirical data exists on the energy, security, or privacy profile of an operating residential node.
4. The role of platforms as private regulators of residential compute has not been studied.

HomeNodes addresses gaps 1, 3, and 4 directly, and informs gap 2.
