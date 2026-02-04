# Copilot for Administrative & Executive Assistants

> Master Microsoft 365 Copilot for administrative and executive assistant roles. Contains [APPROVED] production-safe prompts for Executive Assistants, Office Managers, and Administrative Professionals with role-specific guardrails.

**Category:** Operations & Support

**Total Prompts:** 17

---

[← Back to Main Library](../../README.md)

---

### Board Support

#### 1. [APPROVED] Board Meeting Preparation

**Use Case:** Prepare comprehensive board meeting support materials.

**Target Personas:** Executive Assistant, Chief of Staff, Board Liaison

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `executive-assistant`, `board`, `preparation`

**Prompt:**

```
I am preparing for the upcoming board meeting. Search for:
- Topics discussed in recent leadership meetings
- Issues that may come up
- Updates from various departments
- Previous board meeting action items
- Documents that need to be prepared

Compile as board meeting prep checklist.
```

---

### Calendar Management

#### 1. [APPROVED] Calendar Conflict Analysis

**Use Case:** Analyze calendar for potential issues and optimization opportunities.

**Target Personas:** Executive Assistant, Administrative Assistant, Chief of Staff

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `executive-assistant`, `calendar`, `scheduling`

**Prompt:**

```
Review [Executive Name]'s calendar for [next week/date range]. Based on emails and meeting contexts:
- Identify scheduling conflicts or tight transitions
- Flag meetings that may need more time based on past patterns
- Note meetings that could potentially be delegated
- Identify prep time needed before key meetings
- Flag travel time requirements

Compile as calendar optimization suggestions.
```

---

### Communication Management

#### 1. [APPROVED] Correspondence Summary

**Use Case:** Create executive correspondence summaries for busy periods.

**Target Personas:** Executive Assistant, Chief of Staff, Senior Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `executive-assistant`, `email`, `summary`

**Prompt:**

```
Summarize communications that [Executive Name] needs to be aware of from the past [timeframe]:
- Urgent items requiring response
- Requests awaiting decision
- Updates from key stakeholders
- Items I can handle on their behalf
- FYI items for awareness

Prioritize by urgency and importance.
```

---

#### 2. [APPROVED] Response Draft on Behalf

**Use Case:** Draft executive responses maintaining their voice and style.

**Target Personas:** Executive Assistant, Chief of Staff, Personal Assistant

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `executive-assistant`, `email`, `draft`

**Prompt:**

```
Draft a response on behalf of [Executive Name] to [Recipient] regarding [Topic]. Based on:
- The original message
- Similar responses the executive has sent before
- The executive's communication style
- Our relationship with the recipient

Mark as "From the desk of..." or similar. I will have the executive review before sending.
```

---

### Document Management

#### 1. [APPROVED] Document Organization Summary

**Use Case:** Create document inventory from communications and file searches.

**Target Personas:** Administrative Assistant, Document Controller, Records Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `admin`, `documents`, `organization`

**Prompt:**

```
Search for documents related to [Project/Topic] in my emails and SharePoint. Create an inventory:
- Documents found and their locations
- Version or date information
- Owner/creator if known
- Related documents that should be grouped
- Gaps or missing documents based on discussions

This is for document organization.
```

---

### Event Management

#### 1. [APPROVED] Event Planning Summary

**Use Case:** Consolidate event planning communications into organized status.

**Target Personas:** Office Manager, Facilities Manager, Event Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `office-manager`, `event`, `planning`

**Prompt:**

```
You are assisting an office manager. Search for all discussions about the upcoming [Event Name]. Compile:
- Event details confirmed
- Vendor communications
- Budget discussions
- Attendee-related items
- Logistics arrangements
- Outstanding decisions needed
- Action items and owners

Format as event planning status summary.
```

---

### Expense Management

#### 1. [APPROVED] Expense Report Context

**Use Case:** Gather business context for expense report documentation.

**Target Personas:** Administrative Assistant, Executive Assistant, Office Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `admin`, `expense`, `documentation`

**Prompt:**

```
Search for communications about expenses for [Trip/Event/Project]. Find:
- Purpose and business justification discussed
- Attendees or participants mentioned
- Approval discussions
- Special circumstances noted

Compile as supporting context for expense report submission.
```

---

### Facilities Management

#### 1. [APPROVED] Facilities Issue Tracking

**Use Case:** Track facilities issues from communications for reporting.

**Target Personas:** Office Manager, Facilities Manager, Building Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `office-manager`, `facilities`, `tracking`

**Prompt:**

```
Search for discussions about facilities issues over the past month. Compile:
- Issues reported
- Resolution status
- Recurring problems
- Vendor involvement
- Cost implications mentioned
- Outstanding items

Format as facilities status report.
```

---

### Governance

#### 1. ⚠️ Administrative Copilot Guardrails

**Use Case:** Essential guardrails for administrative professionals using Copilot.

**Target Personas:** Executive Assistant, Office Manager, Administrative Assistant

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `administrative`

**Prompt:**

