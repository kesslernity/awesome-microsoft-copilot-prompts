# Copilot for HSE, Legal & Compliance

> Master Microsoft 365 Copilot for HSE, legal, and IT compliance roles. Contains production-safe prompts for HSE/Quality, Legal/Contracts, and IT/Cloud professionals with strict safety guardrails.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts access your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Security & Compliance

**Prompts:** 20

---

## CRITICAL: HSE CRITICAL GUARDRAILS - READ FIRST

### 1. HSE CRITICAL GUARDRAILS - READ FIRST

**Use Case:** CRITICAL: Read this before any HSE use of Copilot. Print and post in HSE offices and site facilities.

**Target Personas:** HSE Manager, Safety Officer, Quality Manager, Site Manager, Project Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hse`, `safety`, `guardrails`, `critical`

**Prompt:**

```
## CRITICAL: When NEVER to Use Copilot for HSE & Safety

**SAFETY IS NON-NEGOTIABLE. Copilot MUST NEVER be used for:**

### Safety Authorization
- Permit-to-work approval
- LOTO (Lock-Out/Tag-Out) authorization
- Confined space entry approval
- Hot work permits
- Working at height authorization
- Lifting operation approval

### Safety Assessment
- Risk assessments
- JSA (Job Safety Analysis)
- Hazard identification
- Safety case decisions
- Emergency response decisions
- Stop work authority

### Incident Management
- Incident classification
- Investigation conclusions
- Root cause determination
- Corrective action approval
- Near-miss assessment
- Regulatory notification decisions

### Quality & Compliance
- Quality inspection sign-off
- Non-conformance decisions
- Material acceptance
- Test witness approval
- Certificate issuance
- Regulatory submissions

**Golden Rule:**
> "Copilot finds information - HSE professionals protect lives."

**There are NO exceptions. Lives depend on this boundary.**

### What Copilot CAN help with:
- Finding procedures (verify revision!)
- Preparing for HSE meetings
- Searching for incident context
- Drafting communications (for review)

**Remember:** No AI output EVER replaces professional HSE judgment.
```

---

## Legal & IT Copilot Guardrails

### 2. Legal & IT Copilot Guardrails

**Use Case:** Essential guardrails for Legal and IT roles using Copilot. Includes privilege and security warnings.

**Target Personas:** Legal Counsel, Contracts Manager, IT Manager, Systems Administrator, CISO

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `legal`, `it`, `security`

**Prompt:**

```
## When NOT to Use Copilot for Legal & IT

**LEGAL - NEVER use Copilot for:**
- Legal advice or opinions
- Contract interpretation
- Claim entitlement analysis
- Compliance decisions
- Settlement authority
- Litigation strategy
- Contract execution/signing
- Regulatory advice

**Copilot outputs are NEVER legal advice, regardless of how they are worded.**

**Legal Privilege Warning:**
- Be mindful of privilege when prompting
- Attorney-client communications have implications
- Consult your legal team about appropriate Copilot use

---

**IT & CLOUD - NEVER use Copilot for:**
- Production code writing
- Security assessments
- Access control decisions
- Infrastructure changes (use IaC)
- Active incident response
- Vulnerability remediation
- Password/secret handling
- Data handling decisions

**Security Reminder:**
- Never include credentials in prompts
- Remember prompts may be logged
- Follow your organization's AI policy
- Never use Copilot to bypass security controls

---

**Golden Rules:**
- Legal: "Copilot retrieves - legal provides judgment"
- IT: "Copilot researches - IT decides and executes"

**System Integration Note:**
Copilot does NOT integrate with:
- Contract management systems
- Legal research databases
- ServiceNow / ITSM tools
- DevOps platforms
- Security tools
```

---

## Architecture

### 3. Architecture Decision Research

**Use Case:** Research architecture decisions from discussions. Always verify current state with architecture team.

**Target Personas:** Solutions Architect, IT Manager, Technical Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `architecture`, `experimental`

**Prompt:**

```
Search internal documents and emails for discussions about [technology decision, e.g., "container orchestration" or "API gateway selection"]. Compile:
- Options considered
- Pros/cons discussed
- Decisions made and rationale
- Any revisits or regrets mentioned

This is research for architecture documentation.

EXPERIMENTAL: Technical decisions may have evolved. Verify current state with the architecture team.
```

---

## Change Management

### 4. Change Request Preparation

**Use Case:** Research previous change implementations to prepare comprehensive change requests.

**Target Personas:** IT Manager, Change Manager, Systems Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `change-management`, `preparation`

**Prompt:**

```
I'm preparing a change request for [change description]. Search for:
- Similar changes previously implemented
- Any risks or issues that were raised
- Approvals that were required
- Rollback procedures mentioned

