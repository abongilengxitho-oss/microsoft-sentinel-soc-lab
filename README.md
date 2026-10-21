# Microsoft Sentinel SOC Lab

## Project Overview

This project demonstrates a hands-on Security Operations Centre (SOC) lab built around Microsoft Sentinel. It focuses on security monitoring, threat detection, threat hunting, and incident response.

The goal is to develop practical skills aligned with the Microsoft SC-200 Security Operations Analyst learning path.

**Project status:** In progress

## Objectives

- Understand Microsoft Sentinel and SIEM operations.
- Explore security logs using Kusto Query Language (KQL).
- Detect suspicious authentication activity.
- Develop and test security detection queries.
- Investigate alerts and document security incidents.
- Recommend appropriate containment and remediation actions.

## Tools and Technologies

- Microsoft Sentinel
- Microsoft Azure
- Azure Log Analytics
- Kusto Query Language (KQL)
- Windows Security Events
- Ubuntu/Linux system logs (planned integration)
- GitHub for documentation and version control

## Planned Detection Scenarios

### 1. Multiple Failed Logins
Identify repeated failed Windows authentication attempts and investigate potential brute-force activity.

### 2. Suspicious Sign-in Activity
Examine authentication events for unusual patterns that may require further investigation.

### 3. Suspicious Process Activity
Explore endpoint telemetry for potentially suspicious process execution and command activity.

## Project Workflow

1. Configure the lab environment.
2. Connect and validate security log sources.
3. Develop KQL queries for threat hunting.
4. Configure and test detection rules.
5. Investigate generated alerts and incidents.
6. Document findings and remediation recommendations.

## Repository Structure

- `setup/` — Environment setup and configuration.
- `architecture/` — Lab architecture and data flow.
- `kql-queries/` — Threat-hunting queries.
- `detections/` — Detection logic and analytics rules.
- `incident-reports/` — Investigation reports.
- `screenshots/` — Sanitised project evidence.
- `lessons-learned.md` — Findings and improvements.

## Learning Outcomes

This project aims to develop practical knowledge of SIEM operations, KQL, security event analysis, threat detection, incident triage, and incident response.

## Disclaimer

This project is for educational and defensive cybersecurity purposes. Testing will be conducted only in authorised environments using controlled or simulated security events.

Project components will be updated as implementation and testing progress.

**Author:** Abongile Ngxitho  
**GitHub:** https://github.com/abongilengxitho-oss
