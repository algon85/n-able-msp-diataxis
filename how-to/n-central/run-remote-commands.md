# Run Remote Commands in N-central

**Status:** Draft  
**Diátaxis Type:** How-to  
**Product/Scope:** N-central RMM – remote command execution

## Goal
Execute a command or script on one or more managed devices using N-central.

## When to Use This
Use this procedure when you need to:
- Run a one-time command for troubleshooting
- Collect diagnostic information
- Perform a quick remediation task
- Validate system state without interactive remote access

For recurring or automated tasks, use Automation Policies instead.

## Prerequisites
Conditions that need to be met before you begin:
- You have access to the N-central Web Console
- The target device has an active N-central agent
- Your user role has permission to run remote commands
- The device is online and is checking in

## Steps

### 1. Locate the Target Device
1. Log in to the N-central Web Console.
2. Navigate to **Customers** and select the appropriate **Customer** and **Site**.
3. Open the target **Device**.

### 2. Open the Remote Command Interface
1. From the device dashboard, locate the **Tools** menu.
2. Select the **Command Prompt** button.
3. Click **Start Session**.

### 3. Configure the Command
1. Enter the command or script to be executed.
2. Review the command carefully before execution.

> Commands run with agent-level privileges. Ensure the command is safe and appropriate for the target system.

### 4. Execute the Command
1. 
2. 

### 5. Review Results
1. 
2. 

## Validation
Confirm success by:
- 
- 

## Common Issues

- **Command does not run**  

- **Permission denied**  

- **Unexpected results**  

## Related Tasks
- Creating Automation Policies
- Running scheduled tasks
- Accessing devices via remote control

## Links
- [N-central Terminology](../reference/n-central-terminology.md)
- [N-central Architecture](../explanation/n-central-architecture.md)
