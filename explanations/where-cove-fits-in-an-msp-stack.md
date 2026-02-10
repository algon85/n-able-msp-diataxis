# Where Cove Fits in an MSP Stack

**Status:** Draft  
**Diátaxis Type:** Explanation  
**Product/Scope:** Understanding Cove Data Protection within MSP environments

## Purpose
Provide a conceptual overview of how **Cove Data Protection** integrates into the broader MSP service stack, including backup, recovery, and disaster recovery workflows.

## Scope
Covers:
- Role of Cove in protecting endpoints and servers  
- Integration with RMM tools like N-central and N-sight  
- Data flow and policy considerations  
- Use cases for MSPs managing multiple clients
- Cove is not an RMM; it complements EDR/MDR rather than replacing them  

## Key Concepts

- **Endpoint & Server Backup:** Cove provides automated backup of client endpoints and servers to ensure rapid recovery in case of data loss.  

- **Policy Management:** Backup policies can be centrally defined and applied across clients, including retention schedules, encryption settings, and restore procedures.  

- **Integration:** Works alongside RMM platforms to trigger backups based on system events or schedules, allowing MSPs to streamline operations.  

- **Recovery & DR:** Supports point-in-time restores, full system restores, and disaster recovery scenarios for business continuity.

## Links
- [Cove Data Protection Tutorials](https://github.com/algon85/n-able-msp-diataxis/blob/main/tutorials/cove-data-protection/)
- [Deploying Agents at Scale](https://github.com/algon85/n-able-msp-diataxis/blob/main/tutorials/n-central/deploying-agents-at-scale.md)
- [Monitoring and Alerting Basics](https://github.com/algon85/n-able-msp-diataxis/blob/main/tutorials/n-central/monitoring-and-alerting-basics.md)
- [RMM vs EDR vs MDR](https://github.com/algon85/n-able-msp-diataxis/blob/main/explanations/rmm-vs-edr-vs-mdr.md)
