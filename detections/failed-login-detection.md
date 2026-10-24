# Detection Rule: Repeated Failed Windows Logins

## Rule Overview

- **Detection name:** Repeated Failed Windows Logins
- **Platform:** Microsoft Sentinel
- **Data source:** Windows Security Events (`SecurityEvent`)
- **Event ID:** 4625
- **Severity:** Medium (proposed)
- **Status:** Draft — not yet validated against live event data

## Objective

Identify repeated failed Windows authentication attempts that may indicate a brute-force attack, password guessing, or another suspicious authentication pattern.

## Detection Logic

The associated KQL query groups failed logons by account, computer, and 15-minute interval. It flags groups containing five or more failed attempts.

**Query file:** `kql-queries/failed-login-detection.kql`

## Analyst Investigation Steps

1. Identify the affected account and computer.
2. Review the timestamps and frequency of the failed attempts.
3. Examine available source IP addresses and failure details.
4. Check whether successful logons occurred around the same period.
5. Determine whether the activity appears legitimate or suspicious.
6. Document the evidence and escalate according to the organisation's incident-response procedures.

## False-Positive Considerations

Repeated failures can result from mistyped passwords, expired credentials, saved credentials, or misconfigured services. The threshold is a starting point and should be tuned after reviewing real event data.

## Validation Plan

- Confirm that Windows security events are reaching the workspace.
- Run the query against available events.
- Verify the grouping and threshold logic.
- Test representative scenarios where authorised and safe.
- Record the results and adjust the query if necessary.

## Current Limitations

The lab has not yet confirmed Windows security-event ingestion. This rule is documentation for a planned detection and must not be represented as a working production alert.

The KQL query alone does not create a Microsoft Sentinel analytics rule or generate alerts. Those steps will be completed only after data ingestion and query validation.
