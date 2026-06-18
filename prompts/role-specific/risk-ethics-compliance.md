# Copilot for Risk, Ethics & Compliance

> Master Microsoft 365 Copilot for GRC — compliance, ethics, anti-bribery, and risk. Production-safe prompts for policy drafting, due diligence, controls mapping, and investigation prep — with strict guardrails. Copilot prepares; compliance, ethics, and legal decide.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Security & Compliance

**Prompts:** 16

---

## CRITICAL: RISK, ETHICS & COMPLIANCE GUARDRAILS - READ FIRST

### 1. Risk, Ethics & Compliance Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any GRC use of Copilot. Compliance, ethics, and investigation conclusions are human and confidential.

**Target Personas:** Compliance Officer, Ethics & Compliance Counsel, Risk Manager, Internal Audit

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `ethics`, `risk`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Use Copilot for Risk, Ethics & Compliance

**Copilot prepares; it never rules, finds, or accepts. NEVER use it to:**

- Make a compliance determination or give legal advice
- Reach an ethics ruling (conflict of interest, gift, conduct)
- Reach an investigation finding, conclusion, or credibility assessment
- Decide a disciplinary outcome
- Accept, rate, or sign off a risk
- Clear a third party in due diligence

**Confidentiality:** investigations and whistleblower/speak-up matters are highly confidential and may be privileged. Do not paste names, allegations, or identifying details into prompts; work from structure and process.

**Jurisdiction & sources:** obligations differ by jurisdiction and change. Copilot does not hold current law or your control framework — verify against the official source and your policies.

**Golden Rule:**
> "Copilot prepares the paperwork and the questions. Compliance, ethics, and legal investigate, assess, and decide."
```

---

## Policy

### 2. Compliance Policy / Procedure Draft

**Use Case:** Draft a compliance or ethics policy (e.g., code of conduct, ABAC, COI) from requirements, for review.

**Target Personas:** Compliance Officer, Ethics & Compliance Counsel, Policy Owner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `policy`, `drafting`

**Prompt:**

```
Draft a first-draft [policy, e.g., anti-bribery & corruption / conflicts of interest / code of conduct] from these requirements: [list]. Reference any existing related policy in SharePoint for tone and structure. Include purpose, scope, definitions, the rules, roles & responsibilities, reporting routes, and review cadence. Mark "DRAFT — for compliance/legal review and jurisdiction check." Leave [brackets] for gaps; do not assert legal requirements.
```

---

### 3. Policy Explainer / FAQ Draft

**Use Case:** Turn a compliance policy into a plain-language explainer or FAQ for staff, for review.

**Target Personas:** Compliance Officer, Ethics Officer, Internal Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `policy`, `communication`

**Prompt:**

```
From this compliance/ethics policy, draft a plain-language FAQ for employees: [paste or reference]. Cover the questions people actually ask and what to do in common situations, in clear non-legalistic language. Mark "DRAFT — compliance to review for accuracy." Route edge cases to compliance rather than interpreting them.
```

---

## Ethics

### 4. Conflict of Interest (COI) Disclosure Triage

**Use Case:** Structure a COI disclosure into an assessment intake. The determination is the ethics/compliance officer's.

**Target Personas:** Ethics & Compliance Officer, Compliance Manager, HR/Compliance liaison

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `conflict-of-interest`, `ethics`

**Prompt:**

```
From this conflict-of-interest disclosure, produce a structured intake for assessment: [paste the disclosure].
- Who is disclosing and their role
- Nature of the potential conflict
- Parties and interests involved
- What's being requested (approval, recusal, mitigation)
- Information still needed

This prepares the assessment. It does NOT decide whether a conflict exists or how to manage it — the ethics/compliance officer determines that.
```

---

### 5. Gifts & Hospitality Review Prep

**Use Case:** Organize a gifts & hospitality item against the policy thresholds for the approver. Not approval.

**Target Personas:** Ethics & Compliance Officer, Compliance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `gifts-hospitality`, `ethics`

**Prompt:**

```
For this gift/hospitality entry, organize it for review: [paste details].
- Giver/recipient, value, occasion, frequency
- Relationship to any live tender/decision
- The policy thresholds it should be checked against [reference policy]
- Flags to consider (timing near a decision, public official involved)

Present for the approver. Do NOT approve, decline, or rule it acceptable — that is the approver's decision under the policy.
```

---

## Third Parties

### 6. Third-Party / ABAC Due Diligence Prep

**Use Case:** Assemble anti-bribery due-diligence questions and gathered info on a third party. Clearance is human.

**Target Personas:** Compliance Officer, ABAC Officer, Procurement/Compliance liaison

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `abac`, `due-diligence`

**Prompt:**

```
For onboarding [third party / intermediary], prepare anti-bribery due diligence:
- A risk-based questionnaire (ownership, government links/PEPs, use of sub-agents, payment terms, references)
- What we already hold internally on them
- A red-flag checklist to consider
- Gaps to obtain

Compile the pack and gaps. It does NOT clear the third party or assess their risk level — that is a human compliance decision after review and screening.
```

---

## Speak-Up & Investigations

### 7. Whistleblower / Speak-Up Intake

**Use Case:** Structure a speak-up report into a confidential intake. Never an assessment of the allegation.

**Target Personas:** Ethics & Compliance Officer, Investigations Lead, Compliance Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `whistleblower`, `intake`

**Prompt:**

```
From this speak-up report, produce a structured, confidential intake: [paste the report text only — minimise identifying detail].
- Category of concern
- What is alleged (factually, neutrally)
- When/where, as stated
- What the reporter is asking for
- Immediate considerations (confidentiality, anti-retaliation, conflicts in who reviews)
- Information needed to scope

