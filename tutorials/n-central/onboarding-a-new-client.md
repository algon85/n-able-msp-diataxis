# Onboarding a New Client Endpoint in N-central

**Status:** Draft  
**Diátaxis Type:** Tutorial  
**Product:** N-central RMM  
**Audience:** NOC Professionals / Helpdesk Engineers  

---

## Purpose

This tutorial walks through the **standard process for onboarding a new client endpoint** into an **existing N-central environment**.  

It is intended for team members who are new to the organization and need a repeatable, end-to-end procedure to bring a device under monitoring and management.

---

## Assumptions

This tutorial assumes:

- N-central is already deployed and operational
- The client/customer already exists in N-central


---

## Overview of the Workflow

At a high level, onboarding a new endpoint consists of:

1. Verifying client and site context
2. 

Each step builds on the previous one and should be completed in sequence.

---

## Step 1: Confirm Client and Site Context

Before installing the agent, verify that you are working in the correct **client** and **site** within N-central.


---

## Step 2: Install the N-central Agent

Install the N-central agent on the endpoint using the approved deployment method for your environment.



After installation, allow time for the agent to check in.

---

## Step 3: Verify Agent Check-In

Once installed, confirm that the endpoint appears in N-central:



If the agent does not appear or remains offline, resolve this before proceeding.

---

## Step 4: Apply Device Naming Standards

After the device appears in N-central, apply the team’s standard naming convention.

**Team Convention (Example):**
- Format: 
- Example: 

Update the device name according to team standards before continuing.

---

## Step 5: Run Initial Onboarding Automation

With the agent online and properly named, run the onboarding automation policies to baseline the endpoint.

**Team Convention (Example):**
- Run the following AMPs:


---

## Step 6: Verify Monitoring and Alerting

After automation completes, confirm that monitoring is active:


---

## Completion Criteria

The onboarding process is complete when:


## Related Content

- How-to: [Troubleshooting Offline Agents](../../how-to/n-central/troubleshoot-offline-agents.md)  
- How-to: [Running Remote Commands](../../how-to/n-central/run-remote-commands.md)  
- Explanation: [N-central Architecture](../../explanations/n-central-architecture.md)  
- Explanation: [N-central vs N-sight](../../explanations/n-central-vs-n-sight.md)  

