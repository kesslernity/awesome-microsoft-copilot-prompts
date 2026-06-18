# Copilot for Trade Compliance

> Master Microsoft 365 Copilot for trade compliance — export controls, sanctions, and customs. Production-safe prompts for classification prep, screening prep, red-flag review, and licence prep — with strict guardrails. Copilot prepares; trade compliance classifies, screens, and decides.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Security & Compliance

**Prompts:** 16

---

## CRITICAL: TRADE COMPLIANCE GUARDRAILS - READ FIRST

### 1. Trade Compliance Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any trade-compliance use of Copilot. Export and sanctions decisions carry civil and criminal liability and are human.

**Target Personas:** Trade Compliance Manager, Export Control Officer, Sanctions Compliance Officer, Trade Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `export-controls`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Use Copilot for Trade Compliance

**Copilot prepares; it never classifies, screens, or clears. NEVER use it to:**

- Assign an export classification (ECCN, USML/ITAR category, dual-use, EU Annex I)
- Decide whether a party is a sanctions/restricted-party match or "clear" it
- Determine whether a licence is required, or which licence/exception applies
- Decide a country/embargo, end-use, or end-user is permitted
- Clear, approve, or release a shipment, transaction, or technology transfer
- Give a determination on customs/HS classification or origin

**Why it matters:** export-control and sanctions errors carry civil and criminal penalties. These are determinations for a qualified trade-compliance professional, made against current official sources.

**Screening note:** restricted/denied-party and sanctions screening must be run in your screening tool against current, official lists — never in a chat. Copilot does not have live lists and may be out of date.

**Jurisdiction:** rules differ (US EAR/ITAR/OFAC, EU dual-use, UK, others). Copilot does not know which apply.

**Golden Rule:**
> "Copilot prepares the file. Trade compliance classifies, screens, and decides."
```

---

## Classification

### 2. Export Classification Prep

**Use Case:** Assemble the product/technology facts needed to support a classification. Not the classification itself.

**Target Personas:** Export Control Officer, Trade Compliance Manager, Engineer (export liaison)

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `classification`, `export`

**Prompt:**

```
For [product/technology], gather from internal specs and emails the facts needed to support an export classification:
- Technical characteristics and performance parameters
- Function and intended use
- Materials/components and any controlled inputs mentioned
- Prior classifications or rulings referenced

Compile a classification worksheet with the facts and the open questions. Do NOT assign an ECCN, USML category, or dual-use status — that determination is made by the export control officer against current control lists.
```

---

### 3. Customs / HS Classification Prep

**Use Case:** Gather product information to support a customs/HS classification. Not the classification.

**Target Personas:** Customs Compliance, Trade Compliance Manager, Logistics

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `customs`, `hs-code`

**Prompt:**

```
For [product], compile from internal documents the details relevant to customs/HS classification:
- Composition, function, and form
- Intended use
- Any prior HS codes or rulings referenced

Present as a worksheet with facts and open questions. Do not assign an HS/tariff code or determine origin — those are classifications for customs compliance.
```

---

## Screening

### 4. Restricted / Denied Party Screening Prep

**Use Case:** Extract the parties to screen and build a screening checklist. Screening and the hit/clear call happen in the tool.

**Target Personas:** Trade Compliance Manager, Export Control Officer, Trade Ops

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `screening`, `restricted-party`

**Prompt:**

```
From this transaction/order, extract every party to be screened: [paste details — names, addresses, roles].
- List parties with full names, addresses, and roles (buyer, end-user, freight forwarder, bank, intermediaries)
- Note any missing identifying details to obtain

Output the screening list and checklist. Do NOT determine matches or clear anyone — restricted/denied-party and sanctions screening is run in the screening tool against current official lists, and the result is reviewed by trade compliance.
```

---

### 5. Sanctions Exposure Context

**Use Case:** Gather internal context on sanctions exposure to a counterparty or country. Flags, not a determination.

**Target Personas:** Sanctions Compliance Officer, Trade Compliance Manager, Trade Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `sanctions`, `context`

**Prompt:**

```
Search internal emails and documents for context on potential sanctions exposure involving [counterparty/country]:
- Dealings, intermediaries, or routes mentioned
- Ownership/control information referenced
- Concerns previously raised

Summarize as flags for review. This is NOT a sanctions determination — exposure (including 50%-rule ownership) must be assessed by sanctions compliance against current official sources.
```

---

## Due Diligence

### 6. Red Flag Indicators Review

**Use Case:** Apply standard export red-flag indicators to a transaction description. Flags for review, not findings.

**Target Personas:** Export Control Officer, Trade Compliance Manager, Sales (export liaison)

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `red-flags`, `due-diligence`

**Prompt:**

```
Review this transaction against standard export red-flag indicators (e.g., reluctance to give end-use info, mismatched capability, unusual routing/payment, freight forwarder as end-user, refusal of installation): [paste transaction details].
- List which indicators appear present, with the supporting detail
- Note information to obtain to resolve each

These are flags to investigate, not a finding. Trade compliance assesses and decides whether to proceed or hold.
```

---

### 7. End-Use / End-User Statement Prep

**Use Case:** Draft an end-use/end-user statement scaffold and due-diligence questions, for review.

**Target Personas:** Export Control Officer, Trade Compliance Manager, Sales

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `end-use`, `drafting`

**Prompt:**

```
Draft an end-use/end-user statement scaffold for [product] to [customer/country]: [context].
- Fields for end-user, end-use, location, and re-export intentions
- Due-diligence questions to ask the customer
- [TBC] where information is needed