Help me prepare a thorough change request by gathering precedents.
```

---

### 5. CAB Meeting Preparation

**Use Case:** Prepare for CAB meetings with context on pending changes and concerns.

**Target Personas:** IT Manager, Change Manager, CAB Member

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `cab`, `change-management`

**Prompt:**

```
I have a Change Advisory Board meeting. Based on recent emails and Teams:
- What changes are pending approval?
- What concerns have been raised about upcoming changes?
- Any failed changes being discussed?
- Risk assessments mentioned?

Prepare briefing notes for my preparation.
```

---

## Claims Management

### 6. Claim Timeline Summary

**Use Case:** Organize claim timeline from correspondence. Legal analysis requires qualified legal review.

**Target Personas:** Claims Manager, Legal Counsel, Commercial Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `claims`, `timeline`

**Prompt:**

```
Search emails and documents related to [Claim Reference] and compile a chronological summary:
- When the claim was first notified
- Key communications and their dates
- Responses received
- Current status discussed

This is for case file organization - requires legal review for formal use.
```

---

## Contract Negotiation

### 7. Negotiation History Research

**Use Case:** Research contract negotiation history for preparation. Legal analysis requires qualified legal review.

**Target Personas:** Contracts Manager, Legal Counsel, Commercial Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `contracts`, `negotiation`

**Prompt:**

```
You are assisting a contracts professional. Search my emails for the negotiation history of [Contract Reference/Name]. Compile:
- Key issues raised by each party
- Positions and counter-positions
- Compromises reached
- Outstanding items at last discussion

This is research for my preparation - not legal analysis.
```

---

## Contract Standards

### 8. Contract Pattern Research

**Use Case:** Research contract patterns across deals. Legal applicability requires formal legal review.

**Target Personas:** Legal Counsel, Contracts Manager, General Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `patterns`, `experimental`

**Prompt:**

```
Search our contracts database in SharePoint for patterns in how [clause type] is handled across different client types or jurisdictions. Note:
- Variations observed
- Common language patterns
- Any issues flagged in reviews

This is research for internal guidance - requires legal validation.

EXPERIMENTAL: Contract patterns may have contextual reasons not visible in summaries. Always consult legal.
```

---

## Dispute Resolution

### 9. Dispute Preparation

**Use Case:** Prepare for dispute meetings with context from correspondence. Legal strategy requires legal counsel.

**Target Personas:** Legal Counsel, Contracts Manager, Commercial Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `disputes`, `preparation`

**Prompt:**

```
We have a meeting about the dispute with [Party Name]. Based on correspondence:
- What are the main points of contention?
- What evidence has been referenced?
- What positions have each party taken?
- Any settlement discussions?

Prepare briefing notes for my preparation. This is not legal strategy advice.
```

---

## Environmental Compliance

### 10. Environmental Compliance Research

**Use Case:** Research environmental compliance discussions. Actual compliance activities use formal environmental systems.

**Target Personas:** Environmental Manager, HSE Manager, Sustainability Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `environmental`, `compliance`, `research`

**Prompt:**

```
Search for emails discussing environmental compliance for [Project/Site]. Identify:
- Permit requirements mentioned
- Monitoring obligations discussed
- Compliance concerns raised
- Regulatory correspondence referenced

This is research for planning. Actual compliance is managed through formal systems.
```

---

## HSE Analytics

### 11. HSE Trend Identification

**Use Case:** Explore HSE themes from communications. Formal trend analysis must use HSE incident systems.

**Target Personas:** HSE Manager, Safety Analyst, HSE Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hse`, `trends`, `experimental`

**Prompt:**

```
Review HSE-related correspondence for [Project/Site] over the past 3 months. Identify patterns in:
- Types of concerns raised
- Locations or activities frequently mentioned
- Recurring themes

This is EXPLORATORY ONLY for discussion. Formal trend analysis must use HSE data systems.

EXPERIMENTAL: Email analysis cannot replace proper safety data analysis. May miss unreported incidents or observations.
```

---

## HSE Procedures

### 12. HSE Procedure Search

**Use Case:** Quickly locate HSE procedures. ALWAYS verify revision status with Document Control before field use.

**Target Personas:** HSE Manager, Safety Officer, HSE Advisor

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hse`, `safety`, `procedures`

**Prompt:**

```
You are assisting an HSE professional. Search SharePoint for HSE procedures related to [topic, e.g., "confined space entry" or "hot work permit"]. List:
- Procedure documents found
- Effective dates or revision status (if visible)
- Key requirements summarized

