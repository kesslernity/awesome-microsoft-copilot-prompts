# Copilot for Security — SOC Operations

> 20 SCU-optimized prompts for SOC analysts. Each prompt specifies the data source, scope, and output format to minimize follow-up interactions and SCU consumption.

**REQUIRES:** Microsoft Copilot for Security (standalone portal or embedded experience). These prompts do NOT work in Microsoft 365 Copilot Chat. Copilot for Security requires separate provisioning — see the [README](./README.md) for SCU and licensing details.

**Category:** Security Operations

**Prompts:** 20

---

## SCU NOTE — Read Before Using

Each prompt below follows the 4-element structure (goal + data source + scope + output format). Using prompts as written keeps SCU consumption to 1–2 per interaction. Modifying them to be more open-ended (removing the data source, removing the output format) will increase SCU consumption.

---

## Incident Triage

### 1. First Look — Incident Summary

Use when a new high-severity incident lands and you need a fast, structured overview before diving in.

**Target Personas:** SOC Analyst L1/L2, Incident Responder

**Tags:** `incident`, `triage`, `defender-xdr`, `scu-efficient`

**Prompt:**

```
Summarize incident [INCIDENT ID] in Microsoft Defender XDR. Include:
1. What happened (one paragraph, plain language)
2. Affected entities: list all users and devices involved
3. Attack timeline: key events in chronological order
4. Current status: contained, active, or unknown
5. Recommended immediate actions

Format as a structured incident brief. Flag any entity that appears across more than one alert in this incident.
```

---

### 2. Alert Triage — Is This a True Positive?

Use to quickly assess whether an alert warrants escalation before spending time on full investigation.

**Target Personas:** SOC Analyst L1, Tier 1 Triage

**Tags:** `alert`, `triage`, `defender-xdr`, `false-positive`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR, analyze alert [ALERT ID]. 

Answer these questions:
1. What activity triggered this alert?
2. Has this alert type fired for this user or device before in the last 30 days? If yes, how many times and what was the resolution?
3. Is the triggering activity consistent with the user's normal behaviour based on available context?
4. What is your assessment: likely true positive, likely false positive, or requires investigation? State your reasoning in one paragraph.

Do not recommend remediation actions — assessment only.
```

---

### 3. Multi-Alert Correlation — Single Incident Thread

Use when multiple alerts across different products appear related and you need to determine if they form a single attack chain.

**Target Personas:** SOC Analyst L2/L3, Threat Hunter

**Tags:** `correlation`, `defender-xdr`, `sentinel`, `attack-chain`, `scu-efficient`

**Prompt:**

```
I have the following alert IDs that may be related: [LIST ALERT IDs].

In Microsoft Defender XDR, examine these alerts and determine:
1. Do these alerts share common entities (users, devices, IPs, file hashes)? List the shared entities.
2. Is there a logical sequence — do any alerts appear to be precursors or consequences of others?
3. Should these be merged into a single incident? State yes or no with one-paragraph reasoning.

Return a table of alerts with columns: Alert ID, Timestamp, Entity, Tactic (MITRE), and your correlation assessment.
```

---

### 4. Device Investigation — Rapid Scope

Use to quickly establish what a device has been doing around the time of an alert before deciding whether to isolate.

**Target Personas:** SOC Analyst L2, Incident Responder

**Tags:** `device`, `defender-xdr`, `endpoint`, `investigation`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR, investigate device [DEVICE NAME or ID].

For the period [START TIME] to [END TIME]:
1. List all processes executed — flag any that are unusual, unsigned, or living-off-the-land binaries (LOLBins)
2. List all network connections — flag any to external IPs or uncommon destinations
3. List all file events — flag any new executables dropped or scripts run
4. Was any lateral movement attempted from this device?

Return findings as a structured table per category. Flag items that require immediate action.
```

---

### 5. User Investigation — Credential Compromise Assessment

Use when a user account shows anomalous behaviour or is referenced in an alert.

**Target Personas:** SOC Analyst L2, Identity Security Analyst

**Tags:** `identity`, `entra`, `credential-compromise`, `sign-in`, `scu-efficient`

**Prompt:**

```
In Microsoft Entra ID, investigate user [UPN or display name].

For the last 72 hours:
1. List all sign-in events. For each: timestamp, location, IP address, device, application, risk level, and outcome (success/failure/interrupted)
2. Flag any sign-ins from new locations, new devices, or impossible travel scenarios
3. Were any MFA prompts denied or bypassed?
4. Were any privileged roles assigned or modified on this account in this period?

Return a table of sign-in events sorted by timestamp. Highlight high-risk events in bold.
```

