# Monitoring and Alerting Basics in N-central

**Status:** Draft  
**Diátaxis Type:** Tutorial  
**Product:** N-central RMM  
**Audience:** NOC Professionals / Helpdesk Engineers  

---

## Purpose

This tutorial introduces the **core monitoring and alerting concepts** in N-central.  
It is intended for team members who need to understand how N-central detects issues, raises alerts, and surfaces critical information.

---

## Assumptions

- You have access to an N-central environment
- Endpoints are already onboarded and reporting
- Monitoring policies are pre-defined by the team
- You understand basic NOC workflows

---

## Overview

Monitoring in N-central consists of:

1. Predefined checks on devices (CPU, disk, services, etc.)  
2. Alerting policies and thresholds  
3. Notifications via email, dashboard, or integrations  
4. Escalation procedures for critical events

---

## Step 1: Understand Check Types

- **Agent Health Checks:** Confirm endpoints are online and reporting  
- **System Performance Checks:** CPU, memory, disk usage  
- **Service/Application Checks:** Verify critical applications are running  
- **Custom Checks:** Specific to client or environment requirements

> Tip: Focus on the checks that are tied to your client’s SLA priorities.

---

## Step 2: Review Alert Severity Levels

- **Informational / Low:** For non-critical events  
- **Medium:** Potential issues that may require attention  
- **High / Critical:** Immediate action required

> Tip: Consistently use severity levels to prioritize response.

---

## Step 3: Check Alerting Policies

1. Open the **Alerts & Notifications** section in N-central  
2. Review the policy for each check type  
3. Confirm recipients and escalation rules are correct

> Tip: If in doubt, consult the team’s standard alerting configuration.

---

## Step 4: Respond to Alerts

- Acknowledge the alert in N-central  
- Investigate the root cause using endpoint tools  
- Resolve the issue or escalate per team workflow  
- Close the alert once resolved

---

## Completion Criteria

Monitoring is correctly configured and functional when:

- Critical alerts appear in the dashboard as expected  
- Notification recipients are correctly assigned  
- Team members can respond according to standard workflow  

---

## Related Content

- How-to: [Silence Alerts During Maintenance](../../how-to/n-central/silence-alerts-during-maintenance.md)  
- How-to: [Troubleshoot Offline Agents](../../how-to/n-central/troubleshoot-offline-agents.md)  
- Explanation: [N-central Architecture](../../explanations/n-central-architecture.md)
