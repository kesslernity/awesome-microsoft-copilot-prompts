# Copilot for Commercial Operations

> Master Microsoft 365 Copilot for commercial and operations roles. Contains production-safe prompts for Procurement, Document Control, and Planning/Scheduling professionals with role-specific guardrails.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts access your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Operations & Support

**Prompts:** 18

---

## Commercial Operations Copilot Guardrails

> Essential guardrails for commercial and operations roles using Copilot. Understand system boundaries and human accountability.

**Target Personas:** Procurement Manager, Document Controller, Planner, Scheduler

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `operations`

### When NOT to Use Copilot for Commercial & Operations Roles

**PROCUREMENT - NEVER use Copilot for:**
- Vendor selection decisions
- Price approval
- Contract award
- PO generation
- Supplier qualification
- Commercial negotiations
- Claim decisions
- Commitments to vendors

**DOCUMENT CONTROL - NEVER use Copilot for:**
- Document registration/numbering
- Version control
- Transmittal generation
- Approval workflows
- Archive classification
- Distribution control
- Audit evidence
- Compliance certification

**PLANNING & SCHEDULING - NEVER use Copilot for:**
- Schedule creation (use P6/MSP)
- Critical path analysis
- Resource leveling
- Float calculations
- Earned value metrics
- Schedule risk analysis
- Baseline approval
- Schedule certification

### Golden Rules
- **Procurement:** "Copilot researches - procurement decides"
- **Document Control:** "Copilot finds context - DC maintains the record"
- **Planning:** "Copilot narrates - planners calculate"

### What Copilot IS Good For
- Searching correspondence
- Preparing for meetings
- Drafting narratives (not numbers)
- Finding historical context
- Tracking informal discussions

### System Integration Note
Copilot does NOT integrate with:
- SAP/Oracle ERP
- EDMS systems (Aconex, Procore, etc.)
- Primavera P6 / MS Project
- Contract management systems

**Always use official systems for formal records.**

---

## Baseline Management

### 1. Baseline History Search

**Use Case:** Reconstruct baseline change history from communications. Always verify against scheduling software.

**Target Personas:** Planner, Scheduler, Project Controls Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `planning`, `baseline`, `history`

**Prompt:**
```
Find references in emails and SharePoint to schedule baseline changes on [Project Name]. List:
- When baselines were discussed
- Reasons for rebaseline mentioned
- Approvals or rejections noted

I need this to reconstruct baseline history. Will verify against P6 baselines.
```

---

## Bid Management

### 2. Bid Clarification Draft

**Use Case:** Quickly draft bid clarification requests while maintaining professional procurement communication standards.

**Target Personas:** Procurement Manager, Buyer, Contracts Specialist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `procurement`, `bid`, `clarification`

**Prompt:**
```
Draft a professional email to [Vendor Name] requesting clarification on their bid for [RFQ Reference]. Based on my notes and previous correspondence, address these points:
- [List specific clarification points]

Keep tone professional and neutral. I will review and add specific technical questions before sending.
```

---

## Contract Management

### 3. Contract History Search

**Use Case:** Gather comprehensive contract history before renewal negotiations.

**Target Personas:** Procurement Manager, Contracts Manager, Category Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `procurement`, `contract`, `renewal`

**Prompt:**
```
Search for emails and documents related to our contract with [Vendor Name] including:
- Original contract discussions
- Any amendments or change orders
- Performance issues mentioned
- Claims or disputes

I need this to prepare for contract renewal discussions.
```

---

## Delay Analysis

### 4. Delay Analysis Research

**Use Case:** Gather delay discussion history to support formal delay analysis documentation.

**Target Personas:** Planner, Claims Analyst, Project Controls

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `planning`, `delay`, `analysis`

**Prompt:**
```
Search project correspondence for discussions about delays to [milestone/activity]. Compile:
- When the delay was first reported
- Causes mentioned by different parties
- Recovery proposals discussed
- Any schedule impact assessments referenced

This is research for delay analysis documentation - requires formal analysis.
```

---

## Distribution Control

### 5. Distribution List Verification

**Use Case:** Verify document distribution from email records. Always reconcile with formal distribution records.

**Target Personas:** Document Controller, Records Manager, Project Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `document-control`, `distribution`, `verification`

**Prompt:**
```
Search for emails where [Document Number or Type] was distributed or transmitted. List:
- Recipients included
- Dates sent
- Any bounce-backs or errors mentioned
- Acknowledgment receipts discussed

I need to verify against our distribution matrix.
```

