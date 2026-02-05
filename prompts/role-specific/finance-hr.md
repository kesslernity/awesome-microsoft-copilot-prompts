# Copilot for Finance & HR

> Master Microsoft 365 Copilot for finance, HR, and analytics roles. Contains production-safe prompts for Finance/FinOps, HR/Communications, and Data Office/Analytics professionals with role-specific guardrails.

---

> [!WARNING]
> **REQUIRES: Microsoft 365 Copilot** with full M365 integration (Outlook, Teams, SharePoint). These prompts access your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

---

**Category:** Finance & Analytics

**Prompts:** 18

---

## Finance & HR Copilot Guardrails

> [!CAUTION]
> **Essential guardrails for Finance, HR, and Analytics roles using Copilot. Read before using any prompts in this pack.**

### When NOT to Use Copilot for Finance, HR & Analytics

**FINANCE — NEVER use Copilot for:**
- Financial calculations
- Forecasts or projections
- Budget approvals
- Payment authorizations
- Audit evidence (use official systems)
- Tax calculations
- Financial sign-offs
- Investment decisions

**HR — NEVER use Copilot for:**
- Hiring or termination decisions
- Performance evaluations
- Compensation decisions
- Disciplinary actions
- Grievance handling
- Medical/disability accommodations
- Employee relations issues
- Processing confidential employee data

**ANALYTICS — NEVER use Copilot for:**
- Data analysis (use BI tools)
- Report generation
- Data validation
- ETL development
- Model building
- SQL writing
- Data security decisions
- Production code

### Confidentiality Warnings

- **NEVER** include employee names in HR prompts
- **NEVER** include sensitive financial figures in prompts
- Remember that prompts may be logged
- When in doubt, use direct channels

### Golden Rules

- **Finance:** "Copilot searches context — finance maintains accuracy"
- **HR:** "Copilot drafts — HR exercises judgment"
- **Analytics:** "Copilot finds context — analysts deliver insights"

### System Integration Note

Copilot does NOT integrate with:
- HRIS (Workday, SAP SuccessFactors)
- Financial systems (SAP, Oracle)
- BI platforms (Power BI, Tableau)
- Data warehouses

---

## Prompts

### Audit Support

### 1. Audit Support Research

**Use Case:** Gather context for audit preparation. Formal audit evidence must come from financial systems.

**Target Personas:** Finance Manager, Internal Auditor, Controller

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `audit`, `research`

**Prompt:**

```
Search for emails and documents related to [audit topic or transaction type]. Compile:
- Relevant correspondence
- Approvals discussed
- Supporting documentation mentioned
- Any concerns raised during processing

This is research to support audit preparation. Formal evidence must come from official systems.
```

---

### BI Development

### 2. Dashboard Feedback Summary

**Use Case:** Gather user feedback on dashboards and reports to prioritize improvements.

**Target Personas:** BI Developer, Data Analyst, Product Owner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `analytics`, `feedback`, `dashboard`

**Prompt:**

```
Search for emails providing feedback on [Dashboard/Report Name] over the past 3 months. Summarize:
- What users like
- Pain points mentioned
- Enhancement requests
- Questions about the data

This is input for dashboard improvement planning.
```

---

### Budgeting

### 3. Budget Variance Explanation Draft

**Use Case:** Draft variance explanations based on team discussions. Numbers must come from financial systems.

**Target Personas:** FP&A Analyst, Finance Manager, Business Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `budget`, `variance`

**Prompt:**

```
Based on recent emails discussing budget variances for [cost center/project], draft explanation notes covering:
- Variances mentioned
- Causes discussed by the team
- Corrective actions proposed

This is for drafting budget commentary. Actual figures come from the financial system.
```

---

### Data Governance

### 4. Governance Communication Draft

**Use Case:** Draft data governance communications while maintaining consistent organizational tone.

**Target Personas:** Data Governance Lead, CDO, Data Steward

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `analytics`, `governance`, `communication`

**Prompt:**

```
Draft a communication to [audience] about [data governance topic, e.g., "new data classification policy" or "metric standardization"]. Base on previous communications about similar topics in my emails.

Keep tone professional and clear. I will review and enhance before sending.
```

---

### 5. Data Definition Research

**Use Case:** Research metric definitions across the organization to ensure consistency.

