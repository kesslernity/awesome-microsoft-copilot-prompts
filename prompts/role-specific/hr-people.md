# Copilot for HR & People

> Master Microsoft 365 Copilot for HR, talent, people ops, and L&D. Production-safe prompts for drafting, summarizing, and preparing — with strict guardrails. Copilot drafts and organizes; people leaders decide.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Operations & Support

**Prompts:** 16

---

## CRITICAL: HR GUARDRAILS - READ FIRST

### 1. HR Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any HR use of Copilot. People decisions and employee data demand human judgment and care.

**Target Personas:** HR Director, HR Manager, HR Business Partner, People Ops Lead, Talent Acquisition Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Use Copilot for HR

**Copilot drafts and organizes; it never decides about people. NEVER use it for:**

- Hiring, rejection, promotion, or termination decisions
- Disciplinary outcomes or grievance determinations
- Performance ratings or calibration decisions
- Compensation, bonus, or pay-equity decisions
- Employee-relations or legal determinations (discrimination, accommodation, etc.)
- Anything that screens or ranks candidates as a decision

**Employee-data care:**
- Be mindful of confidentiality and data protection when prompting
- Avoid pasting sensitive personal or special-category data
- Follow your AI, privacy, and works-council policies

**Bias warning:** AI can reflect and amplify bias. A human must review every people-facing output for fairness.

**Golden Rule:**
> "Copilot drafts and organizes. People leaders decide — with care, fairness, and a human in the loop."
```

---

## Talent Acquisition

### 2. Job Description Draft

**Use Case:** Draft an inclusive job description from a role brief, for hiring-manager review.

**Target Personas:** Talent Acquisition, HR Business Partner, Hiring Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `recruiting`, `job-description`

**Prompt:**

```
Draft a job description for [role] from this brief: [paste]. Include purpose, responsibilities, must-have vs nice-to-have requirements, and our EVP points. Use inclusive, plain language; avoid gendered or exclusionary terms. Mark "DRAFT — for hiring manager review." Flag anything missing as [TBC].
```

---

### 3. Interview Question Set

**Use Case:** Generate competency-based interview questions from a job description.

**Target Personas:** Talent Acquisition, Hiring Manager, HR Business Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `interviews`, `recruiting`

**Prompt:**

```
From this job description, generate a competency-based interview set: [paste JD].
- 2-3 questions per key competency
- A follow-up probe for each
- What a strong vs weak answer looks like

Behavioural, job-relevant, non-discriminatory. For interviewer use; scoring and the decision stay with the panel.
```

---

### 4. Candidate Screening Summary

**Use Case:** Summarize a CV against role requirements to prepare a human review. Not a screening decision.

**Target Personas:** Talent Acquisition, Hiring Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `screening`, `recruiting`

**Prompt:**

```
Summarize this CV against the role requirements I provide: [paste CV + requirements].
- Relevant experience present
- Requirements not evidenced
- Questions to explore at interview

Neutral and factual. This prepares a human review — it does NOT score, rank, or screen the candidate in or out.
```

---

### 5. Recruiting Outreach / Candidate Comms Draft

**Use Case:** Draft candidate-facing communications (outreach, updates, offers context), for review.

**Target Personas:** Talent Acquisition, Recruiter, HR Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `candidate-comms`, `recruiting`

**Prompt:**

```
Draft a [outreach / interview-invite / status-update] message to a candidate for [role], warm and professional: [context]. Keep it inclusive and clear on next steps. Draft for review — do not send. Do not state a decision unless I supply it.
```

---

## Performance & Development

### 6. Performance Feedback Draft

**Use Case:** Draft balanced SBI-model feedback from notes, for the manager to review and own.

**Target Personas:** Manager, HR Business Partner, HR Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `performance`, `feedback`

**Prompt:**

```
From these notes, draft balanced feedback using the SBI model (Situation-Behaviour-Impact): [paste]. Include strengths and development areas, specific and behavioural, not personal. Mark "DRAFT — manager to review and own." Do not assign a rating; ratings and calibration are the manager's decision.
```

---

### 7. L&D Module Outline

**Use Case:** Turn learning objectives into a training module outline for an SME to build out.

**Target Personas:** L&D Manager, Instructional Designer, HR Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `l-and-d`, `training`

**Prompt:**

```
From these objectives, outline a training module: [paste objectives + audience].
- Learning outcomes
- Section structure with key points
- Activities / checks for understanding
- Suggested duration

