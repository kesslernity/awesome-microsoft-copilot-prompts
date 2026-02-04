# Copilot for Customer Success & Support

> Master Microsoft 365 Copilot for customer success and support roles. Contains [APPROVED] production-safe prompts for CSMs, Support Leads, and Account Managers with role-specific guardrails.

**Category:** Operations & Support

**Total Prompts:** 16

---

[← Back to Main Library](../../README.md)

---

### Account Health

#### 1. [APPROVED] Customer Health Summary

**Use Case:** Gather qualitative account context from communications. Use CS platform for health metrics.

**Target Personas:** Customer Success Manager, Account Manager, Client Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `customer-success`, `account-health`, `review`

**Prompt:**

```
You are assisting a customer success manager. Search my emails and Teams for all recent interactions with [Customer Name]. Summarize:
- Recent conversations and their tone
- Issues or concerns raised
- Feature requests or feedback
- Usage or adoption discussions
- Upcoming renewal mentions
- Escalations or risks identified

This is for my account review. Health scores come from our CS platform.
```

---

### Account Planning

#### 1. [APPROVED] Relationship Mapping

**Use Case:** Map account relationships from communication patterns.

**Target Personas:** Account Manager, Customer Success Manager, Strategic Account Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `account-management`, `relationship`, `mapping`

**Prompt:**

```
You are assisting an account manager. Search for all contacts and interactions with [Account Name]. Create a relationship map showing:
- Key contacts and their roles
- Interaction frequency
- Topics they engage on
- Champions vs. detractors (based on tone)
- Organizational changes mentioned
- Reporting relationships discussed

This is for account planning.
```

---

### Account Transitions

#### 1. [APPROVED] Handoff Documentation

**Use Case:** Create account handoff documentation from relationship history.

**Target Personas:** Account Manager, Customer Success Manager, Client Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `account-management`, `handoff`, `transition`

**Prompt:**

```
I am transitioning [Account Name] to a new account manager. Compile a handoff document including:
- Key contacts and relationship status
- Ongoing initiatives
- Open issues or concerns
- Upcoming milestones (renewals, QBRs)
- Historical context (wins, challenges)
- My recommendations

Format as comprehensive handoff brief.
```

---

### Business Reviews

#### 1. [APPROVED] QBR Preparation

**Use Case:** Prepare QBR content from relationship context. Add platform metrics separately.

**Target Personas:** Customer Success Manager, Account Manager, Customer Success Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `customer-success`, `qbr`, `preparation`

**Prompt:**

```
I have a Quarterly Business Review with [Customer Name]. Search for:
- Value delivered this quarter (mentions of success, ROI, wins)
- Challenges or issues that occurred
- Support tickets discussed
- Product feedback provided
- Goals for next quarter mentioned
- Expansion or upsell conversations

Compile as QBR prep notes. I will add usage data from our systems.
```

---

### Contract Management

#### 1. [APPROVED] Contract Discussion Summary

**Use Case:** Gather contract negotiation context. Legal review required for actual terms.

**Target Personas:** Account Manager, Customer Success Manager, Commercial Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `account-management`, `contract`, `negotiation`

**Prompt:**

```
Search for discussions about contract terms with [Account Name]. Summarize:
- Terms being negotiated
- Concerns raised by either party
- Pricing discussions
- SLA discussions
- Legal points raised
- Timeline pressures mentioned

This is background for contract negotiation. Actual terms require legal review.
```

---

### Customer Communication

#### 1. [APPROVED] Customer Communication Draft

**Use Case:** Draft customer support communications for review.

**Target Personas:** Support Lead, Support Specialist, Technical Support Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `support`, `communication`, `customer`

**Prompt:**

```
Draft an update email to [Customer Name] about their support case [Case Reference]. Include:
- Acknowledgment of the issue
- Current status
- Next steps being taken
- Expected resolution timeline
- Apology if appropriate

Keep tone professional and empathetic. I will review before sending.
```

---

### Escalation Management

#### 1. [APPROVED] Escalation Context Summary

**Use Case:** Gather escalation context from communications for resolution meetings.

**Target Personas:** Support Lead, Support Manager, Technical Support Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `support`, `escalation`, `context`

**Prompt:**

```
You are assisting a support lead. Search for all communications about the escalation from [Customer Name] regarding [Issue]. Compile:
- Timeline of the issue
- Troubleshooting steps discussed
- Customer impact mentioned
- Internal discussions and decisions
- Current status
- Committed resolution timeline

I need this for the escalation review meeting.
```

---

### Expansion

#### 1. [APPROVED] Expansion Opportunity Research

**Use Case:** Identify expansion signals from customer communications.

**Target Personas:** Customer Success Manager, Account Manager, Account Executive

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `customer-success`, `expansion`, `upsell`

**Prompt:**

```
Search for signals of expansion opportunity with [Customer Name]:
- New use cases mentioned
- Additional departments discussed
- Pain points that our other products solve
- Budget cycle mentions
- Growth indicators
- Champion referrals to other teams

Compile as expansion opportunity brief.
```

---

### Governance

#### 1. ⚠️ Customer Success & Support Copilot Guardrails

**Use Case:** Essential guardrails for customer success and support professionals using Copilot.

**Target Personas:** Customer Success Manager, Support Lead, Account Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `customer-success`, `support`

**Prompt:**

