# Copilot for Data Privacy (DPO)

> Master Microsoft 365 Copilot for data protection officers, privacy counsel, and privacy teams. Production-safe prompts for DPIAs, ROPA, DSARs, breach prep, and transfers — with strict guardrails. Copilot prepares the paperwork; the DPO decides.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Security & Compliance

**Prompts:** 16

---

## CRITICAL: DATA PRIVACY GUARDRAILS - READ FIRST

### 1. Data Privacy Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any privacy use of Copilot. Privacy determinations are high-stakes, jurisdiction-specific, and human.

**Target Personas:** Data Protection Officer, Privacy Counsel, Privacy Manager, Compliance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `dpo`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Use Copilot for Data Privacy

**Copilot prepares the paperwork; it never makes the privacy decision. NEVER use it to:**

- Determine the lawful basis or that processing is lawful
- Decide whether a breach is notifiable, or the notification timing
- Rate or accept DPIA / transfer risk
- Decide what to disclose or redact in a DSAR
- Conclude that safeguards or a transfer mechanism are adequate
- Give a compliance determination or legal advice

**Jurisdiction warning:** privacy law differs by jurisdiction (GDPR, UK GDPR, CCPA/CPRA, and more). Copilot does not know which law applies — treat every output as a draft for a qualified privacy professional in the relevant jurisdiction.

**Data minimisation in prompting:**
- Do NOT paste personal data, special-category data, or identifiable records into prompts
- Work from descriptions, categories, and metadata, not the data subjects' data
- Prompts may be logged and are not automatically privileged

**Golden Rule:**
> "Copilot prepares the paperwork. The DPO assesses, decides, and signs."
```

---

## DPIA

### 2. DPIA Scaffold Draft

**Use Case:** Draft a DPIA scaffold from a processing description. Risk rating and the decision are the DPO's.

**Target Personas:** Data Protection Officer, Privacy Manager, Privacy Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `dpia`, `drafting`

**Prompt:**

```
From this processing description, draft a DPIA scaffold: [describe the processing — purposes, data categories, parties; no actual personal data].
- Description of processing and purposes
- Necessity and proportionality questions to answer
- Risks to data subjects to consider (as prompts, not ratings)
- Possible mitigations to evaluate

Mark "DRAFT — risk rating and sign-off by the DPO." Leave the risk-level and residual-risk fields blank for the human to complete.
```

---

### 3. Privacy-by-Design Review Prep

**Use Case:** Generate the privacy questions to put to a new project at design stage.

**Target Personas:** Privacy Manager, Data Protection Officer, Privacy Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `privacy-by-design`, `review`

**Prompt:**

```
For the new [project/system] described here, draft a privacy-by-design review checklist of questions to ask the project team: [describe purpose and data flows]. Cover data minimisation, purpose limitation, retention, access, transfers, transparency, and data subject rights. These are questions to put to the team — not findings or approvals.
```

---

## Records

### 4. ROPA Entry Draft

**Use Case:** Draft a Record of Processing Activities entry from a description, for the DPO to verify.

**Target Personas:** Privacy Manager, Data Protection Officer, Privacy Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `ropa`, `records`

**Prompt:**

```
Draft a ROPA entry from this processing description: [purpose, data categories, subjects, recipients, retention, transfers — no personal data].
Fields: controller/processor role, purpose, categories of data and subjects, recipients, retention, transfers and safeguards, security measures [TBC].
Mark "DRAFT — verify with the process owner and DPO." Do not assert a lawful basis; flag it as [to be confirmed by DPO].
```

---

### 5. Records & Retention Schedule Draft

**Use Case:** Draft a retention schedule outline from inputs, for legal/DPO review.

**Target Personas:** Privacy Manager, Records Manager, Data Protection Officer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `retention`, `records`

**Prompt:**

```
Draft a retention schedule outline for [record type/area] from the inputs I provide:
- Record category
- Suggested retention basis discussed [mark to confirm]
- Trigger for the clock
- Disposal method

Mark "DRAFT — retention periods to be confirmed against legal/regulatory requirements by the DPO/legal." Do not assert legally required periods.
```

---

## Data Subject Rights

### 6. DSAR Intake & Scoping

**Use Case:** Structure an inbound data subject request into intake and scope. Not the response decision.

**Target Personas:** Privacy Manager, Data Protection Officer, Privacy Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `dsar`, `intake`

**Prompt:**

```
From this data subject request, produce a structured intake: [paste the request text — not their wider personal data].
- Requester and right(s) invoked (access, erasure, rectification, etc.)
- What they are asking for and any date range
- Identity verification status [TBC]
- Likely systems/teams in scope
- Statutory clock start and key dates [confirm]

This scopes the request for the privacy team. It does not decide the response, exemptions, or what to disclose.
```

---

### 7. DSAR Response Pack Prep

**Use Case:** Organize the gathering of a DSAR response. Disclosure and redaction decisions stay human.

**Target Personas:** Privacy Manager, Data Protection Officer, Privacy Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `dsar`, `response`

**Prompt:**

```
For DSAR [reference], help organize the response process:
- Checklist of sources/systems to search
- A log structure to track what was found and reviewed
- A redaction-decision checklist (third-party data, exemptions) for the reviewer to apply

