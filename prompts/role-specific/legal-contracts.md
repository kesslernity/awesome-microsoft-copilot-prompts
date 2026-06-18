# Copilot for In-House Legal & Contracts

> Master Microsoft 365 Copilot for in-house legal, contract management, and legal operations. Production-safe prompts for corporate counsel, contracts managers, paralegals, and legal ops — with strict guardrails. Copilot retrieves and drafts; lawyers advise and decide.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants. Where a prompt is noted as draft-from-input, it also works from pasted text.

**Category:** Security & Compliance

**Prompts:** 18

---

## CRITICAL: LEGAL GUARDRAILS - READ FIRST

### 1. Legal Critical Guardrails - Read First

**Use Case:** CRITICAL: Read this before any legal or contracts use of Copilot. Share with everyone in the legal function.

**Target Personas:** General Counsel, Corporate Counsel, Contracts Manager, Legal Operations, Paralegal, Compliance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `contracts`, `guardrails`, `critical`

**Prompt:**

```
## CRITICAL: When NEVER to Use Copilot for Legal & Contracts

**Copilot output is NEVER legal advice, however it is worded.** It MUST NEVER be used for:

### Advice & Interpretation
- Legal advice, opinions, or conclusions
- Authoritative contract interpretation
- Entitlement, liability, or risk determinations
- Litigation strategy or settlement authority
- Regulatory or compliance determinations

### Binding Actions
- Executing, signing, or amending a contract
- Issuing legal notices or waivers
- Filing, serving, or responding to court/regulator deadlines
- Making or accepting an offer

### Judgment Calls
- Privilege or relevance calls in disclosure/e-discovery
- Whether a clause is enforceable in a jurisdiction
- Whether to litigate, escalate, or concede

**Jurisdiction Warning:** Law is jurisdiction-specific. Copilot does not know which law governs your matter. Treat every output as a starting draft for a qualified lawyer in the relevant jurisdiction.

**Privilege & Confidentiality Warning:**
- Prompts and outputs may be logged and are not automatically privileged
- Do not paste matter content that could waive privilege
- Follow your organization's AI and outside-counsel policies

**System Integration Note:** Copilot does NOT connect to your CLM, legal research databases (Westlaw/LexisNexis), e-billing, or court filing systems.

**Golden Rule:**
> "Copilot retrieves and drafts. Lawyers advise and decide."

**No AI output ever replaces qualified legal judgment.**
```

---

## Contract Abstraction

### 2. Contract Key-Terms Abstraction

**Use Case:** Pull the key commercial and legal terms out of a contract into a review table. Always verify against the executed version.

**Target Personas:** Contracts Manager, Corporate Counsel, Legal Operations, Paralegal

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `abstraction`, `review`

**Prompt:**

```
You are assisting an in-house legal professional. From the contract document I reference (in SharePoint or pasted), extract the key terms into a table:
- Parties and signing entities
- Effective date, term, and renewal mechanism
- Contract value and payment terms
- Limitation of liability and indemnity (quote the clause reference)
- Termination rights and notice periods
- Governing law and dispute resolution
- Confidentiality / data protection references

Mark anything not found as "Not located — verify." This is a draft abstraction for legal review, not an interpretation of the terms.
```

---

## Clause Comparison

### 3. Clause Comparison Against Our Standard

**Use Case:** Compare a counterparty's clause against our standard/playbook position and surface the deviations for a reviewer.

**Target Personas:** Corporate Counsel, Contracts Manager, Commercial Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `clause`, `review`, `experimental`

**Prompt:**

```
Compare the [clause type, e.g., "limitation of liability"] clause in the counterparty draft I reference against our standard template clause in SharePoint. Produce:
- Side-by-side summary of each version
- Specific deviations (caps, carve-outs, mutual vs one-way, defined terms)
- A neutral "points a reviewer should check" list

Do NOT advise which is acceptable or assess enforceability. This is reviewer-prep only and requires qualified legal assessment.

EXPERIMENTAL: Clause meaning depends on the whole contract and governing law. Always read the full document.
```

---

## Redline Preparation

### 4. Counterparty Draft Issues List

**Use Case:** Read an inbound third-party draft and produce a reviewer's issues list against our known positions, to speed up redlining.

**Target Personas:** Corporate Counsel, Contracts Manager, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `redline`, `review`

**Prompt:**

```
Review the counterparty contract draft I reference. Against the standard positions in our contract playbook (SharePoint), produce an issues list for the reviewing lawyer:
- Clause / section reference
- What the draft says (brief)
- How it deviates from our standard position
- Suggested point to raise (neutral wording, not advice)

Flag any clause our playbook does not cover as "No standard position on file." This is preparation for a lawyer's redline, not legal advice or an approval.
```

---

## NDA Drafting

### 5. NDA First-Draft from a Brief

**Use Case:** Produce a first-draft NDA from a short brief, clearly marked for legal review before use.

