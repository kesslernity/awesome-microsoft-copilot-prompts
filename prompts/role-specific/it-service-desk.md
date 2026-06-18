# Copilot for IT & Service Desk

> Master Microsoft 365 Copilot for IT operations, service desk, and M365 administration. Production-safe prompts for finding context, preparing changes, and drafting communications — with strict guardrails. Copilot researches; IT decides and executes.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Engineering & DevOps

**Prompts:** 16

---

## CRITICAL: IT GUARDRAILS - READ FIRST

### 1. IT Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any IT use of Copilot. Copilot prepares and researches; it never executes or decides.

**Target Personas:** IT Manager, Systems Administrator, Service Desk Lead, DevOps Engineer, CISO

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Use Copilot for IT

**Copilot output is research or a draft, never an action. NEVER use it for:**

### Execution
- Writing or deploying production code
- Making infrastructure or configuration changes (use IaC and change control)
- Active incident response or live remediation
- Resetting access, granting permissions, or changing accounts

### Security & Access
- Security assessments or vulnerability remediation decisions
- Access control / least-privilege decisions
- Password, secret, or credential handling
- Bypassing any security control

### Data
- Data handling, classification, or deletion decisions

**Security reminders:** never paste credentials; prompts may be logged; follow your org's AI policy.

**System note:** Copilot does NOT integrate with ServiceNow/ITSM, CMDB, DevOps pipelines, or security tools.

**Golden Rule:**
> "Copilot researches. IT decides and executes."
```

---

## Incident Management

### 2. Incident History Search

**Use Case:** Research previous incident resolutions to inform current troubleshooting. Verify applicability before acting.

**Target Personas:** IT Manager, Systems Administrator, Support Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `incidents`, `troubleshooting`

**Prompt:**

```
Search my emails and Teams for previous incidents related to [system/application] or [error type]. Compile:
- Incident descriptions
- Root causes identified
- Resolutions applied
- Workarounds documented

This is research for troubleshooting. I will verify applicability to the current issue before acting.
```

---

### 3. Post-Incident Review Prep

**Use Case:** Gather context for a blameless post-incident review. The review itself is a team decision.

**Target Personas:** IT Manager, SRE, DevOps Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `pir`, `incidents`

**Prompt:**

```
For the incident on [date/system], gather from emails and Teams a factual timeline:
- When it was detected and by whom
- Actions taken and at what time
- Communications sent
- When service was restored

Keep it factual and blameless — no fault attribution. This is preparation for the team's post-incident review, not the review's conclusions.
```

---

## Change Management

### 4. Change Request Preparation

**Use Case:** Research precedents to prepare a thorough change request. Approval remains a CAB decision.

**Target Personas:** IT Manager, Change Manager, Systems Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `change-management`

**Prompt:**

```
I'm preparing a change request for [change]. Search for:
- Similar changes previously implemented
- Risks or issues raised
- Approvals that were required
- Rollback procedures mentioned

Help me gather precedents for a thorough change request. This does not approve the change.
```

---

### 5. CAB Meeting Preparation

**Use Case:** Prepare for a Change Advisory Board meeting with context on pending changes.

**Target Personas:** IT Manager, Change Manager, CAB Member

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `cab`, `change-management`

**Prompt:**

```
I have a CAB meeting. Based on recent emails and Teams:
- What changes are pending approval?
- What concerns have been raised?
- Any failed changes being discussed?
- Risk assessments mentioned?

Prepare briefing notes for my preparation.
```

---

### 6. Change / Maintenance Communication Draft

**Use Case:** Draft user-facing comms for a planned change or maintenance window, for review before sending.

**Target Personas:** IT Manager, Service Desk Lead, IT Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `communication`, `change`

**Prompt:**

```
Draft a clear, non-technical notification for end users about [planned change/maintenance]:
- What is happening and why
- When (window) and expected impact
- What users need to do (if anything)
- Who to contact

Keep it calm and plain-language. This is a draft for review before sending.
```

---

## Service Desk

### 7. Ticket Theme Triage Prep

**Use Case:** Surface recurring themes from recent support requests to guide triage and problem management.

**Target Personas:** Service Desk Lead, IT Manager, Support Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `service-desk`, `triage`

**Prompt:**

```
Review support-related emails and Teams messages from the last [timeframe]. Identify:
- Recurring issue themes
- Systems/apps mentioned most
- Any emerging spike worth a problem record

