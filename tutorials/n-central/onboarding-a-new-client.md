# Onboarding a New Client Endpoint in N-central

**Status:** Draft  
**Diátaxis Type:** Tutorial  
**Product:** N-central RMM  
**Audience:** NOC Professionals / Helpdesk Engineers  

---

## Purpose

This tutorial walks through the **standard process for onboarding a new client endpoint** into an **existing N-central environment**.  

It is intended for team members who are new to the organization and need a repeatable, end-to-end procedure to add a device to the monitoring and management system.

---

## Assumptions

This tutorial assumes:

- N-central is already deployed and operational
- The client/customer already exists in N-central
- Monitoring policies and automation policies (AMPs) are pre-defined
- You have appropriate permissions to install agents and run automation
- The endpoint is online/reachable and meets minimum system requirements

This tutorial does **not** cover initial platform setup or policy design.

---

## Overview of the Workflow

At a high level, onboarding a new endpoint consists of:

1. Verifying client and site context
2. Installing the N-central agent
3. Confirming agent check-in
4. Applying naming standards
5. Running onboarding automation
6. Verifying monitoring and alerting

Each step builds on the previous one and should be completed in sequence.

---

## Step 1: Confirm Client and Site Context

Before installing the agent, verify that you are working in the correct **client** and **site** within N-central.

- Confirm the device belongs to the correct customer
- Confirm the appropriate site (location, department, or logical grouping)
- If multiple sites exist, ensure policies are aligned with the intended site

This prevents misapplied monitoring and reporting issues later.

---

## Step 2: Install the N-central Agent

Install the N-central agent on the endpoint using the team-approved deployment method. The method depends on whether you are **onsite** or **remote**.

### Onsite Deployment
If the device is physically in front of you:

1. Copy the agent installer to the endpoint:
   - Via USB drive **or**
   - By placing the installer on a shared network location (e.g., `\\filesrv`) and accessing it from the endpoint.
2. Run the installer on the endpoint.
3. Allow the agent to complete installation and check in with N-central.
4. Confirm the agent appears online in N-central.

### Remote Deployment
If the device is **not physically present**, but the client can access it:

1. Guide the client to [startcontrol.com](https://startcontrol.com) to initiate a TakeControl session.
2. Once connected, drag and drop the agent installer onto the endpoint.
3. Run the installer and allow it to complete.
4. Reboot the device once the agent appears in N-central.
5. Exit the TakeControl session.
6. Open the endpoint connection via the normal N-central interface to confirm the agent is online.

> **Tip:** Always verify the agent check-in and ensure the device is reporting correctly before moving to the next step.

---

## Step 3: Verify Agent Check-In

Once installed, confirm that the endpoint appears in N-central:

- Agent status shows as online
- Basic system information is populating
- No immediate connectivity or authentication errors are present

If the agent does not appear or remains offline, resolve this before proceeding.

---

## Step 4: Apply Device Naming Standards

Once the device appears in N-central, rename it according to the standard convention to ensure consistency and clarity.

### Team Naming Convention

- **New Hire:** `Firstname Lastname (DESKTOP-XXXXXX)`  
- **Replacement / Existing User:** `Firstname Lastname NEW (DESKTOP-XXXXXX)`

### Procedure

1. Open the device details in N-central.  
2. Navigate to **Settings → Given Name**   
3. Update the device name following the rules above.  
4. Save the changes and confirm the updated name appears correctly in N-central.

**Why this matters:**

- Makes devices easy to identify in alerts and reports  
- Supports automation policies that target endpoints by name  
- Reduces confusion during troubleshooting or replacements  

> **Tip:** Always double-check that the updated name matches the intended convention before proceeding with automation or monitoring steps.

---

## Step 5: Run Initial Onboarding Automation

With the agent online and properly named, run the onboarding automation policies to baseline the endpoint.

**Team Convention (Example):**
- Run the following AMPs:
  - 

These automations typically:
- 

---

## Step 6: Verify Monitoring and Alerting

After automation completes, confirm that monitoring is active:


---

## Completion Criteria

The onboarding process is complete when:


---
## Related Content

- How-to: [Troubleshooting Offline Agents](../../how-to/n-central/troubleshoot-offline-agents.md)  
- How-to: [Running Remote Commands](../../how-to/n-central/run-remote-commands.md)  
- Explanation: [N-central Architecture](../../explanations/n-central-architecture.md)  
- Explanation: [N-central vs N-sight](../../explanations/n-central-vs-n-sight.md)  