I need this to answer a site inquiry. I will verify current approved revision with Document Control.
```

---

## HSE Review

### 13. HSE Meeting Preparation

**Use Case:** Prepare for HSE meetings with context from communications. Formal HSE metrics come from HSE systems.

**Target Personas:** HSE Manager, Safety Manager, Project HSE Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hse`, `meeting-prep`, `safety`

**Prompt:**

```
I have an HSE review meeting for [Project/Site Name] tomorrow. Based on recent correspondence:
- What safety concerns have been raised?
- Any near-misses or observations discussed?
- What inspections or audits are mentioned?
- Actions pending closure?

Prepare briefing notes for my review. This does NOT replace formal HSE reporting.
```

---

## IT Documentation

### 14. Technical Documentation Search

**Use Case:** Locate technical documentation and assess currency. Always verify documentation is current before use.

**Target Personas:** IT Manager, Systems Administrator, DevOps Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `documentation`, `runbooks`

**Prompt:**

```
Find runbooks, SOPs, or technical documentation in SharePoint related to [system/process]. List:
- Document titles and locations
- Last update dates (if visible)
- Topics covered

I need to check if our documentation is current.
```

---

## IT Incident Management

### 15. Incident History Search

**Use Case:** Research previous incident resolutions to inform current troubleshooting.

**Target Personas:** IT Manager, Systems Administrator, Support Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `incidents`, `troubleshooting`

**Prompt:**

```
You are assisting an IT professional. Search my emails and Teams for previous incidents related to [system/application name] or [error type]. Compile:
- Incident descriptions
- Root causes identified
- Resolutions applied
- Any workarounds documented

This is research for troubleshooting - I will verify applicability to current issue.
```

---

## Incident Research

### 16. Incident Context Research

**Use Case:** Gather context on incident discussions. Formal incident data and investigation must use official HSE systems.

**Target Personas:** HSE Manager, Incident Investigator, Safety Officer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hse`, `incidents`, `research`

**Prompt:**

```
Search for emails and Teams discussions related to safety incidents or near-misses for [type or location] over the past [timeframe]. Compile:
- Incidents mentioned
- Initial causes discussed
- Actions taken
- Lessons mentioned

This is RESEARCH ONLY for context. Formal incident data comes from the HSE incident system.
```

---

## Legal Research

### 17. Precedent Search

**Use Case:** Find contract precedents for reference. Legal applicability requires qualified legal assessment.

**Target Personas:** Legal Counsel, Contracts Manager, Paralegal

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `precedents`, `research`

**Prompt:**

```
Find previous contracts, agreements, or legal opinions in SharePoint related to [issue type, e.g., "limitation of liability" or "force majeure"]. List:
- Document titles and references
- Context (type of deal, party type)
- Outcomes mentioned

I need precedents for reference - applicability requires legal assessment.
```

---

## Quality Audit

### 18. Quality Audit Preparation

**Use Case:** Prepare for quality audits with context from communications. Formal quality data comes from QMS.

**Target Personas:** Quality Manager, QA Lead, Audit Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `quality`, `audit`, `preparation`

**Prompt:**

```
I have a quality audit for [Project/System]. Search for:
- Previous audit findings mentioned in emails
- Corrective actions discussed
- Non-conformance reports referenced
- Quality concerns raised by the team

Compile as context for my audit preparation. Formal NCR data comes from the QMS.
```

---

## Regulatory Compliance

### 19. Compliance Correspondence Review

**Use Case:** Research compliance discussions. Compliance determinations require formal compliance review.

**Target Personas:** Compliance Manager, Legal Counsel, Regulatory Affairs

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `compliance`, `research`

**Prompt:**

```
Search for emails related to [regulation/compliance topic] discussions. Summarize:
- Requirements discussed
- Actions taken or proposed
- Concerns raised
- Any regulatory correspondence mentioned

This is research for compliance review - does not constitute compliance advice.
```

---

## Vendor Management

### 20. Vendor Support Summary

**Use Case:** Compile vendor support history to prepare for escalations.

**Target Personas:** IT Manager, Support Engineer, Vendor Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `it`, `vendor`, `support`

**Prompt:**

```
Search my emails for correspondence with [vendor name] support regarding [issue/product]. Summarize:
- Issues reported
- Vendor responses and recommendations
- Ticket numbers mentioned
- Resolution status

I need this for escalation preparation.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1300+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
