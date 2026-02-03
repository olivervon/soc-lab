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