---

## Document Management

### 6. Transmittal Status Search

**Use Case:** Track transmittal discussions across email threads. Always verify against EDMS for official status.

**Target Personas:** Document Controller, Technical Assistant, Project Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `document-control`, `transmittal`, `tracking`

**Prompt:**
```
You are assisting a document controller. Search my emails for correspondence about transmittal [Transmittal Number/Reference] including:
- Client comments or responses
- Internal review comments
- Status updates
- Any rejections or resubmission requests

Summarize the history for my records.
```

---

### 7. Outstanding Documents Follow-up

**Use Case:** Identify overdue documents and their causes from email discussions. Use to drive document status meetings.

**Target Personas:** Document Controller, Project Administrator, Engineering Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `document-control`, `overdue`, `follow-up`

**Prompt:**
```
Search my emails from the past 2 weeks for discussions about overdue documents or late deliverables for [Project Name]. List:
- Documents mentioned as late
- Reasons given for delays
- Commitments made for delivery dates
- Who is responsible (as mentioned)

I need this to prepare for the document status meeting.
```

---

## Knowledge Management

### 8. Schedule Lessons Learned

**Use Case:** Identify schedule-related lessons from project communications for close-out. Requires team validation.

**Target Personas:** Planner, Project Controls Manager, PMO

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `planning`, `lessons-learned`, `experimental`

**Prompt:**
```
Review project emails for [Project Name] and identify recurring themes related to schedule performance:
- What caused delays repeatedly?
- What worked well for recovery?
- Any recommendations mentioned?

Compile as input for project close-out. Requires validation with project team.

EXPERIMENTAL: May miss context or misinterpret technical schedule discussions. Always validate with the planning team.
```

---

## Market Intelligence

### 9. Market Intelligence Summary

**Use Case:** Gather internal market observations to supplement external intelligence. Always verify with current market data.

**Target Personas:** Procurement Manager, Category Manager, Strategic Sourcing

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `procurement`, `market`, `experimental`

**Prompt:**
```
Search our internal emails and documents for any references to [commodity type] pricing, availability, or market conditions over the past 6 months. Summarize what our team has observed or discussed.

Note: This is internal intelligence only - verify with current market data.

EXPERIMENTAL: Internal discussions may be dated or incomplete. Always verify with current market intelligence sources.
```

---

## Meeting Preparation

### 10. Progress Meeting Preparation

**Use Case:** Prepare for schedule review meetings with context from team communications. Always correlate with P6/MSP data.

**Target Personas:** Planner, Scheduler, Project Controls Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `planning`, `meeting-prep`, `schedule-review`

**Prompt:**
```
I have a weekly schedule review meeting for [Project Name]. Summarize from my emails and Teams:
- Schedule concerns raised by discipline leads
- Change requests or scope changes that may impact schedule
- Resource constraints mentioned
- Any float consumption warnings

Format as prep notes. I will correlate with current P6 status.
```

---

## Process Improvement

### 11. Document Issue Pattern Analysis

**Use Case:** Identify patterns in document issues for process improvement. Requires validation with formal tracking data.

**Target Personas:** Document Controller, Quality Manager, Process Improvement Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `document-control`, `patterns`, `experimental`

**Prompt:**
```
Review my emails from the past 3 months related to document control issues (rejections, late deliveries, comment disputes). Identify:
- Recurring problems
- Disciplines or vendors frequently mentioned
- Common causes discussed

This is input for process improvement - requires validation with the team.

EXPERIMENTAL: May not capture the full picture of document issues. Use proper tracking systems for comprehensive analysis.
```

---

## Records Management

### 12. Archive Retrieval Research

**Use Case:** Plan archive retrievals by finding references to archive locations and access procedures.

**Target Personas:** Document Controller, Records Manager, Archivist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `document-control`, `archive`, `retrieval`

**Prompt:**
```
We need to retrieve historical documents from [Project Name - old project]. Search my emails and SharePoint for:
- References to where these documents are archived
- Any previous retrieval requests
- Contact persons mentioned for archive access
- Known issues with accessing old records

This is research to plan the retrieval.
```

---

## Review Management

### 13. Comment Resolution Research

**Use Case:** Track comment resolution progress from email discussions. Always reconcile with formal comment registers.