**Target Personas:** Data Analyst, Data Steward, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `analytics`, `definitions`, `governance`

**Prompt:**

```
Find documentation or discussions in SharePoint and emails about the definition of [metric/KPI name]. Identify:
- How different teams define this metric
- Calculation methods mentioned
- Data sources referenced
- Any discrepancies discussed

I need this to ensure consistent metric definitions.
```

---

### Data Quality

### 6. Data Quality Issue Research

**Use Case:** Research data quality issues from communications to support improvement initiatives.

**Target Personas:** Data Steward, Data Engineer, Data Quality Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `analytics`, `data-quality`, `issues`

**Prompt:**

```
Find discussions about data quality issues in [system/data domain]. List:
- Issues that have been reported
- Root causes identified
- Resolutions implemented
- Ongoing concerns

I need this for data quality improvement planning.
```

---

### Employee Engagement

### 7. Engagement Theme Analysis

**Use Case:** Identify engagement themes from informal feedback. Always supplement with formal surveys.

**Target Personas:** HR Manager, Employee Experience, CHRO

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `engagement`, `experimental`

**Prompt:**

```
Review feedback in emails and Teams related to employee engagement or workplace culture over the past 6 months. Identify recurring themes:
- Positive sentiments
- Concerns raised
- Suggestions made

This is input for engagement planning — requires proper survey methodology.

EXPERIMENTAL: Email feedback may not be representative. Use proper employee survey tools for formal engagement measurement.
```

---

### FinOps

### 8. FinOps Cloud Cost Discussion Search

**Use Case:** Gather context on cloud cost discussions to prepare for FinOps reviews. Cost data comes from cloud platforms.

**Target Personas:** FinOps Practitioner, Cloud Architect, Finance Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finops`, `cloud-costs`, `optimization`

**Prompt:**

```
Search for emails and Teams discussions about cloud costs for [service/project]. Compile:
- Cost concerns raised
- Optimization suggestions mentioned
- Anomalies or unexpected charges discussed
- Actions taken or planned

This helps me prepare for the FinOps review. Actual cost data comes from cloud billing.
```

---

### Financial Review

### 9. Financial Review Preparation

**Use Case:** Enter financial reviews prepared with context on all recent discussions and concerns.

**Target Personas:** Finance Manager, FP&A Analyst, Controller

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `review`, `preparation`

**Prompt:**

```
You are assisting a finance professional. I have a financial review meeting for [Project/Business Unit] tomorrow. Based on recent correspondence:
- What financial concerns have been raised?
- Are there any budget variance discussions?
- What approvals are pending?
- Any cash flow or payment issues mentioned?

Prepare briefing notes for my preparation.
```

---

### HR Policy

### 10. Policy Research

**Use Case:** Quickly find relevant HR policies to answer employee inquiries. Always verify currency of policies.

**Target Personas:** HR Manager, HR Business Partner, HR Generalist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `policy`, `research`

**Prompt:**

```
You are assisting an HR professional. Search SharePoint for HR policies related to [topic, e.g., "remote work" or "leave of absence"]. List:
- Policy documents found
- Effective dates (if mentioned)
- Key provisions summarized

I need this to answer an employee inquiry. I will verify current policy version.
```

---

### Internal Communications

### 11. Internal Comms Feedback Summary

**Use Case:** Gather feedback on internal communications to improve future messaging.

**Target Personas:** Internal Communications, HR Manager, Corporate Affairs

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `feedback`, `communications`

**Prompt:**

```
Search emails for feedback on recent internal communications (newsletters, town halls, announcements). Identify:
- What employees liked
- Concerns or confusion raised
- Suggestions for improvement
- Topics they want to hear more about

This is research for communications improvement.
```

---

### 12. Internal Announcement Draft

**Use Case:** Draft internal announcements quickly while ensuring appropriate tone and completeness.

**Target Personas:** HR Manager, Internal Communications, Corporate Affairs

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `communications`, `announcement`

**Prompt:**

```
Draft an internal announcement about [topic, e.g., "office relocation" or "new benefit program"]. Based on similar announcements in my email history:
- Use an appropriate tone for company-wide communication
- Include key information points
- Mark placeholders for specific details I need to add

