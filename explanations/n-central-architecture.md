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
1. **Agents**: 
2. **Probes**: 
3. **Web Console**: 

---

## Deployment Models
N-central offers flexibility in how the management server is hosted:

| Model | Description | Use Case |
|------|-------------|----------|
| **Cloud-Hosted** |
| **On-Premises** | 

---

## Multi-Tenancy and Scalability

---

## Links
- [N-central Terminology]
- [Onboarding a New Client]
