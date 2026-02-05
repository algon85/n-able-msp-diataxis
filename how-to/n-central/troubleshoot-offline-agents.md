# Troubleshoot Offline Agents (N-central)

**Status:** Final  
**Diátaxis Type:** How-To  
**Product:** N-central RMM

## Purpose
Provide step-by-step guidance to troubleshoot agents that go offline.

## Scope
- Assumes basic familiarity with N-central agent monitoring.
- Focuses on Windows-based endpoints managed via the N-central Windows Agent.

## Steps

1. **Verify Local Service Status** Log in to the target endpoint and open the Services console (`services.msc`). Ensure the **Windows Agent Service** and **Windows Agent Maintenance Service** are both in a "Running" state.

2. **Test Server Connectivity** Confirm the endpoint can reach the N-central server over the network. Open a command prompt and run:  
   `Test-NetConnection <https://ncodXXX.n-able.com/> -Port 443`

3. **Examine Agent Logs** Navigate to the installation directory (default: `C:\Program Files (x86)\N-able Technologies\Windows Agent\log\`) and open `AdvancedUser.log`. Look for "Communication Error" or "403 Forbidden" entries that indicate authentication or certificate issues.

4. **Verify Appliance and Customer Association** In the N-central Web Console, verify that the device is still associated with the correct **Customer** or **Site**. If a device was moved without an agent check-in, it may report as offline.

5. **Force Agent Check-in or Reinstall** Restart the Windows Agent Service. If the device does not check back into the **NOC** dashboard within 10 minutes, download a new agent installer from the N-central UI and perform a "Repair" installation.

## Links
- [N-central Architecture](../../explanations/n-central-architecture.md)
- [N-central Terminology](../../reference/n-central-terminology.md)