---

### 6. Email Threat Analysis

Use to investigate a suspicious email that has been reported or flagged by Defender for Office 365.

**Target Personas:** SOC Analyst L1/L2, Email Security Analyst

**Tags:** `email`, `defender-office365`, `phishing`, `malware`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR (email & collaboration), investigate the email with [message ID / subject / sender] received by [recipient UPN] on [date].

Provide:
1. Sender details: display name, actual sending address, sending IP, and reputation
2. URL analysis: list all URLs in the email and their verdict (safe, suspicious, malicious, unknown)
3. Attachment analysis: list attachments, file type, hash, and verdict if available
4. Delivery action taken by Defender: what happened to the email?
5. Was this email sent to other recipients in the organisation? If yes, how many?

Conclude with a one-paragraph verdict: phishing, malware delivery, business email compromise, spam, or benign.
```

---

## Threat Hunting

### 7. Hunting — Suspicious PowerShell Execution

Use to hunt for LOLBin/PowerShell abuse patterns across your environment.

**Target Personas:** Threat Hunter, SOC Analyst L3

**Tags:** `threat-hunting`, `powershell`, `lolbin`, `defender-xdr`, `kql`

**Prompt:**

```
In Microsoft Defender XDR advanced hunting, write and run a KQL query to find PowerShell executions in the last 7 days where:
- The process was launched by a non-standard parent (not explorer.exe, svchost.exe, or scheduled tasks)
- The command line contains encoded commands (-EncodedCommand or -enc) or downloads (Invoke-WebRequest, IEX, DownloadString)

Return results as a table with columns: device name, initiating process, PowerShell command line (truncated to 200 chars), timestamp, and logged-in user. Sort by timestamp descending. Limit to 50 results.
```

---

### 8. Hunting — Lateral Movement via SMB/PsExec

Use to identify potential lateral movement patterns in your environment.

**Target Personas:** Threat Hunter, SOC Analyst L3

**Tags:** `threat-hunting`, `lateral-movement`, `smb`, `defender-xdr`, `kql`

**Prompt:**

```
In Microsoft Defender XDR advanced hunting, write and run a KQL query to identify potential lateral movement in the last 48 hours.

Look for:
- Remote service creation events (ServiceControlManager)
- PsExec or equivalent tool usage (process name or command line contains psexec, paexec, or remcom)
- Network connections on port 445 (SMB) originating from workstations (not servers)

Return a table: source device, destination device, tool or method used, timestamp, and initiating user. Flag any source device that attempted lateral movement to more than 2 destinations.
```

---

### 9. Hunting — Persistence Mechanisms

Use when investigating a suspected compromise and you want to check for persistence before containment.

**Target Personas:** Threat Hunter, Incident Responder

**Tags:** `threat-hunting`, `persistence`, `registry`, `scheduled-tasks`, `defender-xdr`

**Prompt:**

```
In Microsoft Defender XDR advanced hunting, search for persistence mechanisms created in the last [TIMEFRAME] on device [DEVICE NAME or all devices].

Check for:
1. New scheduled tasks created by non-system accounts
2. Registry run key modifications (HKLM\Software\Microsoft\Windows\CurrentVersion\Run and HKCU equivalent)
3. New services created
4. Startup folder modifications

For each finding: device, user who made the change, timestamp, and the specific value or command added. Flag anything added by non-administrative accounts or pointing to temp/appdata directories.
```

---

### 10. Threat Intelligence Enrichment — IOC Lookup

Use to enrich an IOC (IP, domain, file hash) with threat intelligence context before deciding on response actions.

**Target Personas:** SOC Analyst L2/L3, Threat Intelligence Analyst

**Tags:** `threat-intelligence`, `ioc`, `mdti`, `enrichment`, `scu-efficient`

**Prompt:**

```
Using Microsoft Defender Threat Intelligence, look up the following indicator: [IP ADDRESS / DOMAIN / FILE HASH].

Provide:
1. Reputation score and verdict (malicious, suspicious, benign, unknown)
2. Associated threat actors or malware families, if any
3. First seen and last seen dates in threat intelligence feeds
4. Related CVEs or exploits associated with this indicator
5. Has this indicator been observed in your organisation's environment in the last 30 days? If yes, on which devices or by which users?