**Target Personas:** Corporate Counsel, Contracts Manager, Paralegal, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `nda`, `drafting`

**Prompt:**

```
Draft a first-draft mutual NDA from these parameters:
- Parties: [names/entities]
- Purpose of disclosure: [describe]
- Term and survival: [e.g., 3 years / 5 years survival]
- Governing law: [jurisdiction — REQUIRED, do not assume]
- Any specific carve-outs: [list or "standard"]

Base it on our NDA template in SharePoint if available. Mark the document "DRAFT — FOR LEGAL REVIEW" at the top, leave [SQUARE BRACKETS] for every item not supplied, and add a reviewer checklist at the end. This is a drafting aid; a qualified lawyer must review and approve before it is sent or signed.
```

---

## Obligations Tracking

### 6. Obligations & Key Dates Extraction

**Use Case:** Extract obligations, milestones, and notice/renewal dates from a contract into a tracker.

**Target Personas:** Contracts Manager, Legal Operations, Paralegal, Commercial Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `obligations`, `tracking`

**Prompt:**

```
From the contract I reference, extract into a table every obligation and key date:
- Obligation / deliverable
- Responsible party
- Due date or trigger
- Notice period (if any)
- Clause reference

Separately list all renewal, expiry, and termination-notice deadlines. Mark anything ambiguous as "Verify against contract." This is an operational tracker for review — it does not interpret whether an obligation has been met.
```

---

## Legal Research (Internal)

### 7. Internal Precedent & Memo Summary

**Use Case:** Find and summarize our own internal precedents, opinions, or memos on a topic. Applicability requires qualified assessment.

**Target Personas:** Corporate Counsel, Paralegal, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `research`, `precedents`

**Prompt:**

```
Search SharePoint for our internal memos, opinions, or precedent documents on [issue, e.g., "force majeure" or "limitation of liability"]. Summarize:
- Documents found (title, date, author/team if visible)
- The position or approach taken in each
- Any caveats or conditions noted

This is internal-knowledge retrieval for reference only. It is NOT external legal research and NOT advice — applicability to a new matter requires qualified legal assessment, including current law in the relevant jurisdiction.
```

---

## Matter Management

### 8. Matter Status Summary

**Use Case:** Compile a status summary for a legal matter from correspondence and documents, for an internal update.

**Target Personas:** Corporate Counsel, Legal Operations, Paralegal

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `matter`, `status`

**Prompt:**

```
For [matter name/reference], search my emails, Teams, and SharePoint to compile a status summary:
- Current stage and what is outstanding
- Key recent developments (with dates)
- Pending decisions or approvals
- Upcoming deadlines mentioned
- Who is responsible for the next action

Format as briefing notes for an internal legal team update. This is organization of existing information, not legal strategy or advice.
```

---

## Dispute Files

### 9. Dispute Chronology Builder

**Use Case:** Build a chronological case file of events and communications for a dispute. Strategy requires counsel.

**Target Personas:** Corporate Counsel, Litigation Counsel, Paralegal, Commercial Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `disputes`, `chronology`

**Prompt:**

```
For the dispute with [party], search emails and documents and build a chronological timeline:
- Date
- Event or communication
- Parties involved
- Document/email reference

Keep it strictly factual and sourced. Do not characterize fault, merits, or strategy. This is case-file organization for the responsible lawyer — not litigation analysis or advice.
```

---

## Regulatory Tracking

### 10. Regulatory & Policy Change Brief

**Use Case:** Summarize internal discussion and referenced material on a regulatory change, flagged for compliance review.

**Target Personas:** Compliance Manager, Corporate Counsel, Regulatory Affairs, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `regulatory`, `compliance`, `research`

**Prompt:**

```
Search emails and SharePoint for discussion of [regulation/topic, e.g., "EU AI Act obligations"]. Summarize:
- What is changing or required (as discussed internally)
- Which teams/contracts appear affected
- Actions proposed or taken
- Open questions raised

Mark this "For compliance review — not a compliance determination." Copilot does not provide regulatory advice; a qualified reviewer must confirm requirements against the current official source.
```

---

## Privacy & Data Protection

### 11. DPA / Data-Protection Clause Checklist

**Use Case:** Check a contract or processing arrangement against a data-protection checklist; flag missing elements for review.

**Target Personas:** Privacy Counsel, DPO, Corporate Counsel, Contracts Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `privacy`, `gdpr`, `review`

**Prompt:**

```
Review the contract / DPA I reference against this data-protection checklist and mark each as Present / Missing / Unclear with the clause reference:
- Roles (controller / processor / sub-processor)
- Purpose and scope of processing
- Sub-processor approval and flow-down
- Security measures reference
- Data subject rights assistance
- Breach notification timing
- International transfer mechanism
- Audit and deletion/return on termination

This is a completeness check for a reviewer, NOT a determination of GDPR/data-protection compliance. A qualified reviewer must assess against the applicable law and jurisdiction.
```

