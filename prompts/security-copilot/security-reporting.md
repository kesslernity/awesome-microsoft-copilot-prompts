# Copilot for Security — Security Reporting & Management

> 15 SCU-optimized prompts for security managers, CISOs, and compliance leads. Focused on translating security data into decisions: vulnerability reports, compliance posture, board briefings, and audit responses.

**REQUIRES:** Microsoft Copilot for Security (standalone portal or embedded experience). See the [README](./README.md) for SCU and licensing details.

**Category:** Security Management & Reporting

**Prompts:** 15

---

## SCU NOTE

These prompts are structured for single-interaction execution. Each includes a data source, scope, and output format. Use them as written to keep SCU consumption low. Open-ended variants ("summarize my security posture") will burn significantly more SCUs with less useful output.

---

## Vulnerability Reporting

### 1. Monthly Vulnerability Summary for Leadership

Use at the end of each month to produce a consistent vulnerability posture report without manually pulling data.

**Target Personas:** Security Manager, CISO, Vulnerability Management Lead

**Tags:** `vulnerability`, `reporting`, `defender-xdr`, `leadership`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR (Threat & Vulnerability Management), produce a monthly vulnerability summary for [MONTH/YEAR].

Include:
1. Total open vulnerabilities at end of month: breakdown by severity (critical, high, medium, low)
2. Vulnerabilities remediated this month: count and percentage of total open
3. New vulnerabilities discovered this month: count
4. Top 5 vulnerabilities by number of affected devices (include CVE ID, description, device count, and patch availability)
5. Mean time to remediate (MTTR) for critical vulnerabilities this month, if available
6. Devices with the highest number of unpatched critical vulnerabilities: top 5

Format as a one-page management report. Use plain language for the summary section — this will be reviewed by non-technical stakeholders.
```

---

### 2. Patch Compliance Report by Business Unit

Use to track patch compliance across organisational units and identify which teams are creating risk.

**Target Personas:** Security Manager, IT Director, Compliance Lead

**Tags:** `vulnerability`, `patch-compliance`, `defender-xdr`, `reporting`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR (Threat & Vulnerability Management), generate a patch compliance report.

For devices grouped by [DEPARTMENT / LOCATION / DEVICE GROUP — specify which dimension is configured in your environment]:
1. Count of devices per group
2. Percentage of devices fully patched (no critical or high vulnerabilities)
3. Percentage with at least one unpatched critical vulnerability
4. The single highest-severity unpatched CVE in each group

Return as a table sorted by patch compliance percentage ascending (worst first). Flag any group below 70% patch compliance.
```

---

### 3. Zero-Day and Active Exploit Exposure Check

Use immediately when a new zero-day or actively exploited CVE is announced.

**Target Personas:** CISO, Security Manager, SOC Lead

**Tags:** `zero-day`, `cve`, `active-exploit`, `defender-xdr`, `executive`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender XDR (Threat & Vulnerability Management), check our environment's exposure to [CVE ID].

Provide:
1. Are any devices in the environment running affected software versions? If yes, how many?
2. List the top 10 most critical affected devices (prioritise servers and devices handling sensitive data)
3. Is a patch or official mitigation available from the vendor?
4. Has this CVE been observed in active exploitation in the wild (check threat intelligence if available)?
5. Recommended immediate action: patch now, apply workaround, monitor, or no action

I need this within the next 30 minutes — prioritise speed over completeness. Flag anything I need to verify manually.
```

---

## Compliance & Audit

### 4. Compliance Posture Summary — Microsoft Purview

Use for quarterly compliance reviews or ahead of external audits.

**Target Personas:** Compliance Manager, CISO, Internal Audit

**Tags:** `compliance`, `purview`, `audit`, `posture`, `scu-efficient`

**Prompt:**

```
In Microsoft Purview Compliance Manager, provide a compliance posture summary for [DATE or QUARTER].

Include:
1. Overall compliance score and how it has changed since last quarter
2. Top 3 regulatory frameworks with the highest and lowest compliance scores
3. Improvement actions that are overdue or approaching their deadline
4. Any controls that were compliant last quarter and are now non-compliant (regression)
5. The 5 improvement actions with the highest score impact if completed

Format as a quarterly compliance brief suitable for the board risk committee.
```

---

### 5. Audit Log Export Summary — User Activity

Use when responding to an internal or external audit request for user activity records.

**Target Personas:** Compliance Analyst, Security Manager, Legal

**Tags:** `audit`, `purview`, `user-activity`, `compliance`, `scu-efficient`

**Prompt:**

```
In Microsoft Purview Audit, search for all activity by user [UPN] between [START DATE] and [END DATE].

Include:
1. A summary of the types of activity recorded (e.g. file access, email send, Teams messages, admin actions)
2. Total count of events per activity type
3. Any high-risk activities: bulk file download, sharing to external recipients, deletion events, or permission changes
4. A chronological table of the 20 most significant events (timestamp, activity, target resource, outcome)

