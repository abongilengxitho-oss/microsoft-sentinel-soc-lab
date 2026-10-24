# Simulated Incident Report: Suspicious Successful Login

## Incident Details

- **Incident ID:** SIM-002
- **Scenario:** Hypothetical unusual successful Windows logon
- **Severity:** Medium (proposed)
- **Status:** Simulated exercise — no real incident confirmed

## Scenario

For this exercise, assume a Windows account successfully logs in at an unusual time or from a source that is unfamiliar to the organisation.

A successful login is not inherently malicious. The analyst must assess the surrounding evidence before deciding whether the activity is suspicious.

## Relevant Event

- **Windows Event ID:** 4624 — successful logon
- **Related query:** `kql-queries/successful-login-investigation.kql`

## Investigation Steps

1. Identify the account, computer, timestamp, and logon type.
2. Compare the activity with the user's normal working pattern, if authorised baseline information is available.
3. Review source IP information where it is recorded and meaningful.
4. Correlate with nearby failed logons and other relevant security events.
5. Check whether the activity is consistent with approved remote access or routine administration.
6. Document evidence gaps and decide whether further investigation is warranted.

## Hypothetical Assessment

No live event data has been analysed for this report. An unusual time or unfamiliar source alone is insufficient to conclude that an account has been compromised.

A stronger assessment would require corroborating evidence, such as unexpected authentication patterns or other suspicious activity.

## Recommended Response

If additional evidence indicates possible account compromise:

- Escalate through the appropriate security process.
- Preserve relevant logs.
- Follow approved account-protection and containment procedures.
- Document the rationale for each action.
- Review detection logic and potential false positives.

## Lessons Learned

Successful authentication events provide useful context when correlated with other activity. Analysts should avoid treating a single unusual login as proof of an attack.

## Validation Status

This is a simulated tabletop exercise. No real suspicious login has been confirmed, and live detection validation remains outstanding.