Handle as strictly confidential. This intake does NOT assess credibility, substantiate, or conclude anything — that is for the investigation under the proper process.
```

---

### 8. Investigation Plan / Chronology Prep

**Use Case:** Organize facts and a timeline for an investigation file. Never a finding or conclusion.

**Target Personas:** Investigations Lead, Compliance Counsel, Ethics Officer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `investigation`, `chronology`

**Prompt:**

```
For investigation [reference], help organize the file: [provide the factual material — minimise identifying detail].
- A factual, sourced chronology of events
- An evidence index (what exists, where)
- An investigation plan outline (lines of enquiry, who to interview) for the lead to set
- Open questions

Strictly factual and confidential. Do NOT assess credibility, attribute fault, substantiate, or conclude — findings are the investigator's under the process, often privileged.
```

---

## Regulatory & Controls

### 9. Regulatory Obligations Brief

**Use Case:** Summarize a regulatory change for the compliance team to assess its control impact. Not a determination.

**Target Personas:** Compliance Officer, Compliance Counsel, Regulatory Affairs

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `regulatory`, `obligations`

**Prompt:**

```
Search emails and SharePoint for discussion of [regulation/obligation]. Summarize:
- What is required or changing (as discussed)
- Which processes/controls appear affected
- Actions proposed
- Open questions

Mark "For compliance review — not a compliance determination." Confirm requirements against the current official source; Copilot does not provide regulatory advice.
```

---

### 10. Controls Mapping Draft

**Use Case:** Map a requirement to existing controls and surface gaps, for review.

**Target Personas:** Compliance Officer, Risk Manager, Internal Audit

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `controls`, `mapping`

**Prompt:**

```
Map the requirement [paste/describe] to our controls described here [paste control descriptions]:
- Requirement broken into discrete obligations
- Control(s) that appear to address each
- Apparent gaps or partial coverage
- Questions to confirm with control owners

Mark "DRAFT — for review with control owners." Do not conclude the organisation is compliant or that a control is effective — that requires human assessment and testing.
```

---

## Risk

### 11. Risk Register / ERM Prep

**Use Case:** Compile risks raised internally into a register structure. Ratings and acceptance are human.

**Target Personas:** Risk Manager, Compliance Officer, Internal Audit

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `risk`, `register`

**Prompt:**

```
Search internal emails and documents for risks raised about [area/process]:
- Risk described
- Cause/source and potential impact (as discussed)
- Any mitigation or owner mentioned

Compile into a risk-register structure with the likelihood/impact/rating and risk-acceptance fields left blank. The risk owner/committee rates, accepts, and owns the assessment.
```

---

### 12. Compliance Monitoring / Testing Plan Prep

**Use Case:** Draft a monitoring or controls-testing plan outline, for review.

**Target Personas:** Compliance Officer, Internal Audit, Risk Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `monitoring`, `testing`

**Prompt:**

```
Draft a monitoring/testing plan outline for [control area/policy] from the inputs I provide:
- What to test and why
- Sample approach and frequency [to confirm]
- Evidence to gather
- How results will be recorded and escalated

Mark "DRAFT — for review." This plans the testing; it does not perform it or conclude control effectiveness.
```

---

## Governance & Reporting

### 13. Board / Committee Compliance Report Prep

**Use Case:** Assemble inputs for a compliance/ethics report to a board or committee. Not assurance.

**Target Personas:** Compliance Officer, Compliance Counsel, Company Secretary

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `board`, `reporting`

**Prompt:**

```
For the [board/committee] compliance update, assemble from reports and emails:
- Programme status and key activities
- Issues, incidents, and trends raised (no identifying detail on cases)
- Regulatory developments noted
- Decisions/approvals being sought

Structure as draft sections for review. This is preparation, not assurance — the compliance officer owns what is reported.
```

---

### 14. Compliance Training Content Draft

**Use Case:** Draft compliance/ethics training content for staff, for review.

**Target Personas:** Compliance Officer, Ethics Officer, L&D

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `training`, `ethics`

**Prompt:**

```
Draft compliance/ethics training content on [topic, e.g., anti-bribery, conflicts of interest, speak-up] for [audience]. Practical scenarios, do's and don'ts, the decision to escalate, and how to report. Plain language. Mark "DRAFT — for compliance review." Keep examples generic; confirm rules with the team.
```

---

### 15. Compliance / Ethics Awareness Comms Draft

**Use Case:** Draft an awareness communication (e.g., speak-up week, policy reminder), for review.

**Target Personas:** Compliance Officer, Ethics Officer, Internal Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `awareness`, `communication`

**Prompt:**

```
Draft an awareness communication on [topic, e.g., the speak-up line, gifts policy reminder, code of conduct refresh]: [context]. Clear, encouraging, with the action and the reporting/help route. Draft for review before sending.
```

---

## Incidents

### 16. Compliance Incident Context Prep

**Use Case:** Organize the facts of a potential compliance/policy breach. Disposition is a human decision.

**Target Personas:** Compliance Officer, Compliance Counsel, Risk Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `compliance`, `incident`, `preparation`

**Prompt:**

```
For the potential compliance/policy breach described here, organize the facts: [what happened, when, policy/area involved — minimise identifying detail].
- Timeline of events
- What appears to have occurred (factual)
- Policy/obligation potentially engaged
- Actions taken so far
- Open questions

Structure only. Whether this is a breach, its severity, escalation, and any disclosure are decided by compliance/legal — Copilot does not assess or conclude.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