This is for an audit response. Do not include any inference or opinion — factual activity log only.
```

---

### 6. Data Retention and DLP Policy Coverage Check

Use to verify that DLP and retention policies cover your critical data types before an audit.

**Target Personas:** Compliance Manager, DLP Analyst

**Tags:** `dlp`, `retention`, `purview`, `policy-coverage`, `scu-efficient`

**Prompt:**

```
In Microsoft Purview, review the current state of DLP and retention policies.

Provide:
1. List all active DLP policies: name, sensitive information types covered, workloads (Exchange, SharePoint, Teams, Endpoint), and enforcement mode (enforce, audit, or report-only)
2. List all active retention policies: name, retention period, and workloads covered
3. Identify any workloads with no active DLP policy
4. Identify any sensitive information types (e.g. credit card, national ID, health data) not covered by any active policy
5. Flag any policies in report-only mode that should be enforced

Return as a coverage matrix table. Mark gaps in red (missing coverage) and report-only policies in amber.
```

---

## Identity & Access Reporting

### 7. Privileged Access Review Report

Use for quarterly privileged access reviews (PAR) required by ISO 27001, SOC 2, and similar frameworks.

**Target Personas:** Security Manager, Identity Lead, Internal Audit, CISO

**Tags:** `privileged-access`, `entra`, `access-review`, `compliance`, `scu-efficient`

**Prompt:**

```
In Microsoft Entra ID, produce a privileged access review report for [QUARTER/YEAR].

Include:
1. All users with permanent Global Administrator, Security Administrator, or Privileged Role Administrator roles
2. For each: display name, UPN, account type (member/guest), MFA status, last sign-in date, and whether the assignment is PIM-eligible or permanent
3. Users with privileged roles who have not signed in within the last 90 days
4. Guest accounts with any privileged role assignment
5. Changes to privileged role assignments in the last 90 days: who was added, who was removed, and by whom

Format as a formal access review report. Flag accounts that should be reviewed for removal.
```

---

### 8. Stale Account Report

Use for periodic hygiene reviews or ahead of audits — stale accounts are a common audit finding.

**Target Personas:** Identity Administrator, Security Manager, Compliance Analyst

**Tags:** `stale-accounts`, `entra`, `identity-hygiene`, `audit`, `scu-efficient`

**Prompt:**

```
In Microsoft Entra ID, identify stale accounts — users who have been inactive for 90 days or more.

For each stale account:
1. Display name and UPN
2. Account type (member or guest)
3. Last sign-in date
4. Assigned licences (M365, Azure, or other)
5. Group memberships that grant access to sensitive resources (if identifiable)

Return a table sorted by last sign-in date ascending (most stale first). Separate member accounts from guest accounts. Include a total count for each category.

Do not disable or delete any accounts — report only.
```

---

## Threat Reporting for Management

### 9. Weekly Threat Landscape Briefing

Use to produce a consistent weekly threat briefing for the security leadership team.

**Target Personas:** CISO, Security Director, SOC Lead

**Tags:** `threat-briefing`, `reporting`, `defender-xdr`, `sentinel`, `leadership`, `scu-efficient`

**Prompt:**

```
Produce a weekly threat landscape briefing for the week of [DATE RANGE].

Using data from Microsoft Defender XDR and Microsoft Sentinel:
1. Incidents this week: total count by severity. How does this compare to the previous week?
2. Most prevalent attack techniques observed (MITRE ATT&CK tactics): top 3
3. Most targeted users or devices this week: list top 5 with a brief note on why they were targeted
4. Threat intelligence: any new threat actors or malware campaigns relevant to our industry observed this week?
5. Ongoing risks: any incidents or investigations still open from prior weeks?

Format as a one-page management briefing. Maximum 400 words. Flag anything requiring immediate leadership attention at the top.
```

---

### 10. Security Incident Communication — External Notification Draft

Use when a breach or significant incident may require external notification (customers, regulators, or partners).

**Target Personas:** CISO, Legal, Communications, Security Manager

**Tags:** `incident-communication`, `breach-notification`, `legal`, `scu-efficient`

**Prompt:**

```
I need to draft an external notification regarding the following security incident: [BRIEF DESCRIPTION].

Audience: [SPECIFY — e.g. "affected customers", "data protection authority", "partner organisations"]
Regulatory framework applicable: [SPECIFY — e.g. "GDPR", "HIPAA", "NIS2", or "none confirmed yet"]

Draft a notification that includes:
1. What happened (factual, no speculation)
2. What data or systems were affected
3. What we have done in response
4. What the recipient should do, if anything
5. Who to contact for questions

Use plain language. Do not make admissions of liability. Mark any section requiring legal review with [LEGAL REVIEW REQUIRED]. I will not send this without legal approval.
```

---

### 11. CISO Board Report — Security Posture

Use quarterly for board-level security reporting.

**Target Personas:** CISO

**Tags:** `board-reporting`, `ciso`, `security-posture`, `executive`, `scu-efficient`

**Prompt:**

```
Produce a quarterly board security report for [QUARTER/YEAR].