Draft outline for SME review. Flag where source content is needed.
```

---

## Employee Experience

### 8. Engagement Survey Theme Summary

**Use Case:** Summarize themes from open-text survey or feedback comments. Action planning stays human.

**Target Personas:** People Ops, HR Business Partner, HR Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `engagement`, `survey`

**Prompt:**

```
Summarize the themes in these open-text comments: [paste].
- Top recurring themes (with rough frequency)
- Positive signals
- Concerns raised
- Notable verbatim examples (anonymized)

Neutral summary for the people team. Do not attribute comments to individuals; action planning is a human decision.
```

---

### 9. Exit Interview Theme Summary

**Use Case:** Aggregate exit-interview notes into themes to inform retention. Keep individuals anonymous.

**Target Personas:** HR Business Partner, People Ops, HR Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `attrition`, `retention`

**Prompt:**

```
From these exit-interview notes, identify recurring themes: [paste].
- Top reasons for leaving
- Patterns by team/role if visible
- What leavers said would have helped

Aggregate and anonymize. This is input for retention discussion, not a conclusion about any manager or team.
```

---

## Communications

### 10. Team / Org Announcement Draft

**Use Case:** Draft a people announcement (hire, departure, change), for review before sending.

**Target Personas:** HR Manager, Manager, Internal Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `announcement`, `communication`

**Prompt:**

```
Draft a [hire / departure / role-change / restructure] announcement: [context]. Warm, respectful, appropriate detail only. For sensitive changes keep it factual and dignified. Draft for review — confirm what is shareable before sending.
```

---

### 11. Policy Explainer / FAQ Draft

**Use Case:** Turn an HR policy into a plain-language explainer or FAQ for employees, for review.

**Target Personas:** HR Manager, People Ops, Internal Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `policy`, `communication`

**Prompt:**

```
From this HR policy, draft a plain-language FAQ for employees: [paste or reference]. Cover the questions people actually ask, in clear non-legalistic language. Mark "DRAFT — HR to review for accuracy." Do not interpret edge cases; route those to HR.
```

---

## Operations

### 12. Onboarding Plan Builder

**Use Case:** Build a structured onboarding plan for a new hire from a role brief.

**Target Personas:** Manager, HR Coordinator, People Ops

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `onboarding`, `operations`

**Prompt:**

```
Build a 30/60/90-day onboarding plan for a new [role]: [context]. Include pre-arrival setup, week-1 essentials, key people to meet, early goals, and check-in points. Practical and specific. Mark items needing manager input as [TBC].
```

---

### 13. Employee Relations Case Notes Organization

**Use Case:** Organize ER case correspondence into a factual chronology. Never an adjudication.

**Target Personas:** HR Business Partner, ER Specialist, HR Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `employee-relations`, `chronology`

**Prompt:**

```
For case [reference], organize the correspondence into a factual chronology: date, event, parties, document reference. Strictly factual — no view on fault, credibility, or outcome. This is case-file organization for the responsible HR/ER lead, not an investigation finding or determination. Handle with confidentiality.
```

---

## Reward & Reporting

### 14. Compensation Benchmark Research Prep

**Use Case:** Gather internal context for a comp review. Benchmarks and decisions are owned by reward/HR.

**Target Personas:** Reward Manager, HR Business Partner, HR Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `compensation`, `research`

**Prompt:**

```
For a comp review of [role/team], gather from internal documents and emails:
- Prior comp decisions or ranges discussed
- Retention or offer pressures mentioned
- Relevant policy points

Summarize as context. This does NOT set pay or recommend amounts — comp decisions follow your reward process and require human sign-off.
```

---

### 15. HR Metrics Brief Prep

**Use Case:** Assemble context for an HR metrics or people review. Authoritative data comes from the HRIS.

**Target Personas:** HR Director, People Analytics, HR Business Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `metrics`, `reporting`

**Prompt:**

```
For my people review of [team/area], gather from emails and documents:
- Headcount / hiring / attrition points discussed
- Engagement or capability concerns raised
- Actions from last review and status

Compile as context. Authoritative people metrics come from the HRIS — confirm figures before reporting.
```

---

### 16. Recognition / Review-Cycle Comms Draft

**Use Case:** Draft communications for a recognition or performance-cycle moment, for review.

**Target Personas:** HR Manager, Manager, People Ops

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `recognition`, `communication`

**Prompt:**

```
Draft [recognition message / review-cycle kickoff / deadline reminder] comms: [context]. Clear, motivating, inclusive. For recognition, make it specific and genuine. Draft for review before sending.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
