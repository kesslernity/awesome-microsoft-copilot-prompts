# Copilot for Consulting & Professional Services

> Master Microsoft 365 Copilot for consulting and professional services roles. Contains [APPROVED] production-safe prompts for Consultants, Advisors, and Delivery Leads with role-specific guardrails.

**Category:** Leadership & Management

**Total Prompts:** 16

---

[← Back to Main Library](../../README.md)

---

### Advisory Services

#### 1. [APPROVED] Advisory Relationship Summary

**Use Case:** Maintain advisory relationship context across interactions.

**Target Personas:** Senior Advisor, Executive Advisor, Board Advisor

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `advisory`, `relationship`

**Prompt:**

```
You are assisting a senior advisor. Summarize my advisory relationship with [Client/Executive]. Include:
- Topics we've discussed
- Advice provided
- Outcomes of previous guidance
- Current challenges they're facing
- Relationship dynamics
- Next steps committed

This is for relationship continuity.
```

---

### Board Advisory

#### 1. [APPROVED] Board Preparation Research

**Use Case:** Prepare for board-level advisory presentations.

**Target Personas:** Senior Advisor, Board Advisor, Managing Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `board`, `preparation`

**Prompt:**

```
I'm preparing for a board presentation at [Company]. Search for:
- Board composition and backgrounds
- Topics they typically focus on
- Previous presentations to this board
- Questions they've raised before
- Governance concerns
- Strategic priorities discussed

Compile as board prep briefing.
```

---

### Business Development

#### 1. [APPROVED] Proposal Research

**Use Case:** Gather proposal inputs from previous similar engagements.

**Target Personas:** Management Consultant, Principal, Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `proposal`, `research`

**Prompt:**

```
We're developing a proposal for [Client Name] for [Service/Project]. Search for:
- Similar proposals we've created
- Relevant case studies
- Pricing approaches used
- Team configurations for similar work
- Client-specific requirements mentioned
- Competitive landscape discussed

Compile as proposal development input.
```

---

### Client Management

#### 1. [APPROVED] Client Context Brief

**Use Case:** Prepare comprehensive client briefs for consulting engagements.

**Target Personas:** Management Consultant, Strategy Consultant, Senior Advisor

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `client`, `briefing`

**Prompt:**

```
You are assisting a consultant. I have a meeting with [Client Name] about [Topic]. Search for:
- Previous engagement history
- Key stakeholders and relationships
- Challenges we've helped them with
- Recommendations we've made
- Open items or follow-ups
- Industry context discussed

Compile as a client briefing document.
```

---

### Deliverable Development

#### 1. [APPROVED] Deliverable Draft Outline

**Use Case:** Create deliverable outlines based on proven templates.

**Target Personas:** Management Consultant, Senior Consultant, Engagement Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `deliverable`, `outline`

**Prompt:**

```
I'm creating a [deliverable type - e.g., strategy document, assessment report] for [Client Name]. Search for:
- Similar deliverables we've created
- Templates and structures used
- Best practices mentioned
- Client preferences noted
- Feedback on past deliverables

Draft an outline based on our proven approaches. I will customize for this engagement.
```

---

### Engagement Closure

#### 1. [APPROVED] Engagement Close-Out Prep

**Use Case:** Prepare engagement close-out documentation.

**Target Personas:** Delivery Lead, Engagement Manager, Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `closeout`, `lessons`

**Prompt:**

```
We're closing engagement with [Client Name]. Search for:
- Deliverables completed
- Outstanding items
- Lessons learned mentioned
- Client feedback received
- Follow-on opportunities discussed
- Reference-ability discussed
- Knowledge assets to capture

Compile as close-out checklist.
```

---

### Engagement Management

#### 1. [APPROVED] Engagement Status Summary

**Use Case:** Create engagement status summaries from team communications.

**Target Personas:** Delivery Lead, Engagement Manager, Project Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `delivery`, `status`

**Prompt:**

```
You are assisting a delivery lead. Summarize the status of [Engagement/Project Name] based on recent communications:
- Work completed vs. planned
- Issues or blockers raised
- Client feedback received
- Team concerns mentioned
- Risks identified
- Upcoming milestones

Format as engagement status report. I will add metrics from project tools.
```

---

### Escalation Management

#### 1. [APPROVED] Client Escalation Summary

**Use Case:** Prepare escalation summaries for leadership.

**Target Personas:** Delivery Lead, Engagement Manager, Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `escalation`, `client`

**Prompt:**

```
Search for all communications about the issue with [Client Name] regarding [Topic]. Compile:
- Issue timeline
- Client concerns expressed
- Actions taken
- Internal discussions
- Resolution proposals
- Current status

I need this for partner briefing.
```

---

### Executive Communication

#### 1. [APPROVED] Executive Communication Draft

**Use Case:** Draft executive-level advisory communications.

**Target Personas:** Senior Advisor, Partner, Managing Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `executive`, `communication`

**Prompt:**

```
Draft a communication to [Client Executive] about [Topic]. Based on:
- Our relationship history
- Their communication preferences
- Previous discussions on this topic
- Appropriate level of formality
- Key points to convey

Keep tone advisory and strategic. I will personalize before sending.
```

---