This is a draft for review before distribution.
```

---

### Learning & Development

### 13. Training Program Summary

**Use Case:** Gather training program context and feedback for program planning and improvement.

**Target Personas:** L&D Manager, Training Coordinator, HR Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `training`, `program`

**Prompt:**

```
Find information about [training program name] in emails and SharePoint. Summarize:
- Program objectives
- Content covered
- Feedback received
- Scheduling or logistics mentioned

This helps me prepare for training planning discussions.
```

---

### Month-End Close

### 14. Month-End Discussion Summary

**Use Case:** Prepare for month-end close meetings with context on all issues discussed. Close activities use ERP systems.

**Target Personas:** Finance Manager, Accountant, Controller

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `finance`, `month-end`, `close`

**Prompt:**

```
Summarize discussions from my emails and Teams over the past week related to month-end close for [period]. Include:
- Issues raised that may affect close
- Adjustments discussed
- Timing concerns
- Outstanding items mentioned

I need this to prepare for the close meeting. Actual close activities use our financial systems.
```

---

### Onboarding

### 15. Onboarding Checklist Research

**Use Case:** Compile existing onboarding materials to create comprehensive new hire packages.

**Target Personas:** HR Coordinator, HR Business Partner, Learning & Development

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `hr`, `onboarding`, `checklist`

**Prompt:**

```
Search for onboarding materials, checklists, and new hire communications for [department/role type]. Compile:
- Documents found and their locations
- Topics covered in onboarding
- Any feedback about onboarding mentioned in emails

I'm preparing an onboarding package and want to ensure completeness.
```

---

### Requirements

### 16. Requirements Gathering Summary

**Use Case:** Consolidate stakeholder requirements for data products from scattered communications.

**Target Personas:** Data Analyst, BI Developer, Analytics Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `analytics`, `requirements`, `stakeholder`

**Prompt:**

```
You are assisting a data analyst. Search my emails and Teams for discussions about requirements for [report/dashboard name]. Compile:
- What metrics stakeholders have requested
- Questions they want answered
- Filters or views mentioned
- Any complaints about current reports

This helps me understand stakeholder needs.
```

---

### Self-Service Analytics

### 17. Self-Service Analytics Support Research

**Use Case:** Identify common user struggles with self-service analytics to improve support and training.

**Target Personas:** BI Developer, Data Analyst, Analytics Support

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `analytics`, `self-service`, `experimental`

**Prompt:**

```
Search for emails where business users asked questions about accessing or using data in [Power BI/analytics platform]. Identify:
- Common questions asked
- Issues they faced
- Topics where training was requested

This is research for self-service analytics support improvement.

EXPERIMENTAL: May not capture all user struggles, especially those not communicated via email.
```

---

### Governance

### 18. Finance & HR Copilot Guardrails Reference

**Use Case:** Essential guardrails for Finance, HR, and Analytics roles using Copilot. Includes confidentiality warnings.

**Target Personas:** Finance Manager, HR Manager, Data Analyst, Controller

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `finance`, `hr`, `analytics`

**Prompt:**

```
## When NOT to Use Copilot for Finance, HR & Analytics

**FINANCE — NEVER use Copilot for:**
- Financial calculations
- Forecasts or projections
- Budget approvals
- Payment authorizations
- Audit evidence (use official systems)
- Tax calculations
- Financial sign-offs
- Investment decisions

**HR — NEVER use Copilot for:**
- Hiring or termination decisions
- Performance evaluations
- Compensation decisions
- Disciplinary actions
- Grievance handling
- Medical/disability accommodations
- Employee relations issues
- Processing confidential employee data

**ANALYTICS — NEVER use Copilot for:**
- Data analysis (use BI tools)
- Report generation
- Data validation
- ETL development
- Model building
- SQL writing
- Data security decisions
- Production code

**Confidentiality Warnings:**
- NEVER include employee names in HR prompts
- NEVER include sensitive financial figures in prompts
- Remember that prompts may be logged
- When in doubt, use direct channels

**Golden Rules:**
- Finance: "Copilot searches context — finance maintains accuracy"
- HR: "Copilot drafts — HR exercises judgment"
- Analytics: "Copilot finds context — analysts deliver insights"

**System Integration Note:**
Copilot does NOT integrate with:
- HRIS (Workday, SAP SuccessFactors)
- Financial systems (SAP, Oracle)
- BI platforms (Power BI, Tableau)
- Data warehouses
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1300+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
