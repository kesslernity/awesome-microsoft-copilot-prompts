# Copilot for Data & Analytics

> Master Microsoft 365 Copilot for data analysts, BI analysts, and business analysts. Production-safe prompts for profiling, insight drafting, report requirements, and KPI definitions — with strict guardrails. Copilot explores and drafts; the analyst verifies and concludes.

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint, Excel). These prompts work with your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Finance & Analytics

**Prompts:** 16

---

## CRITICAL: DATA & ANALYTICS GUARDRAILS - READ FIRST

### 1. Data & Analytics Critical Guardrails - Read First

**Use Case:** CRITICAL: Read before any analytics use of Copilot. Its figures are drafts to verify, and its observations are leads to investigate.

**Target Personas:** Analytics Manager, Data Analyst, BI Analyst, Business Analyst, Data Scientist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `analytics`, `guardrails`, `critical`

**Prompt:**

```
## When NEVER to Trust Copilot Blindly for Analytics

**Copilot explores and drafts; it is never the source of truth. NEVER:**

- Treat its calculations or figures as authoritative — verify against the data/BI platform
- Treat an observed correlation as causation
- Treat a summary as a complete or representative analysis (it may miss rows, outliers, or context)
- Make a business decision on its output without analyst review
- Let it determine data quality, lineage, or a metric's official definition

**Data care:** do not paste sensitive, personal, or regulated data into prompts; respect classification and your AI policy. Prompts may be logged.

**Reproducibility:** the number that ships comes from a queryable, repeatable source — not a chat answer.

**Golden Rule:**
> "Copilot explores and drafts. The analyst verifies, reproduces, and concludes."
```

---

## Exploration

### 2. Dataset Profiling Prep

**Use Case:** Get a fast structural read of a dataset before analysis. Verify counts in the source.

**Target Personas:** Data Analyst, BI Analyst, Business Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `profiling`, `excel`

**Prompt:**

```
Profile the dataset I've opened/referenced. Summarize:
- Columns and apparent data types
- Row count and any obviously missing/blank fields
- Value ranges or categories per key column
- Anything that looks inconsistent (mixed formats, duplicates, outliers)

This is a first read to plan analysis — confirm counts and quality in the source system before relying on them.
```

---

### 3. Anomaly / Outlier Exploration

**Use Case:** Surface candidate anomalies to investigate. These are leads, not findings.

**Target Personas:** Data Analyst, BI Analyst, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `anomaly`, `exploration`

**Prompt:**

```
In this dataset, point me to candidate anomalies or outliers in [metric/column]:
- Values that look unusually high/low
- Sudden changes over time
- Categories behaving differently from the rest

List them as leads to investigate, with where to look. Do NOT conclude a cause — these are starting points for analysis.
```

---

### 4. Ad-hoc Analysis Plan

**Use Case:** Structure how to approach an analysis question before diving in.

**Target Personas:** Data Analyst, Business Analyst, Data Scientist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `analysis`, `planning`

**Prompt:**

```
I need to answer: [analysis question]. Help me plan the approach:
- The sub-questions to break it into
- Data needed and likely sources
- Comparisons/segments worth examining
- Pitfalls to watch (bias, confounders, small samples)

This is an analysis plan for me to execute and validate — not the analysis itself.
```

---

## Insight & Narrative

### 5. Data Story / Insight Draft

**Use Case:** Turn validated analysis into a clear narrative for stakeholders. Verify every figure first.

**Target Personas:** BI Analyst, Data Analyst, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `insight`, `narrative`

**Prompt:**

```
From the analysis/figures I provide (already validated), draft a stakeholder-ready narrative:
- The headline (what changed / what we found)
- Supporting points with the numbers
- Caveats and what it does not tell us
- Suggested next questions

Plain language, no overclaiming, correlation flagged as correlation. Every number traces to my input — do not invent or recompute.
```

---

### 6. Report Commentary Draft

**Use Case:** Draft the commentary around a recurring report's numbers, for review.

**Target Personas:** BI Analyst, Reporting Analyst, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `reporting`, `commentary`

**Prompt:**

```
For the [report/dashboard] figures I provide, draft commentary:
- What moved vs prior period and by how much (from my figures)
- Plausible drivers as discussed internally (mark "to confirm")
- What to watch next period

Factual and concise. Do not assert causes as fact; the figures are mine to verify against the BI tool.
```

---

### 7. Insight Readout / Presentation Outline

**Use Case:** Outline an analytics readout deck from your findings, for build-out.

**Target Personas:** Analytics Manager, Data Analyst, BI Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `presentation`, `readout`

**Prompt:**

```
Outline a readout deck for [audience] from these findings: [paste].
- One slide per key message (message as the title)
- The evidence/figure on each
- Caveats slide
- Recommended next steps (as options, not decisions)

Lead with the "so what". Draft outline for me to build and validate.
```