```
## When NOT to Use Copilot for Customer Success & Support

**CSMs — NEVER use Copilot for:**
- Health score calculations (use CS platform)
- Renewal forecasting (use CRM)
- Churn risk scoring (use predictive tools)
- Contract decisions
- Pricing approvals
- SLA commitments
- NPS/CSAT analysis (use survey tools)
- Usage analytics (use product analytics)

**SUPPORT LEADS — NEVER use Copilot for:**
- Ticket resolution (use ticketing system)
- SLA tracking (use support platform)
- Performance metrics (use dashboards)
- Case assignment
- Knowledge base updates (use KB system)
- Bug reporting (use issue tracker)
- Customer data lookup (use CRM)

**ACCOUNT MANAGERS — NEVER use Copilot for:**
- Contract signing authority
- Pricing decisions
- Legal commitments
- Revenue forecasting
- Commission calculations
- Customer data exports
- Compliance certifications

**Customer Data Warnings:**
- Never include customer PII in prompts
- Don't share confidential business information
- Remember prompts may be logged
- Follow data handling policies
- Be careful with competitive information shared by customers

**Golden Rules:**
- CSMs: "Copilot monitors — CSMs build relationships"
- Support: "Copilot researches — support solves"
- AMs: "Copilot tracks — AMs own the relationship"

**System Integration Note:**
Copilot does NOT integrate with:
- CS platforms (Gainsight, ChurnZero, Totango)
- Support ticketing (Zendesk, ServiceNow, Freshdesk)
- CRM (Salesforce, HubSpot)
- Product analytics (Pendo, Amplitude)
- Survey tools (NPS, CSAT platforms)
```

---

### Knowledge Management

#### 1. [APPROVED] Similar Issue Search

**Use Case:** Find precedents for similar issues to inform troubleshooting.

**Target Personas:** Support Lead, Technical Support Engineer, Support Specialist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `support`, `troubleshooting`, `knowledge`

**Prompt:**

```
Search my emails and Teams for previous discussions about [Issue Type/Error]. Find:
- How we resolved similar issues before
- Workarounds that worked
- Root causes identified
- Team members who handled them
- Documentation created

This is research to inform current troubleshooting.
```

---

### Meeting Preparation

#### 1. [APPROVED] Meeting Preparation

**Use Case:** Prepare for customer meetings with full relationship context.

**Target Personas:** Account Manager, Customer Success Manager, Client Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `account-management`, `meeting-prep`, `customer`

**Prompt:**

```
I have a meeting with [Contact Name] at [Account Name]. Based on recent correspondence:
- What topics have they been focused on?
- Any outstanding issues or requests?
- Recent wins to celebrate?
- Items I committed to following up on?
- Potential concerns to address proactively?

Prepare briefing notes for my meeting prep.
```

---

### Onboarding

#### 1. [APPROVED] Onboarding Progress Summary

**Use Case:** Track onboarding progress from communications.

**Target Personas:** Customer Success Manager, Implementation Manager, Onboarding Specialist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `customer-success`, `onboarding`, `implementation`

**Prompt:**

```
Search for communications about [Customer Name]'s onboarding. Summarize:
- Implementation milestones discussed
- Training sessions completed/scheduled
- Blockers or delays mentioned
- Key contacts and their engagement
- Go-live timeline discussions
- Outstanding action items

Format as onboarding status update.
```

---

### Process Improvement

#### 1. [EXPERIMENTAL] Issue Pattern Analysis

**Use Case:** Identify support themes from discussions. Use ticketing analytics for metrics.

**Target Personas:** Support Lead, Support Manager, Operations Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `support`, `analytics`, `experimental`

**Prompt:**

```
Review support-related discussions over the past month. Identify recurring themes:
- Common issue types mentioned
- Product areas with frequent problems
- Customer segments affected
- Process gaps highlighted
- Training needs emerging

This is qualitative input for support improvement planning.

EXPERIMENTAL: Email analysis may miss issues logged only in ticketing system. Use support analytics for comprehensive trends.
```

---

### Renewals

#### 1. [APPROVED] Renewal Preparation

**Use Case:** Gather renewal context from communications. Contract details in CRM.

**Target Personas:** Customer Success Manager, Account Manager, Renewals Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `customer-success`, `renewal`, `preparation`

**Prompt:**

```
Search for all discussions related to [Customer Name]'s upcoming renewal. Compile:
- Contract terms mentioned
- Pricing discussions
- Value realized mentions
- Concerns or objections raised
- Competitive mentions
- Decision makers and their positions
- Timeline discussions

This is research for renewal planning. Actual contract details in CRM.
```

---

### Risk Management

#### 1. [APPROVED] At-Risk Account Assessment

**Use Case:** Identify risk signals from communications. Verify with platform data.

**Target Personas:** Account Manager, Customer Success Manager, Retention Specialist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `account-management`, `risk`, `churn`

**Prompt:**

```
Search for signals that [Account Name] may be at risk:
- Complaints or frustrations expressed
- Competitor mentions
- Reduced engagement discussed
- Budget concerns raised
- Champion departures mentioned
- Usage decline discussions

Compile as risk assessment input. Verify with usage data from platform.
```

---

### Team Management

#### 1. [APPROVED] Team Performance Context

**Use Case:** Gather qualitative team feedback for 1:1s and reviews. Metrics from ticketing system.

**Target Personas:** Support Lead, Support Manager, Customer Service Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `support`, `team-management`, `performance`

**Prompt:**

```
Search for feedback and discussions about my support team over the past month:
- Customer compliments received
- Issues or complaints mentioned
- Training needs identified
- Process improvement suggestions
- Workload concerns raised

This is context for team review. Actual metrics from support platform.
```

---

