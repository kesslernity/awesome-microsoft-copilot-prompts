# Copilot for Sales & Business Development

> Master Microsoft 365 Copilot for sales and business development roles. Contains [APPROVED] production-safe prompts for Account Executives, BDRs, and Sales Managers with role-specific guardrails.

**Category:** Marketing & Sales

**Total Prompts:** 16

---

[← Back to Main Library](../../README.md)

---

### Account Management

#### 1. [APPROVED] QBR Preparation

**Use Case:** Prepare comprehensive QBR content from client interactions. Add metrics from CRM separately.

**Target Personas:** Account Executive, Customer Success Manager, Account Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `qbr`, `preparation`

**Prompt:**

```
I have a Quarterly Business Review with [Account Name]. Search for:
- All wins and successes we delivered this quarter
- Issues or escalations that occurred
- Feature requests or feedback they provided
- Upcoming initiatives they mentioned
- Expansion or upsell opportunities discussed

Compile as QBR prep notes. I will add metrics from our systems.
```

---

#### 2. [APPROVED] Account Research Summary

**Use Case:** Prepare for client calls with comprehensive account context from all communications.

**Target Personas:** Account Executive, Enterprise AE, Strategic Account Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `account-research`, `preparation`

**Prompt:**

```
You are assisting an account executive. Search my emails, Teams, and SharePoint for all information about [Account Name]. Compile:
- Key stakeholders and their roles
- Recent interactions and meetings
- Open opportunities or deals discussed
- Pain points or challenges mentioned
- Competitive mentions
- Any commitments made by either party

Format as a pre-call briefing document.
```

---

### Coaching

#### 1. [APPROVED] Deal Review Preparation

**Use Case:** Prepare for deal reviews with full context on the opportunity.

**Target Personas:** Sales Manager, Sales Director, VP Sales

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `deal-review`, `coaching`

**Prompt:**

```
I have a deal review for [Rep Name]'s opportunity with [Account Name]. Search for:
- Recent correspondence about this deal
- Concerns or risks mentioned
- Customer feedback or objections
- Internal discussions about strategy
- Resources or support requested

Prepare briefing notes so I can provide effective coaching.
```

---

#### 2. [APPROVED] Rep Performance Context

**Use Case:** Gather context for 1:1 coaching conversations. Use HR systems for formal reviews.

**Target Personas:** Sales Manager, Sales Director, Team Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `coaching`, `one-on-one`

**Prompt:**

```
Search for communications related to [Rep Name]'s activities over the past month. Note:
- Wins and successes mentioned
- Challenges they raised
- Support they requested
- Customer feedback about them
- Coaching moments identified

This is context for our 1:1. Not a substitute for proper performance metrics.
```

---

### Competitive Analysis

#### 1. [APPROVED] Competitive Intelligence Search

**Use Case:** Gather competitive intelligence from past interactions to inform sales strategy.

**Target Personas:** Account Executive, Sales Manager, Solutions Consultant

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `competitive`, `intelligence`

**Prompt:**

```
Search my emails and documents for any mentions of [Competitor Name] in relation to [Account Name] or similar deals. Compile:
- What the prospect said about the competitor
- Features or pricing comparisons mentioned
- Why we won or lost against them previously
- Competitive positioning discussed by our team

This is research for competitive strategy. I will validate with current intel.
```

---

### Escalation Management

#### 1. [APPROVED] Customer Escalation Summary

**Use Case:** Create escalation summaries for leadership briefings.

**Target Personas:** Sales Manager, Account Executive, VP Sales

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `escalation`, `customer`

**Prompt:**

```
Search for all communications about the escalation with [Account Name]. Compile:
- Timeline of events
- Issues raised by the customer
- Actions taken by our team
- Current status
- Resolution proposals discussed

I need this for the executive briefing.
```

---

### Forecasting

#### 1. [APPROVED] Forecast Discussion Summary

**Use Case:** Gather forecast context from team discussions. CRM is source of truth for numbers.

**Target Personas:** Sales Manager, Sales Director, VP Sales

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `forecast`, `pipeline`

**Prompt:**

```
Search my emails and Teams from the past week for forecast-related discussions with my team. Compile:
- Deals reps are committing
- Risks to the forecast mentioned
- Upside opportunities discussed
- Push-outs or slips communicated
- Support needed to close

This is prep for forecast call. Actual numbers come from CRM.
```

---

### Governance

#### 1. ⚠️ Sales Copilot Guardrails

**Use Case:** Essential guardrails for sales professionals using Copilot. Understand CRM vs. Copilot boundaries.

**Target Personas:** Account Executive, BDR, Sales Manager, VP Sales

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `sales`

**Prompt:**

```
## When NOT to Use Copilot for Sales

**ACCOUNT EXECUTIVES — NEVER use Copilot for:**
- Pricing decisions or approvals
- Contract terms negotiation
- Discount authorization
- Legal commitments to customers
- Revenue recognition
- Deal registration in CRM
- Forecast commits (use CRM)
- Commission calculations

**BDRs — NEVER use Copilot for:**
- Adding leads to CRM (do it properly)
- Qualification scoring (use your process)
- Territory assignments
- Lead routing decisions
- Compliance-sensitive outreach
- Do-not-contact list checking

**SALES MANAGERS — NEVER use Copilot for:**
- Performance reviews or ratings
- Compensation decisions
- Hiring/firing decisions
- Quota assignments
- Territory changes
- Pipeline commits to leadership
- Revenue forecasts (use CRM)

**Data Privacy Warnings:**
- Never include customer financial details in prompts
- Be careful with competitive intelligence sources
- Remember that prompts may be logged
- Don't share customer PII in prompts

**Golden Rules:**
- AEs: "Copilot researches — AEs close"
- BDRs: "Copilot discovers — BDRs connect"
- Managers: "Copilot summarizes — managers coach"

**System Integration Note:**
Copilot does NOT integrate with:
- Salesforce / HubSpot / CRM
- Sales engagement platforms
- CPQ systems
- Contract management systems

**CRM is the source of truth for:**
- Pipeline and forecasts
- Customer records
- Activity logging
- Performance metrics
```