**Target Personas:** Document Controller, Technical Editor, Project Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `document-control`, `comments`, `review`

**Prompt:**
```
Find email discussions about review comments on [Document Number/Title]. Summarize:
- Comments that were raised
- Proposed resolutions discussed
- Agreement status
- Any outstanding disputes

This is for my comment tracking - will verify against formal comment sheets.
```

---

## Schedule Reporting

### 14. Schedule Narrative Draft

**Use Case:** Draft schedule report narrative from communications. Always verify against scheduling software for actual metrics.

**Target Personas:** Planner, Scheduler, Project Controls

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `planning`, `schedule`, `narrative`

**Prompt:**
```
You are assisting a project planner. Based on recent emails and Teams messages about [Project Name] schedule, draft a schedule performance narrative covering:
- Key milestones achieved or missed (as mentioned in correspondence)
- Main causes of variance discussed
- Recovery actions mentioned
- Upcoming critical milestones

This is draft content for the monthly report. I will verify against actual P6 data and add metrics.
```

---

## Sourcing

### 15. RFQ History Research

**Use Case:** Inform sourcing decisions with historical procurement data and lessons learned.

**Target Personas:** Procurement Manager, Strategic Sourcing, Category Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `procurement`, `rfq`, `history`

**Prompt:**
```
Find references to [Equipment/Service Type] procurement in my emails and SharePoint from the past 2 years. List:
- Previous RFQs issued for similar items
- Vendors who were invited or responded
- Any lessons learned or issues mentioned

I need this to inform the current sourcing strategy.
```

---

## Vendor Management

### 16. Supplier Meeting Prep

**Use Case:** Enter supplier meetings fully prepared with context on all open issues and recent commitments.

**Target Personas:** Procurement Manager, Buyer, Supplier Quality Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `procurement`, `vendor-meeting`, `preparation`

**Prompt:**
```
I have a meeting with [Vendor Name] about [Contract/PO Reference]. Based on recent correspondence:
- What are the outstanding issues?
- Any delivery delays or quality concerns discussed?
- What commitments have they made recently?
- What do I need to follow up on?

Prepare briefing notes for my preparation.
```

---

### 17. Vendor Correspondence Summary

**Use Case:** Prepare for vendor meetings with complete context on all discussions and commitments made.

**Target Personas:** Procurement Manager, Buyer, Supply Chain Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `procurement`, `vendor`, `correspondence`

**Prompt:**
```
You are assisting a procurement professional. Search my emails and Teams for all correspondence with [Vendor Name] regarding [PO/RFQ Reference or scope]. Summarize:
- Key discussion points and queries
- Commitments or promises made (by either party)
- Issues or complaints raised
- Current status of discussions

This is for my records and meeting preparation.
```

---

## Governance

### 18. Commercial Operations Copilot Guardrails

**Use Case:** Essential guardrails for commercial and operations roles using Copilot. Understand system boundaries and human accountability.

**Target Personas:** Procurement Manager, Document Controller, Planner, Scheduler

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `operations`

**Prompt:**
```
## When NOT to Use Copilot for Commercial & Operations Roles

**PROCUREMENT - NEVER use Copilot for:**
- Vendor selection decisions
- Price approval
- Contract award
- PO generation
- Supplier qualification
- Commercial negotiations
- Claim decisions
- Commitments to vendors

**DOCUMENT CONTROL - NEVER use Copilot for:**
- Document registration/numbering
- Version control
- Transmittal generation
- Approval workflows
- Archive classification
- Distribution control
- Audit evidence
- Compliance certification

**PLANNING & SCHEDULING - NEVER use Copilot for:**
- Schedule creation (use P6/MSP)
- Critical path analysis
- Resource leveling
- Float calculations
- Earned value metrics
- Schedule risk analysis
- Baseline approval
- Schedule certification

**Golden Rules:**
- Procurement: "Copilot researches - procurement decides"
- Document Control: "Copilot finds context - DC maintains the record"
- Planning: "Copilot narrates - planners calculate"

**What Copilot IS good for:**
- Searching correspondence
- Preparing for meetings
- Drafting narratives (not numbers)
- Finding historical context
- Tracking informal discussions

**System Integration Note:**
Copilot does NOT integrate with:
- SAP/Oracle ERP
- EDMS systems (Aconex, Procore, etc.)
- Primavera P6 / MS Project
- Contract management systems

Always use official systems for formal records.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1300+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
