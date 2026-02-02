# N-central Architecture

**Status:** Draft  
**Diátaxis Type:** Explanation  
**Product/Scope:** N-central RMM deployment and design

## Purpose
Provide a conceptual overview of the **architecture of N-central RMM**, including how it is structured, hosted, and managed. This helps readers understand how components interact and how the platform scales for MSP environments.

## Scope
Covers:
- Core components of N-central (server, database, web console, agents)  
- Deployment options: cloud vs on-premises  
- Typical network topology considerations  
- Scalability and multi-tenant support  

## Key Concepts

- **Server Components:** N-central includes a central management server, which coordinates agent communication, stores monitoring data, and hosts the web console.  

- **Agents:** Installed on client devices, agents report system health, deploy patches, and enforce policies.  

- **Database:** Stores all monitoring, configuration, and alert data. Ensures data integrity and supports reporting.  

- **Web Console:** Provides the NOC Professionals with an interface to monitor clients, manage policies, and respond to alerts.  

- **Hosting Options:** N-central can be deployed in a cloud-hosted environment or on-premises, giving MSPs flexibility depending on their scale and security requirements.  

## Links
- [Onboarding a New Client](https://github.com/algon85/n-able-msp-diataxis/blob/main/tutorials/n-central/onboarding-a-new-client.md)
- [N-central vs N-sight](https://github.com/algon85/n-able-msp-diataxis/blob/main/explanations/n-central-vs-n-sight.md)
