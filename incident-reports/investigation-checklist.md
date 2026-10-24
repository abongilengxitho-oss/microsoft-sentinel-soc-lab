# SOC Analyst Investigation Checklist

## 1. Alert Triage

- [ ] Record the alert name, time, and severity.
- [ ] Identify the affected account and computer.
- [ ] Confirm which data source generated the alert.
- [ ] Determine whether the alert is based on real, simulated, or unvalidated data.

## 2. Authentication Review

- [ ] Review failed logon events (Windows Event ID 4625).
- [ ] Review successful logon events (Windows Event ID 4624), if available.
- [ ] Compare event timestamps and frequency.
- [ ] Review logon types and available source IP addresses.
- [ ] Check for repeated attempts involving one or multiple accounts.

## 3. Evidence and Correlation

- [ ] Correlate related events within an appropriate time window.
- [ ] Check whether the activity matches expected user behaviour.
- [ ] Consider legitimate explanations, such as mistyped or expired credentials.
- [ ] Record relevant evidence without exposing unnecessary personal information.
- [ ] Identify missing logs or fields that limit the investigation.

## 4. Assessment

- [ ] Decide whether the evidence supports suspicious activity.
- [ ] Document alternative explanations and uncertainty.
- [ ] Assign a severity based on evidence and potential impact.
- [ ] Escalate unresolved or high-risk activity according to the organisation's procedures.

## 5. Response and Closure

- [ ] Recommend proportionate containment or account-protection measures if justified.
- [ ] Record actions taken and who authorised them.
- [ ] Document the final assessment and supporting evidence.
- [ ] Identify detection improvements and lessons learned.

## Lab Note

This checklist is a training aid. Do not mark investigation steps as completed unless the relevant actions have actually been performed. Clearly distinguish simulated exercises from investigations based on real event data.