Draw from Microsoft Defender XDR, Microsoft Sentinel, and Microsoft Purview Compliance Manager where available.

Structure:
1. Security Posture Score (if available): current score, trend vs. last quarter, and what drove the change
2. Incidents: total for the quarter, breakdown by severity, MTTR for critical incidents
3. Vulnerabilities: open critical/high count, remediation rate vs. target, top 3 unresolved risks
4. Compliance: current score, regulatory frameworks in scope, overdue improvement actions
5. Identity: privileged account count, MFA coverage percentage, stale account count
6. Top 3 security risks requiring board awareness
7. Investments or decisions needed from the board

Format as a board-ready presentation outline. Use plain language throughout. Flag where data must be manually added.
```

---

## Responding to Security Questionnaires

### 12. Security Questionnaire Response — Vendor/Customer

Use when a customer or vendor sends a security questionnaire and you need to draft responses grounded in your actual environment state.

**Target Personas:** Security Manager, CISO, Procurement Security

**Tags:** `security-questionnaire`, `vendor-assessment`, `compliance`, `scu-efficient`

**Prompt:**

```
I am responding to a security questionnaire from [VENDOR/CUSTOMER NAME]. The question is: "[PASTE QUESTION]"

Using what you know about our Microsoft security environment (Defender XDR, Purview, Entra, Sentinel), draft a factual response to this question.

Requirements:
- Be accurate — do not claim capabilities we haven't confirmed
- Mark any claim that requires manual verification with [VERIFY]
- Keep the response to 2–4 sentences unless the question requires detail
- Use professional, direct language appropriate for a vendor security review

I will review and approve the response before submitting.
```

---

### 13. Third-Party Risk Summary — Vendor with Elevated Access

Use when onboarding a new vendor with access to your Microsoft environment or reviewing an existing one.

**Target Personas:** Security Manager, Procurement Security, CISO

**Tags:** `third-party-risk`, `vendor`, `access-review`, `scu-efficient`

**Prompt:**

```
I am reviewing the security risk associated with vendor [VENDOR NAME], who has been granted [TYPE OF ACCESS — e.g. "guest access to SharePoint", "Entra B2B access", "Global Admin role"].

In Microsoft Entra ID, provide:
1. All guest accounts associated with this vendor's domain ([VENDOR DOMAIN])
2. Roles or group memberships assigned to these accounts
3. Last sign-in date for each guest account
4. Any conditional access policies applied to these accounts
5. Any security alerts or risk events associated with these accounts in the last 90 days

Return as a third-party access report. Flag any account with privileged access or no recent sign-in activity.
```

---

### 14. Security Awareness Training Compliance Report

Use to track mandatory security training completion and identify non-compliant staff before an audit.

**Target Personas:** Security Manager, HR, Compliance

**Tags:** `security-training`, `compliance`, `reporting`, `scu-efficient`

**Prompt:**

```
In Microsoft Defender for Office 365 (Attack Simulator / Training), produce a training compliance report for [TRAINING CAMPAIGN NAME or "all active campaigns"].

Include:
1. Total users assigned to the training
2. Completion rate (percentage and absolute numbers)
3. Users who have not completed the training: list by department if available, sorted by days since assignment
4. For phishing simulation campaigns: click rate, credential submission rate, and reported rate
5. Comparison to the previous campaign if data is available

Flag any department with completion below 80%. This report will be reviewed by HR and the compliance team.
```

---

### 15. Security Metrics Dashboard Preparation

Use to pull the raw metrics you need before building or updating a security dashboard or scorecard.

**Target Personas:** Security Manager, SOC Lead, CISO

**Tags:** `metrics`, `kpi`, `reporting`, `defender-xdr`, `sentinel`, `scu-efficient`

**Prompt:**

```
Pull the following security metrics for [PERIOD — e.g. "last 30 days" or "Q1 2026"] from Microsoft Defender XDR and Microsoft Sentinel:

1. Total incidents: breakdown by severity
2. Mean time to detect (MTTD): average time from first alert to incident creation
3. Mean time to respond (MTTR): average time from incident creation to resolution, for critical and high severity
4. False positive rate: percentage of alerts closed as false positive
5. Alert volume by data source (Defender XDR, Sentinel, Entra, Purview)
6. Top 5 MITRE ATT&CK techniques observed
7. Devices with active critical alerts: count

Return as a metrics table. Flag any metric where data is unavailable or may be incomplete, and note what manual query would retrieve it.
```

---

## Navigation

← Back to [Security Copilot README](./README.md) | [SOC Operations Prompts](./soc-operations.md)

---

**License:** CC BY-SA 4.0 · [NerdyChefs.ai](https://nerdychefs.ai) · [AI at Work Newsletter](https://newsletter.kesslernity.com/?utm_source=github&utm_medium=readme&utm_campaign=prompts_repo&utm_content=seccopilot_reporting)
