![N-able](https://img.shields.io/badge/Platform-N--able-orange)
![Status](https://img.shields.io/badge/Status-In--Progress-success)
![Focus](https://img.shields.io/badge/Focus-MSP%20Operations-lightgrey)
# N-able MSP Diátaxis Knowledge Base

## Documentation Approach

This repository outlines real-world MSP tooling from the N-able ecosystem and demonstrates structured technical documentation using **Diataxis framework**, which structures content for clarity into four types:

- **Tutorials:** end-to-end learning workflows  
- **How-Tos:** task-focused procedural guides  
- **Explanations:** conceptual understanding  
- **Reference:** facts and definitions

If you’re new to this approach and want the reasoning behind this structure, see the canonical guide:  
👉 [Diátaxis Framework](https://github.com/algon85/diataxis-framework/blob/main/diataxis.md)


## Purpose
- Showcase operational familiarity with N-able products
- Demonstrate clear technical writing and system thinking
- Provide realistic MSP-focused workflows and explanations

## Structure
- **Tutorials** — learning-oriented, step-by-step guides
- **How-To Guides** — task-focused operational instructions
- **Explanations** — conceptual and architectural context
- **Reference** — factual lookup material

## Full Scaffold
````text
n-able-msp-diataxis/
├─ README.md
├─ tutorials/
│  ├─ n-central/
│  │  ├─ README.md
│  │  ├─ onboarding-a-new-client.md
│  │  ├─ deploying-agents-at-scale.md
│  │  └─ monitoring-and-alerting-basics.md
│  ├─ n-sight/
│  │  └─ README.md
│  ├─ cove-data-protection/
│  │  └─ README.md
│  └─ passportal/
│     └─ README.md
├─ how-to/
│  ├─ n-central/
│  │  ├─ silence-alerts-during-maintenance.md
│  │  ├─ troubleshoot-offline-agents.md
│  │  └─ run-remote-commands.md
│  ├─ take-control/
│  │  └─ safely-access-user-endpoints.md
│  └─ mail-assure/
│     └─ manage-spam-and-quarantine.md
├─ explanations/
│  ├─ diataxis.md
│  ├─ n-central-vs-n-sight.md
│  ├─ rmm-vs-edr-vs-mdr.md
│  └─ where-cove-fits-in-an-msp-stack.md
└─ reference/
   ├─ n-central-terminology.md
   ├─ agent-status-codes.md
   └─ alert-severity-levels.md
````
## Why There Are Separate Tutorials

This repository contains tutorials for both **N-central** and **N-sight** RMM platforms.  
While both products share core concepts like client onboarding and agent deployment, they are designed for different MSP audiences and operational scopes:

- **N-central** — large or enterprise-level MSPs, highly customizable, supports on-premises hosting  
- **N-sight** — small to mid-sized MSPs, cloud-only, simplified setup  

For a deeper conceptual comparison of these platforms, see [Explanations: N-central vs N-sight](./explanations/n-central-vs-n-sight.md).

This content is based on public product knowledge and practical MSP experience.
No proprietary or internal documentation is included.