This is exploratory input for triage and problem management, not a formal ticket analysis (which comes from the ITSM tool).
```

---

### 8. Outage Communication Draft

**Use Case:** Draft a service-status update during or after an outage, for review before publishing.

**Target Personas:** Service Desk Lead, IT Manager, IT Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `outage`, `communication`

**Prompt:**

```
Draft a service-status update about [system] being [degraded/unavailable]:
- What users are experiencing
- What we know and are doing (from the notes I provide)
- Workaround if any
- Next update time

Plain, reassuring, no speculation about cause. Draft for review — do not invent root cause or restoration times.
```

---

## Documentation

### 9. Technical Documentation Search

**Use Case:** Locate runbooks, SOPs, or technical docs and assess currency. Verify before relying on them.

**Target Personas:** IT Manager, Systems Administrator, DevOps Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `documentation`, `runbooks`

**Prompt:**

```
Find runbooks, SOPs, or technical documentation in SharePoint related to [system/process]. List:
- Document titles and locations
- Last update dates (if visible)
- Topics covered

I need to check whether our documentation is current.
```

---

### 10. Knowledge Base Article Draft

**Use Case:** Turn a resolved issue into a draft KB article for the service desk, for SME review.

**Target Personas:** Service Desk Lead, Support Engineer, IT Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `knowledge-base`, `documentation`

**Prompt:**

```
From the resolution notes I provide for [issue], draft a knowledge base article:
- Symptom / what the user reports
- Cause (as established)
- Resolution steps (numbered)
- Workaround (if any)

Mark "DRAFT — for SME review." Do not add steps not in the notes; flag gaps as [verify].
```

---

### 11. Runbook / SOP Draft Prep

**Use Case:** Structure an operational procedure into a runbook draft from notes, for technical review.

**Target Personas:** Systems Administrator, SRE, DevOps Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `runbook`, `sop`

**Prompt:**

```
Turn these operational notes into a structured runbook draft: [paste notes].
- Purpose and scope
- Prerequisites
- Numbered procedure (one action per step)
- Verification / rollback
- Escalation contacts

Mark "DRAFT — verify each step in a safe environment before use." Do not invent steps; flag missing detail.
```

---

## Architecture & Planning

### 12. Architecture Decision Research

**Use Case:** Research past architecture discussions. Verify current state with the architecture team.

**Target Personas:** Solutions Architect, IT Manager, Technical Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `architecture`, `experimental`

**Prompt:**

```
Search internal documents and emails for discussions about [technology decision]. Compile:
- Options considered
- Pros/cons discussed
- Decisions made and rationale
- Any revisits or regrets mentioned

EXPERIMENTAL: decisions may have evolved. Verify current state with the architecture team.
```

---

### 13. M365 / Tenant Policy Research

**Use Case:** Find prior decisions on a tenant or M365 admin policy before changing configuration.

**Target Personas:** M365 Administrator, IT Manager, Identity Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `m365-admin`, `policy`

**Prompt:**

```
Search emails and SharePoint for prior decisions and discussions about [policy area, e.g., "conditional access" or "external sharing"]. Summarize:
- What was decided and when
- The rationale and any exceptions
- Who owned the decision

This is research before any configuration review. Confirm current settings in the admin center — Copilot does not read live tenant config.
```

---

## Access & Vendors

### 14. Access Request Context

**Use Case:** Gather the context behind an access request to inform the approver. Approval is a human decision.

**Target Personas:** IT Manager, Identity Engineer, Service Desk Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `access`, `context`

**Prompt:**

```
For the access request from [person/role] for [system], gather context from emails/Teams:
- What access is requested and the stated reason
- Any manager or business approval mentioned
- Prior similar access for the role

Summarize for the approver. This does NOT grant or recommend access — least-privilege approval is a human decision.
```

---

### 15. Vendor Support Summary

**Use Case:** Compile vendor support history to prepare for an escalation.

**Target Personas:** IT Manager, Support Engineer, Vendor Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `vendor`, `support`

**Prompt:**

```
Search emails for correspondence with [vendor] support regarding [issue/product]. Summarize:
- Issues reported
- Vendor responses and recommendations
- Ticket numbers mentioned
- Resolution status

I need this to prepare an escalation.
```

---

## Reporting

### 16. SLA / Service Report Prep

**Use Case:** Gather context for a service or SLA report. Authoritative metrics come from the ITSM/monitoring tools.

**Target Personas:** IT Manager, Service Delivery Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `sla`, `reporting`

**Prompt:**

```
For my [weekly/monthly] service review of [service], gather from emails and Teams:
- Major incidents and their impact
- Changes implemented
- Recurring complaints or praise
- Outstanding actions

Compile as context for my report. Authoritative SLA metrics come from the ITSM and monitoring tools, not this summary.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
