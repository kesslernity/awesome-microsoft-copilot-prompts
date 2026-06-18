# Copilot for Finance

> Master Microsoft 365 Copilot for finance roles — FP&A, controllers, treasury, AP/AR, and CFOs. Production-safe prompts for close prep, variance stories, reporting, and reviews — with strict guardrails. Copilot gathers and drafts; finance verifies and decides.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint, Excel). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Finance & Analytics

**Prompts:** 16

---

## CRITICAL: FINANCE GUARDRAILS - READ FIRST

### 1. Finance Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any finance use of Copilot. Numbers it produces are drafts to verify, never authoritative.

**Target Personas:** CFO, Finance Manager, Controller, FP&A Lead, Treasury Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Use Copilot for Finance

**Copilot output is a draft to verify, never an authoritative figure or approval. NEVER use it for:**

- Authoritative financial calculations or the numbers in filed/published results
- Budget, spend, or payment approval or authorization
- Finalizing forecasts, accruals, or provisions
- Signing off accounts, reconciliations, or controls
- Tax, audit, or accounting-treatment determinations
- Investment or credit decisions

**Always verify every figure against the system of record (ERP/GL).** Copilot does not connect to your ERP, consolidation, or treasury systems; numbers it summarizes from emails or documents may be stale or wrong.

**Golden Rule:**
> "Copilot gathers and drafts. Finance verifies and decides."

No AI output replaces professional review and the controls in your close.
```

---

## Month-End Close

### 2. Month-End Close Prep

**Use Case:** Pull together the context and open items for the close from communications.

**Target Personas:** Controller, Finance Manager, Accountant

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `close`, `preparation`

**Prompt:**

```
For the [month] close, search emails and Teams for:
- Open items and pending journal entries mentioned
- Accruals or provisions being discussed
- Late information or blockers from other teams
- Anything flagged as a risk to the timetable

Compile a close-prep checklist. Figures must be confirmed in the GL — this is coordination, not the numbers.
```

---

## Variance Analysis

### 3. Variance Story Draft

**Use Case:** Draft the narrative behind a variance from context you provide. Confirm drivers with the business.

**Target Personas:** FP&A Lead, Finance Business Partner, Controller

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `variance`, `fpa`

**Prompt:**

```
I have a [favourable/adverse] variance of [amount] in [cost line / area]. From the emails and notes I provide, draft a plain-language explanation:
- The likely drivers discussed
- One-off vs recurring
- What the business said about cause

Mark drivers as "to confirm with [owner]". This is a narrative draft; the figures and root cause require your verification.
```

---

### 4. Budget vs Actual Summary

**Use Case:** Summarize budget-vs-actual discussion for a review. Authoritative figures come from the GL/EPM.

**Target Personas:** FP&A Lead, Finance Manager, Budget Owner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `budget`, `reporting`

**Prompt:**

```
For [cost centre / project], gather from emails and documents:
- Where spend is running vs budget (as discussed)
- Reasons given for over/underspend
- Reforecast or reallocation requests
- Approvals pending

Summarize for my review. Reconcile every figure to the GL before use.
```

---

## Reporting

### 5. Executive Financial Pre-Read

**Use Case:** Assemble a pre-read for a finance review or leadership meeting from existing material.

**Target Personas:** CFO, Finance Manager, FP&A Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `pre-read`, `executive`

**Prompt:**

```
Prepare a one-page pre-read for the [meeting] from recent reports, emails and decks:
- Headline results (as reported, cite source)
- Key movements and why
- Risks and decisions needed
- Open actions from last time

Keep figures sourced and flag any not yet confirmed.
```

---

### 6. Financial Narrative / Commentary Draft

**Use Case:** Draft management commentary (MD&A style) from results and notes, for review.

**Target Personas:** Controller, FP&A Lead, CFO

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `commentary`, `reporting`

**Prompt:**

```
Draft management commentary for [period/entity] from the results and notes I provide:
- Performance vs prior period and budget
- Drivers of the main movements
- Outlook points raised internally

Plain, factual, no spin. Every number traces to the input; mark anything unconfirmed [verify]. Draft for review.
```

---

### 7. Board Finance Pack Prep

**Use Case:** Gather and structure inputs for a board finance pack. Numbers stay subject to verification.

**Target Personas:** CFO, Finance Manager, FP&A Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `board`, `reporting`

**Prompt:**

```
For the board finance pack, pull together from existing reports and emails:
- Results summary and KPIs (sourced)
- Cash and liquidity points discussed
- Risks, covenants, or funding items raised
- Decisions or approvals being sought

