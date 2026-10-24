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

## Project Progress

### Completed Portfolio Components

- Created KQL queries for investigating failed and successful Windows logons.
- Documented a proposed repeated-failed-login detection.
- Documented the lab architecture and cost-safety considerations.
- Created a SOC analyst investigation checklist.
- Prepared simulated incident reports covering repeated failed logins and unusual successful logons.

### Skills Demonstrated

- Kusto Query Language (KQL)
- Windows authentication event analysis
- Security alert triage and investigation planning
- Detection logic and false-positive assessment
- Incident documentation and response recommendations
- Security monitoring concepts using Microsoft Sentinel
- GitHub documentation and version control

### Current Limitations

The lab workspace has been created and Microsoft Sentinel enabled, but Windows Security Event ingestion has not yet been confirmed.

The KQL queries remain drafts pending validation against suitable event data. The incident reports are simulated exercises, not confirmed security incidents. A live Sentinel analytics rule has not yet been validated as operational.

### Cost and Safety Approach

This project prioritises cost awareness and safe configuration. No additional endpoint agents are being installed while data-collection eligibility and cost implications are being reviewed. Azure pay-as-you-go remains disabled.

### Next Objectives

- Identify a suitable and affordable Windows event-collection method.
- Validate the KQL queries against event data when available.
- Refine detection logic and document testing results.
- Configure a live analytics rule if prerequisites are met.
- Capture sanitised evidence and publish a final project summary.



Project components will be updated as implementation and testing progress.

**Author:** Abongile Ngxitho  
**GitHub:** https://github.com/abongilengxitho-oss