---

## E-Discovery

### 12. Document Triage Preparation

**Use Case:** Organize and theme a document set to speed up human review. Never a privilege or relevance determination.

**Target Personas:** Litigation Counsel, Paralegal, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `e-discovery`, `triage`, `experimental`

**Prompt:**

```
For the document set I reference relating to [matter], help me organize for human review:
- Group documents by theme/topic
- Note apparent date ranges and key custodians/senders
- Flag documents that mention [key terms] for priority human review

Do NOT make relevance, privilege, or responsiveness calls — those are decisions for the legal team. Preserve everything; this only orders the set for review.

EXPERIMENTAL: AI grouping can miss or mis-bucket documents. Every document still requires human review.
```

---

## Governance

### 13. Board / Committee Minutes Draft

**Use Case:** Draft minutes from board or committee notes for the company secretary to review and finalize.

**Target Personas:** Company Secretary, Legal Operations, Corporate Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `governance`, `minutes`, `drafting`

**Prompt:**

```
Draft minutes from the meeting notes I provide (pasted or in SharePoint). Structure:
- Attendees, apologies, quorum
- Agenda items in order
- Key discussion points (concise, neutral)
- Decisions and resolutions (mark clearly)
- Actions with owners and dates

Mark "DRAFT — for Company Secretary review." Do not record anything not in the notes; flag gaps as "[To confirm]". Minutes are a formal record — the secretary must verify and approve before circulation.
```

---

## Policy Drafting

### 14. Internal Policy First-Draft

**Use Case:** Draft an internal policy from requirements, for legal and stakeholder review.

**Target Personas:** Corporate Counsel, Compliance Manager, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `policy`, `drafting`

**Prompt:**

```
Draft a first-draft internal policy on [topic, e.g., "acceptable AI use" or "data retention"] from these requirements: [list]. Reference any existing related policy in SharePoint for tone and structure. Include:
- Purpose and scope
- Definitions
- Policy statements / rules
- Roles and responsibilities
- Exceptions and escalation
- Review cadence

Mark "DRAFT — for legal and stakeholder review." Leave [brackets] where input is missing. This is a drafting aid; legal must review for jurisdictional and regulatory fit before adoption.
```

---

## Contract Lifecycle

### 15. Renewal & Expiry Watch

**Use Case:** Surface upcoming renewals, expiries, and notice deadlines from the contract register for action.

**Target Personas:** Contracts Manager, Legal Operations, Commercial Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `renewals`, `tracking`

**Prompt:**

```
From our contract register / repository in SharePoint, list contracts with renewal or expiry dates in the next [timeframe, e.g., 90 days]:
- Contract / counterparty
- Expiry or renewal date
- Notice deadline to terminate or renegotiate
- Auto-renew? (Yes/No/Unknown)
- Owner

Sort by soonest deadline. Mark anything uncertain as "Verify in contract." This is an action list for the team, not a recommendation to renew or terminate.
```

---

## Legal Intake

### 16. Legal Request Intake Summary

**Use Case:** Turn an inbound business request into a structured legal intake for triage and routing.

**Target Personas:** Legal Operations, Corporate Counsel, Paralegal

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `intake`, `triage`

**Prompt:**

```
From the email/thread I reference, produce a structured legal intake:
- Requestor and business unit
- What they are asking legal to do
- Matter type (contract review, advice, dispute, policy, other)
- Deadline / urgency
- Counterparty and value (if relevant)
- Documents attached or referenced
- Missing information to request

Format as an intake record for routing. Do not assess the merits or provide an answer — this prepares the request for a lawyer to pick up.
```

---

## Stakeholder Communication

### 17. Plain-Language Clause Explainer

**Use Case:** Explain a contract clause or legal concept in plain language for a business stakeholder, with a clear caveat.

**Target Personas:** Corporate Counsel, Contracts Manager, Legal Operations

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `legal`, `plain-language`, `communication`

**Prompt:**

```
Explain the following clause/concept in plain language for a non-lawyer business stakeholder: [paste clause or name the concept]. Cover:
- What it means in practice
- Why it matters to the business
- What to watch for

Keep it neutral and general. End with: "This is a plain-language explanation for internal understanding, not legal advice. Confirm specifics with Legal." Do not tell the stakeholder what to decide.
```

---

## Negotiation Preparation

### 18. Negotiation History Brief

**Use Case:** Reconstruct the negotiation history of a contract for preparation. Analysis requires legal review.

**Target Personas:** Contracts Manager, Corporate Counsel, Commercial Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `contracts`, `negotiation`, `preparation`

**Prompt:**

```
Search my emails and documents for the negotiation history of [contract/counterparty]. Compile:
- Key issues raised by each party
- Positions and counter-positions over time
- Compromises reached
- Items still open at the last exchange

Format as preparation notes for the next session. This is research for preparation, not legal analysis or a negotiating recommendation.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