Structure as draft sections for my review. Confirm all figures against the system of record.
```

---

## Audit & Controls

### 8. Audit Request Response Prep

**Use Case:** Assemble context and evidence pointers for an audit request. Responses require finance sign-off.

**Target Personas:** Controller, Finance Manager, Internal Audit Liaison

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `audit`, `preparation`

**Prompt:**

```
For the audit request on [topic], search for:
- Relevant policies and process notes
- Prior responses on similar items
- Where supporting evidence is likely held
- Any open issues previously raised

Draft a response outline with evidence pointers. The response must be reviewed and signed off by finance before it goes to the auditors.
```

---

## Accounts & Cash

### 9. AR / Collections Context

**Use Case:** Compile collections context for an overdue account to prepare a follow-up.

**Target Personas:** Credit Controller, AR Manager, Finance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `ar`, `collections`

**Prompt:**

```
For [customer/account], search emails for the collections history:
- Invoices and amounts referenced
- Promises to pay and dates
- Disputes or queries raised
- Last contact and outcome

Summarize to prepare my follow-up. Confirm balances in the ledger.
```

---

### 10. AP / Invoice Query Research

**Use Case:** Research an accounts-payable query from correspondence to resolve it faster.

**Target Personas:** AP Manager, Accountant, Finance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `ap`, `invoices`

**Prompt:**

```
For the invoice/PO query [reference] with [vendor], search emails for:
- What was ordered and agreed
- Approvals or goods-receipt confirmations mentioned
- The nature of the discrepancy
- Prior resolution of similar queries

Summarize to help resolve. Do not authorize payment — that follows your approval workflow.
```

---

### 11. Cash Flow Briefing Prep

**Use Case:** Gather cash and liquidity talking points for a treasury or leadership briefing.

**Target Personas:** Treasury Manager, CFO, Finance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `treasury`, `cash`

**Prompt:**

```
For my cash/liquidity briefing, gather from emails and reports:
- Large receipts/payments expected (as discussed)
- Funding, facility, or covenant points raised
- FX or rate concerns mentioned
- Any cash risks flagged

Compile as talking points. Actual cash positions come from treasury/bank systems — confirm before reporting.
```

---

## Planning

### 12. FP&A Assumptions Log

**Use Case:** Capture the assumptions behind a forecast or budget from discussion, for transparency.

**Target Personas:** FP&A Lead, Finance Business Partner, Controller

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `fpa`, `assumptions`

**Prompt:**

```
For the [forecast/budget], extract from emails and meeting notes the assumptions discussed:
- Assumption
- Owner / source
- Status (agreed / open / disputed)
- Sensitivity mentioned

Compile an assumptions log for review. Do not invent assumptions; flag gaps.
```

---

### 13. Forecast Input Gathering

**Use Case:** Collect the inputs needed for a reforecast from across the business.

**Target Personas:** FP&A Lead, Finance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `forecast`, `fpa`

**Prompt:**

```
For the [Q/period] reforecast, search emails and Teams for inputs already shared:
- Revenue/pipeline signals from sales
- Cost or headcount changes from departments
- Project timing changes
- Risks and opportunities raised

Summarize by area with the source. Mark anything still outstanding to chase.
```

---

## Cost & Investment

### 14. Cost Centre Review Prep

**Use Case:** Prepare for a cost-centre or department spend review with relevant context.

**Target Personas:** Finance Business Partner, FP&A Lead, Budget Owner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `cost`, `review`

**Prompt:**

```
For my spend review with [department/cost centre], gather:
- Spend topics raised in recent emails
- Commitments or new requests mentioned
- Prior actions and whether they closed
- Questions the owner is likely to raise

Prepare briefing notes. Confirm actuals in the GL before the meeting.
```

---

### 15. Capex / Investment Justification Draft

**Use Case:** Draft the justification narrative for a capex or investment request, for review.

**Target Personas:** Finance Manager, FP&A Lead, Budget Owner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `capex`, `business-case`

**Prompt:**

```
Draft the justification for the [capex/investment] request from the inputs I provide:
- Need and options considered
- Costs and benefits stated (sourced)
- Risks and assumptions
- Payback / returns as provided

Mark figures [to validate]. This is a draft narrative; the numbers and the decision are not Copilot's.
```

---

## Vendor

### 16. Vendor Spend Summary

**Use Case:** Compile spend and contract context for a vendor ahead of a review or renewal.

**Target Personas:** Finance Manager, FP&A Lead, Procurement Finance

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `vendor`, `spend`

**Prompt:**

```
For [vendor], gather from emails and documents:
- Spend and invoices referenced
- Contract value and renewal dates mentioned
- Issues or disputes raised
- Savings or change discussions

Summarize for a vendor review. Confirm actual spend against the ledger.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
