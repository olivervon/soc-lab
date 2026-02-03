# Lab Overview

This SOC lab simulates a small enterprise environment used to practice Tier 1 alert triage,
Tier 2 investigation, and basic incident response.

## Environment
- Hyper-V on a local workstation
- Windows Server (Active Directory, DNS)
- Windows 10 Endpoint
- Linux host (attack simulation)
- Azure + Microsoft Sentinel (SIEM)

## Log Flow
Endpoint and server logs are forwarded to Microsoft Sentinel for detection and investigation.