### Facilitation

#### 1. [APPROVED] Workshop Preparation

**Use Case:** Prepare for client workshops with proven formats and content.

**Target Personas:** Management Consultant, Workshop Facilitator, Change Consultant

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `workshop`, `facilitation`

**Prompt:**

```
I'm facilitating a workshop on [Topic] with [Client Name]. Search for:
- Workshop formats we've used successfully
- Materials and exercises from similar sessions
- Client-specific context and preferences
- Outcomes they're looking for
- Attendee backgrounds
- Logistics discussed

Compile as workshop prep package.
```

---

### Governance

#### 1. ⚠️ Consulting & Professional Services Copilot Guardrails

**Use Case:** Essential guardrails for consulting professionals using Copilot. Emphasizes confidentiality.

**Target Personas:** Management Consultant, Senior Advisor, Delivery Lead, Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `consulting`, `professional-services`

**Prompt:**

```
## When NOT to Use Copilot for Consulting

**CONSULTANTS — NEVER use Copilot for:**
- Client recommendations (requires judgment)
- Pricing decisions
- Contract negotiations
- Final deliverable content (requires review)
- Competitive intelligence from external sources
- Client confidential data analysis
- Investment advice (requires licensing)
- Legal or regulatory guidance

**ADVISORS — NEVER use Copilot for:**
- Strategic recommendations (requires expertise)
- Board-level advice (personal accountability)
- M&A guidance (confidentiality critical)
- Executive coaching (relationship-based)
- Crisis advisory (real-time judgment)
- Investment opinions (regulatory requirements)
- Legal opinions (requires qualification)

**DELIVERY LEADS — NEVER use Copilot for:**
- Budget approvals (use finance systems)
- Resource allocation decisions
- Contract change orders (requires approval)
- Client commitments
- Timeline guarantees
- Risk sign-offs
- Quality certifications
- Invoice approvals

**Client Confidentiality Warnings:**
- CRITICAL: Never mix client information across engagements
- Never include client proprietary data in prompts
- Be extremely careful with competitive situations
- Chinese wall principles apply
- Remember prompts may be logged
- Follow your firm's confidentiality policies
- Client names in prompts create confidentiality risk

**Golden Rules:**
- Consultants: "Copilot prepares — consultants advise"
- Advisors: "Copilot informs — advisors guide"
- Delivery Leads: "Copilot tracks — delivery leads execute"

**Professional Standards:**
- All client communications require human review
- Recommendations require professional judgment
- Independence and objectivity must be maintained
- Follow professional body ethical requirements
```

---

### Knowledge Management

#### 1. [APPROVED] Knowledge Asset Search

**Use Case:** Find relevant knowledge assets for consulting engagements.

**Target Personas:** Management Consultant, Senior Consultant, Knowledge Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `knowledge`, `assets`

**Prompt:**

```
Search for knowledge assets related to [Topic/Industry/Capability]. Find:
- Frameworks we've developed
- Methodologies documented
- Case studies available
- Subject matter experts
- Recent project learnings
- Reusable templates

Compile as knowledge inventory for current engagement.
```

---

### Practice Development

#### 1. [EXPERIMENTAL] Advisory Practice Insights

**Use Case:** Identify practice insights from advisory work. Respect confidentiality.

**Target Personas:** Senior Advisor, Practice Lead, Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `practice`, `experimental`

**Prompt:**

```
Review advisory interactions across my client portfolio over the past quarter. Identify:
- Common challenges clients face
- Advice that resonated
- Emerging themes
- Capability gaps to address
- Cross-client opportunities

This is for practice development planning.

EXPERIMENTAL: May miss confidential client-specific insights. Respect client confidentiality boundaries.
```

---

### Scope Management

#### 1. [APPROVED] SOW/Scope Discussion Summary

**Use Case:** Track scope discussions for engagement management.

**Target Personas:** Delivery Lead, Engagement Manager, Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `scope`, `sow`

**Prompt:**

```
Search for discussions about scope for [Engagement Name]. Compile:
- Original scope agreed
- Change requests discussed
- Scope creep concerns
- Client expectations vs. contract
- Out-of-scope items mentioned
- Approval discussions

This is for scope management and potential change order.
```

---

### Team Management

#### 1. [APPROVED] Team Coordination Summary

**Use Case:** Coordinate consulting team from communications.

**Target Personas:** Delivery Lead, Engagement Manager, Team Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `team`, `coordination`

**Prompt:**

```
Summarize team coordination for [Engagement Name]:
- Team member updates and status
- Resource constraints mentioned
- Collaboration issues raised
- Skill gaps identified
- Workload concerns
- Support needs

This is for team standup preparation.
```

---

### Thought Leadership

#### 1. [APPROVED] Industry Trends Research

**Use Case:** Synthesize industry observations from client interactions.

**Target Personas:** Senior Advisor, Industry Expert, Practice Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `consulting`, `trends`, `industry`

**Prompt:**

```
Search for discussions about trends in [Industry/Sector]. Compile:
- Trends we've observed with clients
- Market changes mentioned
- Technology impacts discussed
- Regulatory developments noted
- Competitive dynamics
- Client concerns and opportunities

This is for thought leadership development.
```

---