Prepare the process and checklists only. Copilot does not decide what is disclosed, exempt, or redacted — a human reviewer makes every disclosure call.
```

---

## Breach

### 8. Breach Assessment Prep

**Use Case:** Organize the facts of a suspected breach for assessment. Notifiability is a human decision.

**Target Personas:** Data Protection Officer, Privacy Manager, Incident Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `breach`, `incident`

**Prompt:**

```
For the suspected personal-data breach described here, organize the facts for assessment: [what happened, when discovered, data categories and approx numbers involved — no personal data].
- Timeline of events
- Data and data subjects affected (categories/volumes)
- Containment actions taken
- Open questions for the assessment

Structure only. Copilot does NOT decide whether this is notifiable, to whom, or by when — the DPO assesses notifiability and timing against the applicable law.
```

---

## Transfers

### 9. Transfer Impact Assessment (TIA) Prep

**Use Case:** Draft a TIA scaffold for an international transfer. Adequacy and risk are the DPO's call.

**Target Personas:** Data Protection Officer, Privacy Counsel, Privacy Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `transfers`, `tia`

**Prompt:**

```
Draft a transfer impact assessment scaffold for sending [data categories] from [origin] to [destination] via [mechanism, e.g., SCCs]: [describe — no personal data].
- Transfer details and mechanism
- Questions on the destination's legal regime to research
- Supplementary measures to consider
- Residual-risk fields [left blank for DPO]

Mark "DRAFT — adequacy and residual risk to be assessed by the DPO." Do not conclude the transfer is lawful or the safeguards adequate.
```

---

### 10. Vendor / Processor Privacy Due Diligence Prep

**Use Case:** Assemble privacy due-diligence questions and gathered info for a processor. Approval is human.

**Target Personas:** Privacy Manager, Data Protection Officer, Vendor/Procurement

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `processor`, `due-diligence`

**Prompt:**

```
For onboarding [processor] handling [data categories], prepare privacy due diligence:
- A questionnaire (security, sub-processors, location/transfers, breach process, deletion, certifications)
- What we already hold internally on them
- A gaps/missing-info list

Compile the pack and gaps. It does not clear or approve the processor — that's a human privacy decision after review.
```

---

## Transparency

### 11. Privacy Notice Draft

**Use Case:** Draft a privacy notice or a section of one from inputs, for legal/DPO review.

**Target Personas:** Privacy Counsel, Data Protection Officer, Privacy Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `notice`, `transparency`

**Prompt:**

```
Draft a [privacy notice / privacy notice section on X] from these inputs: [purposes, data categories, recipients, retention, rights — no personal data]. Plain, transparent language. Mark "DRAFT — for legal/DPO review and jurisdiction check." Flag any required element not supplied as [TBC]; do not state a lawful basis as settled.
```

---

### 12. Consent / Lawful Basis Options Draft

**Use Case:** Lay out the lawful-basis options to consider for a processing activity. The DPO determines the basis.

**Target Personas:** Data Protection Officer, Privacy Counsel, Privacy Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `lawful-basis`, `analysis`

**Prompt:**

```
For this processing, lay out the lawful-basis options to consider: [describe the processing]. For each candidate basis, note what it would require and questions to resolve. Present as options and considerations only. The DPO/privacy counsel determines and documents the actual basis — do not pick one as the answer.
```

---

## Operations

### 13. Privacy Training / Awareness Content Draft

**Use Case:** Draft privacy awareness content for staff, for review.

**Target Personas:** Privacy Manager, DPO, L&D

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `training`, `awareness`

**Prompt:**

```
Draft privacy awareness content on [topic, e.g., handling personal data in email] for [audience]. Practical do's and don'ts, short scenarios, and a quick checklist. Plain language. Mark "DRAFT — for DPO review." Keep examples generic; use no real personal data.
```

---

### 14. Privacy Policy / Procedure Explainer

**Use Case:** Turn a privacy policy or procedure into a plain-language explainer for staff, for review.

**Target Personas:** Privacy Manager, DPO, Internal Comms

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `policy`, `communication`

**Prompt:**

```
From this privacy policy/procedure, draft a plain-language explainer for employees: [paste or reference]. Cover what it means in practice and the questions staff ask. Mark "DRAFT — DPO to review for accuracy." Route edge cases to the privacy team rather than interpreting them.
```

---

### 15. Privacy Risk Register Prep

**Use Case:** Compile privacy risks raised internally into a register structure, for the DPO to assess.

**Target Personas:** Data Protection Officer, Privacy Manager, Risk

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `risk`, `register`

**Prompt:**

```
Search internal emails and documents for privacy risks raised about [area/project]:
- Risk described
- Where it arises
- Any mitigation discussed
- Owner mentioned

Compile into a risk-register structure with the likelihood/impact/rating fields left blank. The DPO rates and owns the assessment.
```

---

## Regulator

### 16. Regulator Correspondence Prep

**Use Case:** Organize context for correspondence with a supervisory authority. Responses require DPO/legal sign-off.

**Target Personas:** Data Protection Officer, Privacy Counsel, Compliance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `privacy`, `regulator`, `preparation`

**Prompt:**

```
For correspondence with [supervisory authority] about [matter], gather context from internal emails and documents:
- What was asked or what we need to address
- Relevant facts and prior correspondence
- Documents likely needed

Draft a response outline with evidence pointers. The response must be reviewed and signed off by the DPO/legal before it is sent — Copilot does not provide regulatory advice.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
