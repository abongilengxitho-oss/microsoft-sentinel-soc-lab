# Microsoft Sentinel SOC Lab Architecture

## Project Purpose

This lab demonstrates fundamental Security Operations Centre (SOC) workflows using Microsoft Sentinel, Log Analytics, and Kusto Query Language (KQL).

## Planned Architecture

1. **Windows endpoint:** A Windows 11 computer intended as a potential source of security events, subject to compatibility and safe configuration checks.
2. **Log collection:** A compatible, cost-conscious collection method to be selected after confirming endpoint eligibility and Azure requirements.
3. **Log Analytics workspace:** `law-sc200-soc`, intended to store collected security data.
4. **Microsoft Sentinel:** The SIEM platform used to investigate security events and, after validation, configure detections.
5. **KQL queries:** Queries for investigating failed and successful Windows logons.
6. **Detection documentation:** Proposed detection logic, investigation steps, and false-positive considerations.
7. **GitHub portfolio:** Sanitised documentation, queries, validation notes, and future investigation reports.

## Current Status

- Azure subscription: Active at last check.
- Log Analytics workspace: Created.
- Microsoft Sentinel: Enabled for the workspace.
- KQL editor: Basic query test succeeded.
- Windows Security Events: Not yet confirmed in the workspace.
- Detection rule: Documented as a draft; not yet configured as a live analytics rule.
- Endpoint onboarding: Pending compatibility and cost review.

## Cost and Safety Controls

- Do not enable pay-as-you-go without reviewing the potential charges and obtaining explicit approval.
- Check current Azure pricing and free-credit terms before enabling new services or ingestion.
- Keep the Windows endpoint's existing work or school connection unchanged.
- Do not install agents or onboard the endpoint until eligibility and cost implications are understood.
- Never commit credentials, tokens, tenant identifiers, subscription identifiers, or raw sensitive logs to the public repository.
- Azure budgets provide alerts; they do not automatically stop spending.

## Planned Validation

1. Confirm the permitted data-collection path for the available Windows edition.
2. Review the cost implications before enabling any additional resources.
3. Confirm security events are arriving in the workspace.
4. Test and refine the KQL queries against actual events.
5. Configure a Sentinel analytics rule only after validating the query.
6. Document results accurately, distinguishing real evidence from simulated examples.

## Project Status

**In progress.** The workspace and initial portfolio documentation exist, but endpoint ingestion and live detection validation remain outstanding.
