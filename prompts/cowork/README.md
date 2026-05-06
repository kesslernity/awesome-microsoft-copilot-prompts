# Copilot Cowork — Agentic Workflow Prompts

> Production-ready prompts for Microsoft 365 Copilot Cowork. Cowork is the agentic execution layer inside M365 Copilot — you describe an outcome, Cowork plans the steps, searches across your Outlook, Teams, Calendar, and SharePoint, and executes the work with your approval at each action. These are not Copilot Chat prompts. They require Cowork access.

**REQUIRES:**
- Microsoft 365 Copilot licence
- Frontier program enrolment (Admin Center → Settings → Org Settings → Microsoft 365 Frontier)
- Anthropic models enabled as sub-processor in M365 Admin Center
- Access at: [m365.cloud.microsoft](https://m365.cloud.microsoft)

**NOT compatible with:** Copilot Chat, ChatGPT, Claude.ai, or any non-Cowork interface.

**Prompts:** 18

---

## How Cowork Prompts Differ from Chat Prompts

Copilot Chat prompts are task-focused: "Summarize this document." Cowork prompts are outcome-focused: "I need X done — find the relevant information, show me what you found, then produce the output." Cowork plans, executes, and reports. You steer and approve.

**The Delegation Brief format (use this structure for every Cowork prompt):**
1. **Goal** — the outcome you want
2. **Inputs** — which M365 sources to pull from (Outlook, Teams, Calendar, SharePoint)
3. **Output** — what to produce and in what format
4. **Boundaries** — what not to do, what needs your approval before action

**Scheduled prompts:** Cowork can run prompts on a recurring schedule (daily, weekly, monthly). After a prompt runs successfully, click the clock icon to set a schedule. **Maximum 5 scheduled prompts per user** — choose carefully.

---

## Cowork Guardrails

### 1. What Cowork Should Never Do Without Your Approval

**Use Case:** Understand Cowork's approval model before delegating any action that affects others.

**Target Personas:** All M365 Copilot users with Frontier access

**Tags:** `cowork`, `frontier`, `guardrails`, `governance`, `agentic`

**Prompt:**
```
Before you take any of the following actions, stop and show me exactly what you are about to do, with full details, and wait for my explicit approval:
- Send any email
- Post any message to Teams
- Create or modify any calendar event
- Share or edit any SharePoint or OneDrive file
- Schedule any meeting or invite any attendee

For everything else — searching, reading, drafting, summarising — proceed without asking.

When you show me something for approval, include:
- The exact content (full email text, full Teams message, full event details)
- Who it is going to
- What action you will take after I approve

Do not use "Approve All" for multi-action sequences unless I explicitly ask you to.
```

**Schedulable:** No
**Skills used:** All
**Approval required:** Foundational prompt — set this expectation before any action-taking workflow

---

## Scheduled / Recurring Prompts

Use these for recurring work. Run once, verify the output, then schedule via the clock icon. Remember: 5-prompt limit per user — treat these as high-value slots.

### 2. Monday Week-Start Briefing

**Use Case:** Start every week with a clear picture of what needs your attention — open threads, commitments, calendar priorities.

**Target Personas:** Manager, Project Manager, Executive, Individual Contributor

**Tags:** `cowork`, `frontier`, `weekly`, `briefing`, `schedulable`, `outlook`, `teams`, `calendar`

**Prompt:**
```
Every Monday at 7:00 AM, prepare my week-start briefing. Search my emails and Teams messages from the last 7 days and my calendar for this week. Produce:
- Unresolved email threads I have not replied to — list each with sender, subject, and age, sorted oldest first
- Commitments I made to others in the last 7 days that I have not followed up on — list each with the date I made it and who I made it to
- Meetings this week that need preparation — for each one, include key context from my past exchanges with those attendees
- One thing I should proactively reach out about this week based on what you found

Format as a briefing I can read in under 3 minutes. Do not send or post anything — deliver this as a message to me only.
```

**Schedulable:** Yes — Monday 7:00 AM
**Skills used:** Email, Meetings, Calendar Management, Daily Briefing
**Approval required:** No (read-only output)

---

### 3. Friday End-of-Week Digest

**Use Case:** Close the week with a record of what was done, what's open, and what carries into next week.

**Target Personas:** Manager, Project Manager, Individual Contributor

**Tags:** `cowork`, `frontier`, `weekly`, `digest`, `schedulable`, `outlook`, `teams`

**Prompt:**
```
Every Friday at 4:30 PM, prepare my end-of-week digest. Search my emails, Teams messages, and calendar from the past 5 days. Produce:
- Decisions made this week — who owns each one
- Commitments others made to me that have not been delivered — list each with the date and who made it
- Items I committed to that are still open — list each with the due date if mentioned
- What I should address first thing Monday morning

Keep this under 150 words. Do not send or post anything — deliver as a message to me only.
```

**Schedulable:** Yes — Friday 4:30 PM
**Skills used:** Email, Teams, Calendar Management
**Approval required:** No (read-only output)

---

### 4. Daily Inbox Priority Scan

**Use Case:** Surface the 3–5 emails that actually need your attention today without reading everything.

**Target Personas:** Manager, Executive, Anyone with a high-volume inbox

**Tags:** `cowork`, `frontier`, `daily`, `inbox`, `schedulable`, `outlook`

**Prompt:**
```
Every weekday at 8:30 AM, scan my Outlook inbox for emails received in the last 24 hours. Identify the 3–5 that most need my attention today based on:
- Explicit requests directed at me that have not been answered
- Deadlines or time-sensitive items mentioned
- Senior stakeholders or external contacts waiting on a response
- Threads where I was the last to speak more than 48 hours ago

For each one, give me: sender, subject, one-sentence summary of what they need, and suggested action (reply, delegate, defer). Do not send anything — deliver as a list to me only.
```

**Schedulable:** Yes — weekdays 8:30 AM
**Skills used:** Email
**Approval required:** No (read-only output)

---

### 5. Weekly Commitment Tracker

**Use Case:** Automatically surface every promise you made across email and Teams before it becomes a missed deadline.

**Target Personas:** Project Manager, Account Manager, Consultant, Anyone managing multiple stakeholders

**Tags:** `cowork`, `frontier`, `weekly`, `commitments`, `schedulable`, `outlook`, `teams`

**Prompt:**
```
Every Wednesday at 9:00 AM, search my emails and Teams messages from the last 14 days. Find every instance where I committed to doing something — including phrases like "I will", "I'll send", "I'll follow up", "I'll check", "let me get back to you", "I'll have this to you by". For each commitment found:
- Who I made it to
- What I committed to
- When I committed to it
- Whether there is any evidence I followed through

Sort by age — oldest first. Flag any that are more than 5 days old with no follow-up. Do not send or post anything — deliver as a list to me only.
```

**Schedulable:** Yes — Wednesday 9:00 AM
**Skills used:** Email, Teams
**Approval required:** No (read-only output)

---

## Meeting & Stakeholder Prep

### 6. Pre-Meeting Research Brief

**Use Case:** Walk into any meeting fully prepared — know what was last discussed, what's open, and what they're likely to raise.

**Target Personas:** Account Manager, Project Manager, Executive, Consultant

**Tags:** `cowork`, `frontier`, `meeting-prep`, `outlook`, `teams`, `calendar`

**Prompt:**
```
I have a meeting with [Name] at [Company/Team] coming up. Search all my emails, Teams messages, and meeting notes involving them from the last 90 days. Produce a pre-meeting brief:
- The last 3 topics we discussed — newest first
- Any open items or commitments on either side — list each with the date it was raised
- The tone and direction of the last exchange — positive, tense, neutral, transactional
- One thing I should bring up proactively based on what you found

Show me the source messages you are drawing from before writing the brief, so I can verify accuracy. Keep the final brief under 150 words. Do not send or post anything.
```

**Schedulable:** No (requires [Name] variable)
**Skills used:** Email, Meetings, Enterprise Search
**Approval required:** No (read-only output)

---

### 7. Stakeholder Update — Multi-Step

**Use Case:** Prepare a structured stakeholder update by letting Cowork find the relevant content first, then draft from verified sources.

**Target Personas:** Project Manager, Account Manager, Program Lead

**Tags:** `cowork`, `frontier`, `stakeholder`, `agentic`, `outlook`, `teams`

**Prompt:**
```
I need to prepare a stakeholder update for [project or initiative name]. Do the following in sequence:

Step 1: Search my emails and Teams from the last 2 weeks for any updates, blockers, or decisions related to this project. Show me what you found — the actual message subjects, senders, and key content — before moving to Step 2.

Step 2: From what you found, identify the 3 most important developments to highlight.

Step 3: Draft a 5-bullet stakeholder update in this format:
- What happened (the facts)
- What is next (next actions and owner)
- What needs a decision (anything blocked waiting on someone)
- Key risks or concerns
- Suggested subject line for the email

Do not send anything. Present the draft for my review.
```

**Schedulable:** No (requires project name variable)
**Skills used:** Email, Teams, Communications
**Approval required:** Yes — review draft before sending

---

### 8. Post-Meeting Action Capture

**Use Case:** Immediately after a meeting, convert notes and transcript into assigned tasks and a recap email — without doing it manually.

**Target Personas:** Project Manager, Team Lead, Consultant, Executive Assistant

**Tags:** `cowork`, `frontier`, `meeting-follow-up`, `teams`, `outlook`

**Prompt:**
```
I just finished a meeting with [attendees/team]. Search for the Teams meeting transcript or my notes from the last 2 hours. Produce:

1. A structured list of action items — each with: what needs to be done, who owns it, and any deadline mentioned
2. A recap email draft to all attendees with: key decisions made, action items with owners, open questions, and next meeting date if mentioned

Show me the action item list first. After I confirm it is accurate, show me the email draft. Do not send the email until I explicitly approve it and confirm the recipient list.
```

**Schedulable:** No
**Skills used:** Email, Meetings, Communications
**Approval required:** Yes — email send requires explicit approval

---

### 9. Executive Pre-Read

**Use Case:** Before meeting with a senior stakeholder or exec, get a concise picture of the relationship, recent context, and what they care about.

**Target Personas:** Account Manager, Business Developer, Project Manager, Consultant

**Tags:** `cowork`, `frontier`, `executive`, `meeting-prep`, `outlook`, `teams`

**Prompt:**
```
I am meeting with [Name], [Title], at [Organisation] on [date]. Search my emails, Teams messages, and calendar entries involving them or their organisation from the last 6 months. Produce an executive pre-read:
- Last 3 topics or decisions involving them — what was the outcome of each
- Any open asks, commitments, or concerns on either side
- What they have said they care about or are focused on — use their exact words where possible, not paraphrases
- Any signals about priorities, pressures, or agenda items for this meeting

Keep this under 200 words. Do not send or post anything.
```

**Schedulable:** No
**Skills used:** Email, Meetings, Enterprise Search
**Approval required:** No (read-only output)

---

## Project & Portfolio Management

### 10. Project Status Digest — Across All Active Projects

**Use Case:** Get a cross-project status overview by letting Cowork sweep all recent communications rather than chasing each project lead.

**Target Personas:** PMO Director, Program Manager, Portfolio Lead

**Tags:** `cowork`, `frontier`, `project-management`, `portfolio`, `outlook`, `teams`

**Prompt:**
```
Search my emails and Teams messages from the last 7 days. Across all active projects I am involved in, identify and summarise:
- Projects where something notable happened — decision, blocker, escalation, or milestone
- Projects that have gone quiet — no communication in the last 5+ days
- Any deadline or milestone mentioned that falls within the next 14 days
- Any open risk or issue flagged but not yet resolved

Group by project. For each project use maximum 3 bullet points. Flag any project that needs my attention this week. Do not send or post anything.
```

**Schedulable:** Yes — Monday 8:00 AM
**Skills used:** Email, Teams, Enterprise Search
**Approval required:** No (read-only output)

---

### 11. Risk and Blocker Sweep

**Use Case:** Surface every risk, blocker, or escalation mentioned across your communications before it reaches you in a meeting.

**Target Personas:** Project Manager, Program Lead, PMO

**Tags:** `cowork`, `frontier`, `risk`, `blockers`, `outlook`, `teams`

**Prompt:**
```
Search my emails and Teams messages from the last 10 days. Find every instance where someone raised a risk, blocker, issue, delay, concern, or escalation — including phrases like "at risk", "blocked", "delayed", "concerned about", "issue with", "problem", "stuck", "waiting on". For each one:
- What is the risk or blocker
- Who raised it and when
- What project or workstream it relates to
- Whether there is any evidence it has been resolved

Sort by date — most recent first. Do not infer — only surface items explicitly stated in the communications. Do not send or post anything.
```

**Schedulable:** Yes — Friday 3:00 PM
**Skills used:** Email, Teams
**Approval required:** No (read-only output)

---

## Document Generation

### 12. Document from Meeting Notes

**Use Case:** Turn raw meeting notes or a transcript into a finished Word document — briefing, MOM, or decision record.

**Target Personas:** Project Manager, Executive Assistant, Consultant, Analyst

**Tags:** `cowork`, `frontier`, `document`, `word`, `meeting-notes`

**Prompt:**
```
I am attaching my notes from [meeting name] on [date]. [Attach file]

Using these notes, create a Word document formatted as a Minutes of Meeting / Decision Record with:
- Meeting: name, date, attendees
- Context: one-paragraph summary of why this meeting was held
- Key decisions: each on its own line with the decision and who made it
- Action items: what needs to be done, who owns it, deadline if stated
- Open questions: items discussed but not resolved
- Next steps: agreed next meeting or follow-up date

Use formal but clear language. Do not invent content not in the notes — if something is unclear, flag it with [CLARIFY] rather than guessing. Save as a Word document and show me the draft before saving.
```

**Schedulable:** No
**Skills used:** Word, Meetings
**Approval required:** Yes — review before saving

---

### 13. Presentation from Brief

**Use Case:** Turn a written brief or set of bullet points into a structured PowerPoint deck.

**Target Personas:** Project Manager, Consultant, Executive, Sales

**Tags:** `cowork`, `frontier`, `powerpoint`, `presentation`, `document`

**Prompt:**
```
I am attaching a brief for [presentation name / audience]. [Attach file]

Using this brief, create a PowerPoint presentation with the following structure:
- Slide 1: Title and context (what this presentation is and why it matters)
- Slides 2–4: The three main points — one key message per slide, supporting evidence below
- Slide 5: Implications or recommendations
- Slide 6: Next steps and owner for each

Use clean, minimal formatting. Each slide should have a single headline that stands alone as a sentence — not a label. Speaker notes on every slide with the key point to make verbally. Show me an outline of the slides before building the deck so I can confirm the structure.
```

**Schedulable:** No
**Skills used:** PowerPoint
**Approval required:** Yes — confirm outline before deck is built

---

## Research & Analysis

### 14. Deep Research — Multi-Source Synthesis

**Use Case:** Compile a research brief from both internal M365 data and external sources on a specific topic, company, or technology.

**Target Personas:** Consultant, Analyst, Business Developer, Executive

**Tags:** `cowork`, `frontier`, `research`, `deep-research`, `enterprise-search`

**Prompt:**
```
I need a research brief on [topic, company, or technology]. Do the following in sequence:

Step 1: Search my emails, Teams, and SharePoint for any internal content we already have on this topic. Show me what you found before continuing.

Step 2: Search external sources for recent developments — focus on facts, announcements, and concrete data. No opinion pieces.

Step 3: Synthesise both into a research brief with:
- What we already know internally (from Step 1)
- What is new or has changed recently (from Step 2)
- The 3 most important things to understand about this topic right now
- Gaps — what we do not know that we should

Cite every source. Flag any claim you are not confident about with [VERIFY]. Do not send or post anything.
```

**Schedulable:** No (requires topic variable)
**Skills used:** Deep Research, Enterprise Search, Email, Teams
**Approval required:** No (read-only output)

---

### 15. Competitive Signal Sweep

**Use Case:** Find every mention of competitors or alternatives across your recent communications — before a renewal, pitch, or strategy review.

**Target Personas:** Account Manager, Sales, Business Developer, Strategy Lead

**Tags:** `cowork`, `frontier`, `competitive`, `research`, `outlook`, `teams`

**Prompt:**
```
Search my emails and Teams messages from the last 90 days. Find every mention of a competitor, alternative solution, or vendor comparison — including company names, product names, and phrases like "evaluating alternatives", "looking at other options", "comparing with", "also talking to". For each mention:
- What was said and by whom
- The date and context
- Whether it was raised by a customer, colleague, or external party
- Whether there is any follow-up or resolution in the thread

Do not infer — only surface explicit mentions. Do not send or post anything.
```

**Schedulable:** No
**Skills used:** Email, Teams, Enterprise Search
**Approval required:** No (read-only output)

---

### 16. New Colleague or Stakeholder Onboarding Brief

**Use Case:** Before working with someone new, quickly understand who they are based on your org's existing communications and their public profile.

**Target Personas:** Manager, Project Manager, Executive, Account Manager

**Tags:** `cowork`, `frontier`, `onboarding`, `stakeholder`, `research`

**Prompt:**
```
I am about to start working with [Name] who is joining [team/project/organisation]. Search my emails and Teams for any existing context about them — past exchanges, mentions by colleagues, or project history. Also search externally for their professional background.

Produce a brief covering:
- What we already know about them internally (roles, projects, interactions)
- Their professional background based on public sources
- Any relevant context I should know before our first meeting
- One question worth asking them to build rapport early

Keep this under 200 words. Do not send or post anything.
```

**Schedulable:** No
**Skills used:** Enterprise Search, Email, Teams, Deep Research
**Approval required:** No (read-only output)

---

## Calendar Management

### 17. Weekly Calendar Triage

**Use Case:** Delegate your weekly calendar review — surface conflicts, low-value meetings, and missing focus time — then approve changes.

**Target Personas:** Executive, Manager, Senior Individual Contributor

**Tags:** `cowork`, `frontier`, `calendar`, `time-management`, `schedulable`

**Prompt:**
```
Review my Outlook calendar for the next 7 days. Identify:
- Any scheduling conflicts — two or more events at the same time
- Meetings with no agenda or context in the invite that I own — list them so I can add context or cancel
- Days with no focus time (blocks of 90+ uninterrupted minutes) — suggest where to add focus blocks
- Any meeting I have accepted that appears low-value based on the invite content

For each issue you identify, propose a specific action: decline, reschedule, add focus block, or request agenda. Present all proposed changes for my approval before making any calendar modifications. Do not accept, decline, or reschedule anything without my explicit go-ahead for each item.
```

**Schedulable:** Yes — Sunday evening or Monday 6:30 AM (run before Monday briefing)
**Skills used:** Calendar Management, Scheduling
**Approval required:** Yes — all calendar changes require explicit approval

---

### 18. Recurring Meeting Preparation — Automated

**Use Case:** For a meeting that recurs every week or two, automatically pull the relevant context before each occurrence.

**Target Personas:** Project Manager, Team Lead, Account Manager

**Tags:** `cowork`, `frontier`, `meeting-prep`, `recurring`, `schedulable`, `outlook`, `teams`

**Prompt:**
```
Before every [meeting name, e.g. "GenAI Biweekly Review"] — which recurs on [day and time] — do the following automatically 30 minutes before it starts:

Search my emails and Teams for anything related to [topic/project] from the last 14 days. Produce:
- New developments since the last meeting
- Open items from previous meeting notes that are still unresolved
- Anything I should raise proactively today
- One question worth asking the group

Keep this under 100 words. Deliver as a message to me only. Do not send or post to any other recipient.
```

**Schedulable:** Yes — set to 30 minutes before each recurrence
**Skills used:** Email, Teams, Meetings, Calendar Management
**Approval required:** No (read-only output)

---

## Notes & Limitations

- **5 scheduled prompt limit** — treat each slot as a high-value decision. Recommended priority: Monday Briefing → Commitment Tracker → Calendar Triage → Project Digest → Daily Inbox Scan
- **Approval model** — Cowork shows a preview before sending emails, posting to Teams, or modifying calendar events. Always read the preview carefully — verify recipients, content, and timing before approving
- **Show sources first** — include "show me what you found before drafting" in any prompt where accuracy matters. Cowork will pause after the search phase and display source messages before writing
- **Attach files explicitly** — for document generation prompts, drag and drop the file rather than asking Cowork to find it from SharePoint (more reliable in current Frontier preview)
- **Custom skills** — for workflows you run frequently, save the prompt as a custom skill at `/Documents/Cowork/skills/` in OneDrive as a Markdown file. Up to 50 custom skills supported
- **EU tenants** — Cowork requires Anthropic models enabled. EU/EFTA tenants have Anthropic off by default — admin must enable separately in M365 Admin Center before Cowork is fully functional

---

*Prompts tested in Microsoft 365 Copilot Cowork (Frontier program, May 2026). Production use — review all outputs before sending or sharing.*

*Part of the [awesome-microsoft-copilot-prompts](https://github.com/kesslernity/awesome-microsoft-copilot-prompts) collection by [NerdyChefs.ai](https://www.nerdychefs.ai)*