---

### Lead Qualification

#### 1. [APPROVED] Lead Qualification Notes

**Use Case:** Organize discovery information into structured qualification notes.

**Target Personas:** BDR, SDR, Inside Sales Rep

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `qualification`, `discovery`

**Prompt:**

```
Based on my call/email notes with [Contact Name] at [Company Name], help me organize the qualification information:
- Budget indicators mentioned
- Authority/decision process discussed
- Need/pain points identified
- Timeline expectations
- Current solutions they use

Format as structured qualification notes for handoff to AE.
```

---

### Outreach

#### 1. [APPROVED] Outreach Sequence Draft

**Use Case:** Draft initial outreach emails that can be personalized before sending.

**Target Personas:** BDR, SDR, Inside Sales Rep

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `outreach`, `email`

**Prompt:**

```
Draft a personalized outreach email to [Contact Name], [Title] at [Company Name]. Based on:
- Their industry: [Industry]
- Likely pain points for their role
- Our value proposition for similar companies

Keep it concise (under 150 words), professional, and include a clear call-to-action. I will personalize further before sending.
```

---

#### 2. [APPROVED] Meeting Request Follow-up

**Use Case:** Create follow-up sequences that add value without being pushy.

**Target Personas:** BDR, SDR, Inside Sales Rep

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `follow-up`, `sequence`

**Prompt:**

```
Draft a follow-up email to [Contact Name] who hasn't responded to my meeting request. Reference:
- My original outreach topic
- A new angle or value point
- Flexible meeting options

Keep it short, respectful of their time, and not pushy. This is attempt [2/3/4] so adjust tone accordingly.
```

---

### Performance Analysis

#### 1. [EXPERIMENTAL] Outreach Pattern Analysis

**Use Case:** Identify patterns in outreach effectiveness. Supplement with sales analytics tools.

**Target Personas:** BDR, SDR, Sales Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `analytics`, `experimental`

**Prompt:**

```
Review my sent emails and responses over the past month. Identify patterns in:
- Subject lines that got responses
- Send times that worked best
- Message lengths that performed
- Value propositions that resonated

This is for improving my outreach strategy.

EXPERIMENTAL: Email analysis may not capture all factors affecting response rates. Use proper sales analytics tools for comprehensive metrics.
```

---

### Pipeline Management

#### 1. [APPROVED] Deal Progress Summary

**Use Case:** Get a complete picture of deal progress from scattered communications before pipeline reviews.

**Target Personas:** Account Executive, Sales Manager, Enterprise AE

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `deal-tracking`, `pipeline`

**Prompt:**

```
Search my emails and Teams for all correspondence related to the [Deal Name/Opportunity] with [Account Name]. Summarize:
- Current deal stage and next steps discussed
- Key decision makers involved
- Objections or concerns raised
- Pricing discussions (without specific numbers)
- Timeline expectations mentioned
- Competitive threats discussed

This is for my pipeline review preparation.
```

---

### Proposal Management

#### 1. [APPROVED] Proposal Follow-up Draft

**Use Case:** Create personalized proposal follow-ups that reference actual conversation points.

**Target Personas:** Account Executive, Solutions Consultant, Sales Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `proposal`, `follow-up`

**Prompt:**

```
Draft a follow-up email to [Contact Name] at [Account Name] regarding the proposal we sent for [Solution/Product]. Based on our previous correspondence:
- Reference specific points they showed interest in
- Address any concerns they raised
- Suggest next steps
- Keep tone professional but warm

Mark areas where I need to add specific details or pricing. I will review before sending.
```

---

### Prospecting

#### 1. [APPROVED] Prospect Research

**Use Case:** Research prospects using internal knowledge before outreach.

**Target Personas:** BDR, SDR, Inside Sales Rep

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `prospecting`, `research`

**Prompt:**

```
You are assisting a business development rep. Search for any information in my emails, Teams, or SharePoint about [Company Name] or [Contact Name]. Find:
- Any previous outreach or responses
- Colleagues who may have connections
- Industry or company news mentioned
- Potential pain points discussed
- Best contact methods that worked

This is for outreach preparation.
```

---

### Team Management

#### 1. [APPROVED] Team Pipeline Summary

**Use Case:** Consolidate team updates from communications before adding CRM metrics.

**Target Personas:** Sales Manager, Sales Director, VP Sales

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `sales`, `pipeline`, `team-management`

**Prompt:**

```
You are assisting a sales manager. Search my emails and Teams for updates from my team about their deals this week. Summarize:
- Deals that progressed or closed
- Deals at risk or stalled
- Support requests from reps
- Blockers mentioned
- Wins to celebrate

Format as a weekly team summary. I will add CRM data for complete picture.
```

---

