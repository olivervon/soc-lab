# Setup Documentation

This section documents the step-by-step setup of the lab environment.

## Step 2.1 – SOC Analyst VM

### Objective
Create a dedicated SOC analyst workstation to interact with Microsoft Sentinel and perform alert triage and investigations.

### VM Details
- Name: SOC-Analyst-VM
- OS: Windows 10 Pro
- Platform: Hyper-V
- Network: SOC-Lab-Internal

### Verification
The SOC analyst VM was successfully deployed and connected to the isolated lab network.

![SOC Analyst VM network](../screenshots/setup/01-soc-analyst-vm-network.PNG)
![SOC Analyst VM desktop](../screenshots/setup/02-soc-analyst-vm-desktop.PNG)

### Why This Matters for SOC
SOC analysts typically work from client systems while the SIEM runs in the cloud. This setup reflects a realistic SOC workflow.

## Step 2.2: Create Log Analytics Workspace

In this step we set up the logging backend for our SOC lab SIEM.  
A dedicated Log Analytics Workspace is used as the central location for security telemetry.

We used a dedicated resource group and chose Sweden Central as region.  
Log ingestion is intentionally not enabled yet to avoid any cost during the Azure Free Trial.

#### Workspace overview

Here is the workspace overview right after creation:

![Log Analytics Workspace overview](../screenshots/setup/03-law-overview.PNG)

This shows the workspace name, resource group and region.

#### Cost validation

We verified the workspace usage immediately after creation to ensure that no logs are being ingested and that the estimated cost remains zero.

![Usage and estimated costs](../screenshots/setup/04-law-usage-zero.PNG)

At this stage the workspace shows:
- 0 GB ingested
- Estimated cost 0 USD

This confirms that we stay within Free Trial limits.

#### Current status

The Log Analytics Workspace is ready and prepared for Microsoft Sentinel in the next step.  
No logs are ingested yet and no costs are generated.
