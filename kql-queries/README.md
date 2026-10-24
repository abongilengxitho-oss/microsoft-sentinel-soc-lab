# KQL Queries — Microsoft Sentinel SOC Lab

## Overview

This folder contains Kusto Query Language (KQL) queries developed for a Microsoft Sentinel security operations lab. The queries are designed to support Windows authentication monitoring, threat hunting, and security investigations.

## Queries

### 1. Failed Login Detection
**File:** `failed-login-detection.kql`

Identifies repeated failed Windows logon attempts (Event ID 4625), grouped by account, computer, and 15-minute interval. The current threshold flags groups with five or more failures.

**Investigation goal:** Identify possible brute-force attempts or suspicious authentication patterns.

### 2. Failed Login Investigation
**File:** `failed-login-investigation.kql`

Lists failed Windows logon events from the last 24 hours, including available timestamps, computer names, account names, failure details, and source IP addresses.

**Investigation goal:** Review authentication failures and identify patterns requiring further investigation.

### 3. Successful Login Investigation
**File:** `successful-login-investigation.kql`

Lists successful Windows logon events (Event ID 4624) from the last 24 hours, including available account, computer, logon type, and source IP information.

**Investigation goal:** Review successful authentication activity and investigate unusual logon patterns.

## Testing Status

These queries are currently portfolio drafts. They have not yet been validated against a confirmed collection of Windows security events in the lab.

Field availability and event details can vary depending on the data source and schema. Queries must be tested and adjusted before being used as production detections.

## Planned Improvements

- Connect an eligible Windows event source safely.
- Validate queries against real security events.
- Refine detection thresholds and investigate false positives.
- Document findings with sanitized screenshots and incident reports.