---

## Definitions & Documentation

### 8. KPI / Metric Definition Draft

**Use Case:** Draft clear KPI definitions and calculation logic, for governance review.

**Target Personas:** Analytics Manager, BI Analyst, Data Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `kpi`, `definitions`

**Prompt:**

```
Draft definitions for these KPIs: [list]. For each:
- Plain-language definition
- Calculation logic (numerator/denominator, filters, grain)
- Inclusions/exclusions and edge cases
- Owner and source [TBC]

Mark "DRAFT — for data governance review." The official definition is owned by governance, not set here.
```

---

### 9. Data Dictionary / Field Documentation Draft

**Use Case:** Turn a column list or schema into a data dictionary draft.

**Target Personas:** Data Analyst, Analytics Engineer, Business Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `dictionary`, `documentation`

**Prompt:**

```
From this column list / schema, draft a data dictionary: [paste].
- Field name
- Plain-language description
- Type and example value
- Notes / known caveats [TBC where unknown]

Draft for SME/owner review. Do not invent meanings for fields you cannot infer — mark them [TBC].
```

---

### 10. Excel Formula / Logic Explainer

**Use Case:** Explain what a formula or logic does, to document or debug it.

**Target Personas:** Business Analyst, Data Analyst, Finance Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `excel`, `formula`

**Prompt:**

```
Explain this formula/logic in plain language: [paste formula]. Cover:
- What it calculates, step by step
- The inputs it depends on
- Edge cases or errors it could produce

For understanding and documentation. Verify behaviour on real data before relying on it.
```

---

## Requirements & Intake

### 11. Report / Dashboard Requirements Builder

**Use Case:** Turn a stakeholder ask into a structured BI requirements spec, for sign-off.

**Target Personas:** BI Analyst, Business Analyst, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `bi`, `requirements`

**Prompt:**

```
From this stakeholder request, draft a report/dashboard requirements spec: [paste].
- Business question and decision it supports
- Metrics and dimensions needed
- Filters, grain, and refresh frequency
- Audience and access
- Data sources [TBC]

Mark gaps [TBC] and "DRAFT — confirm with the requester." This scopes the work; it does not commit a delivery date.
```

---

### 12. Stakeholder Data Request Triage

**Use Case:** Turn an inbound data request into a structured intake for prioritization.

**Target Personas:** Analytics Manager, Data Analyst, BI Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `intake`, `triage`

**Prompt:**

```
From the email/thread, produce a structured data request intake:
- Requester and the decision they're trying to make
- What they're asking for (metric/cut/report)
- Deadline / urgency
- Data likely involved
- Missing information to clarify

Format for triage. Do not promise effort or dates — that's prioritization.
```

---

## Quality & Segments

### 13. Data Quality Issue Summary

**Use Case:** Compile data-quality concerns from comms and docs to flag for review.

**Target Personas:** Data Analyst, Analytics Engineer, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `data-quality`, `summary`

**Prompt:**

```
Search emails and documents for data-quality issues raised about [dataset/domain]:
- Issues mentioned (missing, duplicate, mismatched, late)
- Impact described
- Owners or fixes discussed

Summarize as flags for the data team. This is not a data-quality assessment — it surfaces what's been reported for human triage.
```

---

### 14. Cohort / Segment Definition Draft

**Use Case:** Draft the logic for a cohort or segment, for analyst review.

**Target Personas:** Data Analyst, BI Analyst, Marketing Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `segmentation`, `cohort`

**Prompt:**

```
Draft the definition for the [cohort/segment] I describe: [paste].
- The inclusion/exclusion rules in plain language
- The fields/conditions it implies
- Edge cases to decide

Mark "DRAFT — validate against the data." Do not finalize numbers; this is the logic for me to implement and test.
```

---

### 15. Survey / Feedback Analysis Prep

**Use Case:** Theme open-text responses to prepare a human analysis. Keep responses anonymized.

**Target Personas:** Data Analyst, People Analytics, Business Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `survey`, `text-analysis`

**Prompt:**

```
Summarize the themes in these open-text responses: [paste].
- Top recurring themes (rough frequency)
- Notable verbatim examples (anonymized)
- Sentiment direction per theme

Neutral summary as input to human analysis. Do not over-quantify qualitative data or attribute responses to individuals.
```

---

## Visualization

### 16. Chart / Visual Recommendation

**Use Case:** Recommend appropriate visuals for a question and data shape. The analysis stays yours.

**Target Personas:** BI Analyst, Data Analyst, Business Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `data`, `visualization`, `charts`

**Prompt:**

```
I want to show [message/relationship] from data shaped like [describe columns/grain]. Recommend:
- 2-3 suitable chart types and when each works best
- What to put on each axis / encoding
- Pitfalls (truncated axes, dual axes, too many series)

This guides design — the underlying analysis and the numbers are mine to validate.
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1,565+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