```
## When NOT to Use Copilot for Administrative Roles

**EXECUTIVE ASSISTANTS — NEVER use Copilot for:**
- Accessing executive's calendar without permission
- Sending emails as the executive without review
- Financial approvals or commitments
- Confidential HR matters
- Legal or contractual decisions
- Board-sensitive information sharing
- M&A or confidential deal information

**OFFICE MANAGERS — NEVER use Copilot for:**
- Budget approvals (use finance systems)
- Vendor contract signing
- Employee records access (use HRIS)
- Safety certifications
- Building access decisions
- Insurance or liability matters
- Emergency response (follow protocols)

**ADMINISTRATIVE PROFESSIONALS — NEVER use Copilot for:**
- Expense approval (use expense system)
- Confidential document distribution
- Personnel file access
- Policy interpretation (consult HR)
- Payment processing
- Contract execution
- Compliance certifications

**Confidentiality Warnings:**
- Be extremely careful with executive communications
- Never share confidential meeting content inappropriately
- Remember prompts may be logged
- Follow information classification policies
- Board and investor communications require extra care
- Personal executive information is off-limits

**Golden Rules:**
- EAs: "Copilot organizes — EAs orchestrate"
- Office Managers: "Copilot coordinates — office managers deliver"
- Admins: "Copilot assists — admins execute"

**System Integration Note:**
Copilot does NOT integrate with:
- HRIS (Workday, BambooHR)
- Expense systems (Concur, Expensify)
- Visitor management systems
- Building access systems
- Corporate card systems
```

---

### Internal Communication

#### 1. [APPROVED] Office Announcement Draft

**Use Case:** Create office announcements for staff communication.

**Target Personas:** Office Manager, Administrative Manager, HR Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `office-manager`, `announcement`, `communication`

**Prompt:**

```
Draft an office announcement about [Topic - e.g., policy change, office closure, new amenity]. Include:
- Clear headline
- Key information (what, when, why)
- Impact on staff
- Action required (if any)
- Who to contact with questions

Match our internal communication style. I will review before sending.
```

---

### Meeting Documentation

#### 1. [APPROVED] Meeting Minutes Draft

**Use Case:** Draft meeting minutes from notes and discussion context.

**Target Personas:** Administrative Assistant, Executive Assistant, Team Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `admin`, `meeting-minutes`, `documentation`

**Prompt:**

```
You are assisting an administrative professional. Based on the meeting about [Topic] with [Attendees], draft meeting minutes including:
- Attendees list
- Key discussion points
- Decisions made
- Action items with owners and due dates
- Next meeting date (if set)

Format professionally. I will review for accuracy before distributing.
```

---

### Meeting Support

#### 1. [APPROVED] Meeting Preparation Brief

**Use Case:** Prepare comprehensive meeting briefs for executives.

**Target Personas:** Executive Assistant, Chief of Staff, Senior Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `executive-assistant`, `meeting-prep`, `briefing`

**Prompt:**

```
You are assisting an executive assistant. [Executive Name] has a meeting with [Person/Company] tomorrow. Search for:
- Previous interactions and context
- Topics likely to be discussed
- Outstanding items or commitments
- Recent news or updates about the other party
- Documents that may be needed
- Any preparation notes from similar meetings

Compile as a briefing document for the executive.
```

---

### Onboarding Support

#### 1. [APPROVED] New Hire Setup Checklist

**Use Case:** Gather onboarding context to ensure complete new hire setup.

**Target Personas:** Office Manager, Administrative Manager, HR Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `office-manager`, `onboarding`, `checklist`

**Prompt:**

```
Search for onboarding-related communications for new hires. Compile a setup checklist covering:
- IT equipment needs mentioned
- Access requirements discussed
- Workspace arrangements
- Training scheduled
- Introduction meetings
- First week activities

Compare against our standard checklist for completeness.
```

---

### Process Documentation

#### 1. [EXPERIMENTAL] Process Documentation Draft

**Use Case:** Draft process documentation from observed patterns. Requires validation.

**Target Personas:** Administrative Assistant, Office Manager, Operations Coordinator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `admin`, `process`, `experimental`

**Prompt:**

```
Based on how we've handled [Process/Task Type] in the past, draft a process document including:
- Steps typically followed
- People involved
- Tools used
- Common variations
- Tips and tricks mentioned

This is a starting draft — requires validation with the team.

EXPERIMENTAL: May miss steps or include outdated practices. Always validate with process owners.
```

---

### Reporting

#### 1. [APPROVED] Report Compilation

**Use Case:** Gather report content from communications.

**Target Personas:** Administrative Assistant, Team Coordinator, Project Administrator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `admin`, `report`, `compilation`

**Prompt:**

```
I need to compile a [weekly/monthly] report for [Manager/Team]. Search for:
- Status updates from team members
- Completed tasks and milestones
- Ongoing projects status
- Issues or blockers reported
- Upcoming deadlines
- Metrics or KPIs mentioned

Compile into report draft format.
```

---

### Travel Management

#### 1. [APPROVED] Travel Itinerary Draft

**Use Case:** Create travel context briefs for executive trips.

**Target Personas:** Executive Assistant, Travel Coordinator, Administrative Assistant

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `executive-assistant`, `travel`, `itinerary`

**Prompt:**

```
Based on [Executive Name]'s upcoming trip to [Destination] for [Purpose], compile:
- Meeting schedule at destination
- Relevant contact information
- Background on people being met
- Time zone considerations
- Any dietary or preference notes from past trips
- Documents likely needed

Format as a travel brief. I will add flight/hotel details from booking system.
```

---

### Vendor Management

#### 1. [APPROVED] Vendor Communication Summary

**Use Case:** Gather vendor relationship context from communications.

**Target Personas:** Office Manager, Facilities Manager, Administrative Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `office-manager`, `vendor`, `management`

**Prompt:**

```
Search for correspondence with [Vendor Name] regarding [Service/Product]. Compile:
- Service issues discussed
- Contract terms mentioned
- Pricing discussions
- Satisfaction or complaints
- Upcoming renewals
- Alternative vendor discussions

I need this for vendor review meeting.
```

---