Mark "DRAFT — for trade compliance review." This gathers and structures; it does not verify the end-use or clear the transaction.
```

---

## Licensing

### 8. Licence Determination Prep

**Use Case:** Organize the facts and questions needed for a licence determination. Not the determination.

**Target Personas:** Export Control Officer, Trade Compliance Manager, Trade Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `licensing`, `preparation`

**Prompt:**

```
For exporting [item] to [destination/end-user], organize what's needed for a licence determination:
- The facts on hand (classification status [from officer], destination, end-use, parties)
- The questions that drive whether a licence/exception applies
- Documents likely required

Present as a determination-prep worksheet. Do NOT conclude whether a licence is required or which exception applies — that is the export control officer's determination against current regulations.
```

---

### 9. Licence Application Draft Prep

**Use Case:** Assemble the information for an export licence application, for the officer to review and file.

**Target Personas:** Export Control Officer, Trade Compliance Manager, Trade Ops

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `licensing`, `application`

**Prompt:**

```
Assemble the information for a licence application for [item/transaction] from the inputs I provide:
- Parties, item, classification [from officer], destination, end-use, value, quantity
- Supporting documents on file
- [TBC] for anything missing

Compile a draft application pack. Mark "DRAFT — for export control officer review and filing." Do not submit or assert approvability.
```

---

## Country & Programme

### 10. Country / Embargo Profile Research

**Use Case:** Gather internal context on a destination. Always confirm against current official sanctions/embargo sources.

**Target Personas:** Trade Compliance Manager, Sanctions Compliance Officer, Trade Counsel

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `country`, `research`

**Prompt:**

```
For [country/destination], gather internal context relevant to trade:
- Prior dealings and any restrictions discussed
- Routes, partners, or licences referenced
- Concerns raised

Summarize as background. Mark "Confirm against current official sanctions/embargo and country-policy sources." Copilot does not hold live restrictions and must not be relied on for the current status.
```

---

### 11. Technology Control Plan (TCP) Draft

**Use Case:** Draft a Technology Control Plan scaffold to manage access to controlled technology, for review.

**Target Personas:** Export Control Officer, Trade Compliance Manager, Facility Security

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `tcp`, `controlled-technology`

**Prompt:**

```
Draft a Technology Control Plan scaffold for [project/controlled technology] from the inputs I provide:
- Controlled items/technology in scope [classification from officer]
- Who needs access and their nationality/status considerations [TBC]
- Physical and IT access controls to consider
- Training and recordkeeping

Mark "DRAFT — for export control officer review." Do not make nationality/eligibility or deemed-export determinations.
```

---

## Operations

### 12. Shipment Compliance Checklist Draft

**Use Case:** Draft a pre-export compliance checklist for a shipment. Release is a human decision.

**Target Personas:** Trade Ops, Export Control Officer, Logistics Compliance

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `shipment`, `checklist`

**Prompt:**

```
Draft a pre-export compliance checklist for [shipment/order] from our process: classification confirmed [officer], parties screened [tool], licence/exception in place if needed [officer], EUS obtained, documentation complete, embargo check. For each item, leave a confirmed-by/date field. This is a checklist to work through — it does not release the shipment; release follows sign-off by trade compliance.
```

---

### 13. Trade Compliance Audit Prep

**Use Case:** Assemble context and evidence pointers for a trade-compliance audit. Responses require sign-off.

**Target Personas:** Trade Compliance Manager, Export Control Officer, Internal Audit Liaison

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `audit`, `preparation`

**Prompt:**

```
For the trade-compliance audit on [scope], gather:
- Relevant procedures and records locations
- Prior findings and corrective actions
- Sample transactions referenced
- Open issues

Draft a response outline with evidence pointers. Responses must be reviewed and signed off by trade compliance/counsel before going to auditors or regulators.
```

---

## Governance

### 14. Trade Compliance Training Content Draft

**Use Case:** Draft trade-compliance awareness content for staff, for review.

**Target Personas:** Trade Compliance Manager, Export Control Officer, L&D

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `training`, `awareness`

**Prompt:**

```
Draft trade-compliance awareness content on [topic, e.g., recognizing export red flags] for [audience]. Practical do's and don'ts, short scenarios, and who to contact. Plain language. Mark "DRAFT — for trade compliance review." Keep examples generic and current rules to be confirmed by the team.
```

---

### 15. Trade Compliance Policy / Procedure Explainer

**Use Case:** Turn a trade-compliance policy into a plain-language explainer for staff, for review.

**Target Personas:** Trade Compliance Manager, Internal Comms, Export Control Officer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `policy`, `communication`

**Prompt:**

```
From this trade-compliance policy/procedure, draft a plain-language explainer for staff: [paste or reference]. Cover what it means in practice and when to involve trade compliance. Mark "DRAFT — trade compliance to review for accuracy." Route edge cases to the team rather than interpreting the rules.
```

---

## Incidents

### 16. Voluntary Disclosure / Incident Context Prep

**Use Case:** Organize the facts of a potential trade-compliance incident. The disclosure decision is counsel's.

**Target Personas:** Trade Compliance Manager, Trade Counsel, Export Control Officer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `trade-compliance`, `incident`, `disclosure`

**Prompt:**

```
For the potential trade-compliance issue described here, organize the facts: [what happened, when, items/parties/destinations involved].
- Timeline of events
- What appears to have occurred (factual)
- Items, classifications [from officer], parties, destinations involved
- Containment/remediation taken
- Open questions

Structure only. Whether to make a voluntary self-disclosure, to whom, and when is decided by trade counsel/compliance — Copilot does not advise on or decide disclosure.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
