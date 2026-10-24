# Simulated Incident Report: Repeated Failed Logins

## Incident Details

- **Incident ID:** SIM-001
- **Scenario:** Simulated brute-force login attempt
- **Environment:** Microsoft Sentinel SOC lab
- **Severity:** Medium (proposed)
- **Status:** Simulated exercise — no real incident confirmed

## Scenario

For this exercise, assume an account receives multiple failed Windows authentication attempts within a short period. The pattern may indicate password guessing, but it could also result from a user entering an incorrect password repeatedly.

## Detection

The planned detection uses Windows Security Event ID 4625 and groups failed logons by account, computer, and 15-minute interval. Groups with five or more failures are flagged for investigation.

**Related query:** `kql-queries/failed-login-detection.kql`

## Investigation Plan

1. Identify the affected account and computer.
2. Establish the number and timing of failed attempts.
3. Review available logon failure details and source IP information.
4. Check for successful logons before or after the failures.
5. Determine whether the activity has a plausible legitimate explanation.
6. Recommend escalation if suspicious activity remains unexplained.

## Hypothetical Findings

No real event data has been analysed for this report. The scenario and findings are not evidence of an actual attack.

If validated event data later shows repeated failures from an unfamiliar source, the analyst should correlate the events and assess the risk before concluding that a brute-force attack occurred.

## Recommended Response

If the activity is confirmed to be malicious:

- Follow the organisation's incident-response process.
- Notify the appropriate security team.
- Consider account protection measures under approved procedures.
- Preserve relevant evidence and document the response.
- Review whether the detection threshold needs tuning.

## Lessons Learned

Repeated authentication failures are a useful investigation signal, but they do not independently prove malicious activity. Analysts should correlate events, consider false positives, and distinguish observed evidence from assumptions.

## Validation Status

This is a simulated tabletop exercise. Live Windows event collection and detection validation remain outstanding.
