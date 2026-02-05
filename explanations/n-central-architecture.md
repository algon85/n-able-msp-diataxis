# N-central Architecture

**Status:** Draft  
**Diátaxis Type:** Explanation  
**Product/Scope:** N-central RMM deployment and design

---

## Purpose
Provide a conceptual overview of the **architecture of N-central RMM**, including how it is structured, hosted, and managed. This helps readers understand how components interact and how the platform scales for MSP environments.

---

## Scope
Covers:
- Core components of N-central (server, database, web console, agents).
- Deployment options: cloud vs on-premises.
- Typical network topology considerations.
- Scalability and multi-tenant support.

---

## System Components
N-central is composed of a centralized management platform and distributed components deployed throughout customer environments.

### The N-central Server
The N-central server acts as the control plane for the platform. It coordinates communication with managed devices, evaluates monitoring checks, executes automation tasks, and stores configuration and historical data.

Key responsibilities include:
- Receiving status and performance data from agents and probes
- Evaluating thresholds and generating alerts
- Orchestrating scheduled tasks and automation policies
- Serving the Web Console used by NOC professionals

In cloud-hosted deployments, this server is operated and maintained by N-able. In on-premises deployments, it is installed and managed by the MSP.

### Data Storage & Integrity
N-central relies on a backend database to persist configuration, inventory, and monitoring data.

- **Database**: Stores device metadata, monitoring results, alert history, configuration settings, and automation state. The database is tightly coupled to the N-central server and is not accessed directly by agents or end-user systems.
- **Integrity**: Data integrity is enforced through controlled server-side access, role-based permissions, and transactional updates. Backup, retention, and disaster recovery strategies depend on the chosen deployment model (cloud-hosted or on-premises).

### Communication Tiers
1. **Agents**  
   Lightweight services installed on managed devices. Agents collect system metrics, execute tasks locally, and report results to the N-central server over secure channels.

2. **Probes**  
   Specialized services deployed within customer networks to discover and monitor devices that cannot run an agent (such as printers, switches, and network appliances). Probes act as intermediaries, aggregating data and forwarding it to the N-central server.

3. **Web Console**  
   A browser-based interface hosted by the N-central server. NOC professionals use the Web Console to configure monitoring, respond to alerts, manage customers and sites, and view reporting data.

---

## Deployment Models
N-central offers flexibility in how the management platform is hosted, allowing MSPs to align deployment with operational and compliance requirements.

| Model | Description | Use Case |
|------|-------------|----------|
| **Cloud-Hosted** | The N-central server and database are hosted and maintained by N-able. MSPs access the platform via the web without managing underlying infrastructure. | MSPs seeking reduced operational overhead, faster onboarding, and simplified maintenance. |
| **On-Premises** | The N-central server and database are installed within the MSP’s own infrastructure or private cloud. The MSP is responsible for maintenance, updates, and backups. | MSPs with strict data residency, compliance, or customization requirements. | 

---

## Multi-Tenancy and Scalability

---

## Links
- [N-central Terminology]
- [Onboarding a New Client]