Return as a structured brief. Conclude with a recommended action: block, monitor, or no action needed.
```

---

## Identity & Access

### 11. Privileged Account Audit

Use for routine checks on privileged accounts or before/after a change freeze.

**Target Personas:** Identity Security Analyst, SOC Analyst L2

**Tags:** `identity`, `entra`, `privileged-access`, `audit`, `scu-efficient`

**Prompt:**

```
In Microsoft Entra ID, list all users currently assigned to the following roles: Global Administrator, Security Administrator, and Privileged Role Administrator.

For each user:
1. Display name and UPN
2. Account type (member or guest)
3. MFA status (registered, not registered, or enforced by conditional access)
4. Last sign-in date
5. Whether the role is permanent or time-limited (PIM-eligible)

Return as a table. Flag any guest accounts with privileged roles, any accounts with no MFA, and any accounts with no sign-in in the last 90 days.
```

---

### 12. Conditional Access Gap Analysis

Use to identify users who may be operating outside conditional access policy coverage.

**Target Personas:** Identity Security Analyst, Security Administrator

**Tags:** `conditional-access`, `entra`, `policy-gap`, `scu-efficient`

**Prompt:**

```
In Microsoft Entra ID, analyse the conditional access policies currently in place.

Identify:
1. Policies that are in report-only mode (not enforced)
2. Users or groups explicitly excluded from policies that require MFA or compliant device
3. Applications not covered by any conditional access policy
4. Sign-in events in the last 7 days that were interrupted or failed due to conditional access — list the top 10 by frequency

Return findings as a structured gap report with a priority column (high / medium / low) based on the exposure level of each gap.
```

---

## Vulnerability Management

### 13. Vulnerability Prioritisation

Use to cut through a long vulnerability list and focus remediation effort on what matters most.

**Target Personas:** Vulnerability Management Analyst, SOC Analyst L2

**Tags:** `vulnerability`, `defender-xdr`, `remediation`, `cvss`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR (Threat & Vulnerability Management), list all critical and high-severity vulnerabilities (CVSS 7.0 and above) currently active in the environment.

For each vulnerability:
1. CVE ID and name
2. CVSS score
3. Number of affected devices
4. Whether a public exploit exists (yes/no)
5. Recommended remediation action

Sort by number of affected devices descending. Return the top 20. Flag any CVE with a public exploit as requiring immediate attention.
```

---

### 14. Single CVE Impact Assessment

Use when a new CVE is published or reported and you need to know your exposure fast.

**Target Personas:** Vulnerability Management Analyst, SOC Analyst

**Tags:** `vulnerability`, `cve`, `defender-xdr`, `impact-assessment`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR (Threat & Vulnerability Management), assess the organisation's exposure to [CVE ID].

Provide:
1. CVE description in plain language (two sentences maximum)
2. Affected software and versions
3. Number of devices in the environment running affected versions
4. List the top 10 most exposed devices (by exposure score or business criticality if available)
5. Is a patch or mitigation available? If yes, what is it?
6. Has this CVE been linked to active exploitation in the wild?

Return as a one-page impact brief.
```

---

## Compliance & DLP

### 15. DLP Alert Investigation

Use to investigate a data loss prevention alert before deciding on escalation or user notification.

**Target Personas:** SOC Analyst, Compliance Analyst, DLP Analyst

**Tags:** `dlp`, `purview`, `data-loss`, `compliance`, `scu-efficient`

**Prompt:**

```
In Microsoft Purview, investigate DLP alert [ALERT ID or description].

Provide:
1. What sensitive data type was detected (e.g. credit card numbers, PII, classified content)?
2. What action triggered the alert — email send, file share, Teams message, or other?
3. Who was the user involved and what was the destination (internal or external)?
4. Was the data actually exfiltrated, or was it caught before leaving the organisation?
5. What policy was triggered and what action did it take (block, notify, audit only)?

Conclude with a recommended next step: close as false positive, notify user, escalate to HR/Legal, or initiate formal investigation.
```

---

### 16. Insider Risk Signal Review

Use for periodic review of insider risk signals or when a user is flagged for HR/Legal review.

**Target Personas:** Compliance Analyst, SOC Analyst L2

**Tags:** `insider-risk`, `purview`, `compliance`, `scu-efficient`

**Prompt:**

```
In Microsoft Purview Insider Risk Management, review the current open alerts for user [UPN].

Provide:
1. Alert summary: what risk indicators triggered the alert?
2. Activity timeline: what actions did the user take that contributed to the risk score?
3. Risk score and severity level
4. Has this user had prior alerts in the last 90 days?
5. What policies is this user included in?

Do not recommend disciplinary action. Return a factual activity summary suitable for review by HR or Legal.
```

---

## Reporting

### 17. Incident Post-Mortem Draft

Use after incident closure to produce a structured post-mortem without starting from a blank page.

**Target Personas:** Incident Commander, SOC Lead, Security Manager

**Tags:** `post-mortem`, `reporting`, `incident`, `defender-xdr`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR, retrieve the full details of incident [INCIDENT ID], which is now closed.

Draft a post-mortem report with the following sections:
1. Executive Summary (3 sentences: what happened, impact, how it was resolved)
2. Timeline of Events (chronological, key milestones only)
3. Root Cause
4. Impact Assessment (systems affected, data involved, business disruption)
5. Response Actions Taken
6. Lessons Learned (minimum 3)
7. Recommended Improvements

Mark any section where you have insufficient data with [REQUIRES MANUAL INPUT]. I will complete those sections before sending.
```

---

### 18. Daily Threat Digest

Use to produce a consistent daily threat summary for the SOC team or security leadership.

**Target Personas:** SOC Lead, Security Manager, CISO

**Tags:** `reporting`, `daily-digest`, `defender-xdr`, `sentinel`, `scu-efficient`

**Prompt:**

```
Produce a daily security digest for [DATE].

Using Microsoft Defender XDR and Microsoft Sentinel:
1. New incidents opened in the last 24 hours: count by severity (critical, high, medium, low)
2. Top 3 incidents by severity: for each, one-sentence summary and current status
3. Alerts closed as false positive in the last 24 hours: count
4. Any active threat hunts or ongoing investigations: status update
5. Vulnerabilities newly discovered in the last 24 hours with a CVSS score above 7.0

Format as a briefing note. Keep total length under 300 words. This will be shared with the security leadership team.
```

---

### 19. Executive Security Briefing (Non-Technical)

Use when you need to communicate security posture or an incident to a non-technical audience.

**Target Personas:** CISO, Security Manager, Communications Lead

**Tags:** `executive-reporting`, `non-technical`, `scu-efficient`

**Prompt:**

```
I need to brief [AUDIENCE — e.g. "the CFO and COO" or "the board risk committee"] on the following security event or posture update: [BRIEF DESCRIPTION].

Here are the technical details: [PASTE TECHNICAL SUMMARY].

Rewrite this as a non-technical briefing that:
1. Explains what happened or what the risk is in plain language (no jargon)
2. States the business impact clearly — what could happen if this isn't addressed?
3. Describes what has been done or is being done
4. States what decision or approval, if any, is needed from this audience

Keep it under 200 words. Do not soften the risk — be accurate about the potential impact.
```

---

### 20. KQL Query Generation — Save for Reuse

Use to generate a KQL query you can save, test, and reuse — avoiding repeated Copilot prompting for the same hunt.

**Target Personas:** Threat Hunter, SOC Analyst L3, Detection Engineer

**Tags:** `kql`, `sentinel`, `defender-xdr`, `query-generation`, `scu-efficient`

**Prompt:**

```
Write a KQL query for Microsoft Sentinel (or Defender XDR advanced hunting — specify which) that detects the following behaviour: [DESCRIBE THE BEHAVIOUR IN PLAIN LANGUAGE].

Requirements:
- The query should cover a configurable time window (use a variable at the top for easy adjustment)
- Include comments explaining each major section
- Return results as a table with columns: timestamp, entity (user or device), action, source, and severity if applicable
- Include a count of events per entity so I can identify which entities are generating the most hits

After the query, add a one-paragraph explanation of the detection logic and any known false positive scenarios I should filter out.
```

---

## Navigation

← Back to [Security Copilot README](./README.md) | [Security Reporting Prompts →](./security-reporting.md)

---

**License:** CC BY-SA 4.0 · [NerdyChefs.ai](https://nerdychefs.ai) · [AI at Work Newsletter](https://newsletter.kesslernity.com/?utm_source=github&utm_medium=readme&utm_campaign=prompts_repo&utm_content=seccopilot_soc)
