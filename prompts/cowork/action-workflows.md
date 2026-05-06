# Copilot Cowork — Action-Taking Workflows

> These prompts do things Chat cannot. Chat drafts — Cowork executes. Every prompt here ends with Cowork taking an action (sending, scheduling, posting, creating) after showing you a full preview for approval.

[← Back to Cowork Collection](README.md) | [← Back to Main Collection](../../README.md)

---

## Requirements

> **REQUIRES:** Microsoft 365 Copilot licence + Frontier program enrolment + Anthropic sub-processor enabled. See [README.md](README.md) for full setup details.

---

## Why This Is Different

Both Copilot Chat and Cowork can search your emails, Teams messages, and SharePoint. That is not the difference.

The difference is what happens after the research. Chat produces a draft and stops. You have to copy it, open Outlook, paste it, check recipients, and send it yourself. Cowork can send the email, schedule the meeting, post to Teams, create the calendar block — with your explicit approval before each action.

Every prompt in this file completes an action. None of them stops at the draft.

---

## Action-Taking Prompts

### 19. Send Meeting Follow-Up Email

**Use Case:** After any meeting, automatically draft and send the recap email to all attendees — without doing it manually.

**Target Personas:** Project Manager, Account Manager, Consultant, Team Lead

**Tags:** `cowork`, `frontier`, `action`, `email`, `meeting-follow-up`, `outlook`, `teams`

**Prompt:**
```
I just finished a meeting with [attendees or team name]. Find the Teams transcript or my notes from the last 2 hours.

Step 1: Extract all action items (what, who owns it, deadline if mentioned), decisions made, and open questions. Show me this list and wait for my confirmation that it is accurate.

Step 2: Draft a follow-up email to all attendees with this structure:
- Subject: Follow-up: [meeting name] — [date]
- Action items with owners and deadlines
- Decisions made
- Open questions and who is responsible for answering them
- Next meeting date if discussed

Step 3: Show me the full draft and the complete recipient list. Wait for my explicit approval before sending.

Step 4: Send the email only after I approve.
```

**Schedulable:** No
**Skills used:** Email, Meetings, Teams, Communications
**Approval required:** Yes — full draft + recipient list shown before send

---

### 20. Schedule a Meeting Based on Calendar Availability

**Use Case:** Find a time that works for a group of people and send the calendar invite — without the back-and-forth.

**Target Personas:** Project Manager, Executive Assistant, Manager, Account Manager

**Tags:** `cowork`, `frontier`, `action`, `calendar`, `scheduling`, `outlook`

**Prompt:**
```
I need to schedule a [30/60]-minute meeting with [names or email addresses] about [topic]. The meeting should happen within the next [7/14] days, preferably [morning/afternoon], and not during lunch hours.

Step 1: Check my calendar and their calendars for available slots that work for everyone. Show me the top 3 options with day, time, and duration.

Step 2: After I select a slot, create a calendar invite with:
- Title: [meeting title]
- Attendees: [list]
- Teams meeting link included
- Agenda in the body: [I will describe the agenda or you propose one based on the topic]

Step 3: Show me the full invite details before sending. Do not send until I confirm.

Step 4: Send the invite.
```

**Schedulable:** No
**Skills used:** Calendar Management, Scheduling, Email
**Approval required:** Yes — slot selection + invite preview before sending

---

### 21. Post Weekly Project Update to Teams Channel

**Use Case:** Compile the week's project developments from email and Teams, then post a structured update to the team channel — without writing it from scratch.

**Target Personas:** Project Manager, Team Lead, Program Manager

**Tags:** `cowork`, `frontier`, `action`, `teams`, `project-management`, `schedulable`

**Prompt:**
```
Every Friday at 4:00 PM, prepare and post the weekly project update for [project name] to the [Teams channel name] channel.

Step 1: Search my emails and Teams messages from the last 7 days related to [project name]. Identify: what progressed, what is blocked, what was decided, what is due next week.

Step 2: Draft a Teams post in this format:
**Week ending [date] — [Project Name] Update**
✅ Done this week: [bullet points]
🔄 In progress: [bullet points]
🚫 Blocked: [bullet points — include who needs to act]
📅 Next week: [bullet points]

Step 3: Show me the draft and confirm the channel name. Wait for my approval.

Step 4: Post to the channel after I approve.
```

**Schedulable:** Yes — Friday 4:00 PM
**Skills used:** Email, Teams, Communications
**Approval required:** Yes — draft + channel confirmed before posting

---

### 22. Inbox Triage — Reply to Flagged Emails

**Use Case:** Surface the emails that need a reply today and draft responses — then send after your review, not before.

**Target Personas:** Manager, Executive, Account Manager, Anyone with high email volume

**Tags:** `cowork`, `frontier`, `action`, `email`, `inbox`, `outlook`

**Prompt:**
```
Scan my Outlook inbox for emails received in the last 48 hours that are waiting for a reply from me. Identify the ones where:
- Someone asked me a direct question
- Someone is waiting on a decision or approval from me
- A deadline or deliverable is mentioned that requires my response

For each one, draft a concise reply. Keep replies under 100 words unless the email requires a detailed response.

Show me each draft alongside the original email before sending anything. I will approve, edit, or reject each reply individually. Do not send any email without my explicit approval for that specific email.
```

**Schedulable:** No
**Skills used:** Email
**Approval required:** Yes — each reply approved individually before sending

---

### 23. Send Stakeholder Update After Approval

**Use Case:** Full end-to-end workflow — research, draft, get approval, send. The action-taking version of the Stakeholder Update from the research collection.

**Target Personas:** Project Manager, Account Manager, Program Lead

**Tags:** `cowork`, `frontier`, `action`, `email`, `stakeholder`, `outlook`, `teams`

**Prompt:**
```
I need to send a stakeholder update for [project name] to [recipient names or distribution group].

Step 1: Search my emails and Teams from the last 2 weeks for updates, decisions, and blockers related to this project. Show me the key threads you found.

Step 2: Draft a 5-bullet update email:
- What happened
- What is next and who owns it
- What needs a decision
- Risks or concerns
- Subject line suggestion

Step 3: Show me the full draft and the recipient list. Wait for my approval and any edits.

Step 4: Send the email after I approve. Confirm when sent.
```

**Schedulable:** No (requires project and recipient variables)
**Skills used:** Email, Teams, Communications
**Approval required:** Yes — full draft + recipient list before sending

---

### 24. Block Focus Time on Calendar This Week

**Use Case:** Find the gaps in your calendar and add focus blocks before your week fills up completely.

**Target Personas:** Manager, Individual Contributor, Executive, Anyone in back-to-back meetings

**Tags:** `cowork`, `frontier`, `action`, `calendar`, `time-management`, `schedulable`

**Prompt:**
```
Look at my calendar for the next 5 working days. Find any day that has less than 90 minutes of uninterrupted time between 8 AM and 6 PM.

For each such day, propose one focus block of [60/90/120] minutes placed in the largest available gap, avoiding early morning before 8 AM and lunch hours.

Show me the proposed blocks — day, start time, end time — before creating anything.

After I confirm, create the calendar events titled "Focus Time — [project or topic if I specify one]" and set them as Busy. Do not create any event until I approve the full list.
```

**Schedulable:** Yes — run Sunday evening or Monday 6:30 AM
**Skills used:** Calendar Management, Scheduling
**Approval required:** Yes — full list of blocks shown before any calendar event created

---

### 25. Reschedule Conflicts on My Calendar

**Use Case:** When your week has scheduling conflicts, let Cowork identify them and propose resolutions — then act after your approval.

**Target Personas:** Manager, Executive, Executive Assistant

**Tags:** `cowork`, `frontier`, `action`, `calendar`, `scheduling`, `outlook`

**Prompt:**
```
Scan my calendar for the next 7 days. Find every scheduling conflict — two or more events overlapping at the same time.

For each conflict:
- List the two events, their times, and attendees
- Identify which event I organised vs which I was invited to
- Propose a resolution: which one to reschedule and suggest 2 alternative slots based on my calendar availability

Show me all conflicts and your proposed resolutions before taking any action.

After I confirm each resolution, reschedule the relevant event and send updated calendar notifications to the affected attendees. Handle one conflict at a time — do not reschedule anything until I approve that specific change.
```

**Schedulable:** No
**Skills used:** Calendar Management, Scheduling, Email
**Approval required:** Yes — each conflict resolved individually with explicit approval

---

### 26. Draft and Send Renewal or Follow-Up Reminder

**Use Case:** For accounts approaching a renewal, contract review, or follow-up date — research the relationship, draft the outreach, and send after approval.

**Target Personas:** Account Manager, Sales, Customer Success

**Tags:** `cowork`, `frontier`, `action`, `email`, `renewal`, `account-management`, `outlook`

**Prompt:**
```
I need to send a renewal outreach email to [Contact Name] at [Company]. The renewal or follow-up date is [date].

Step 1: Search my emails and Teams from the last 6 months for all communications with [Contact Name]. Identify: what they care about, any concerns raised, value they acknowledged, any pricing or timing sensitivities mentioned.

Step 2: Draft a brief, direct email (under 150 words) that:
- References something specific from our recent history — not a generic opener
- States the purpose (renewal discussion / check-in)
- Proposes a specific next step (call, reply, meeting)
- Does not include pricing or contract terms

Step 3: Show me the draft. Wait for my approval and any edits.

Step 4: Send after I approve. Confirm when sent.
```

**Schedulable:** No (requires contact variables)
**Skills used:** Email, Enterprise Search, Communications
**Approval required:** Yes — draft reviewed before sending

---

### 27. Create and Share a Document with Stakeholders

**Use Case:** Generate a Word document from notes or a brief, then share it directly with the right people — without manually uploading and emailing.

**Target Personas:** Project Manager, Analyst, Consultant, Executive Assistant

**Tags:** `cowork`, `frontier`, `action`, `word`, `sharepoint`, `email`, `document`

**Prompt:**
```
I am attaching [notes / brief / source document]. [Attach file]

Step 1: Create a Word document from this content structured as [briefing / report / MOM / proposal — specify]. Include: title, date, key sections with headers, and a summary at the top.

Step 2: Show me the document before saving. Wait for my confirmation and any edits.

Step 3: After I approve the document, save it to [OneDrive folder name or SharePoint location].

Step 4: Draft a short email to [recipient names] with the document attached and a one-sentence description of what it is. Show me the email draft before sending.

Step 5: Send the email after I approve it.
```

**Schedulable:** No
**Skills used:** Word, Email, SharePoint/OneDrive
**Approval required:** Yes — document review before saving; email review before sending

---

### 28. End-to-End Weekly Status Report — Research, Draft, Send

**Use Case:** The full weekly status workflow: pull data across M365, compile the report, send it to your distribution list. Set it once, runs every week.

**Target Personas:** Project Manager, Program Lead, Team Lead

**Tags:** `cowork`, `frontier`, `action`, `email`, `weekly`, `schedulable`, `outlook`, `teams`

**Prompt:**
```
Every Friday at 3:30 PM, prepare and send the weekly status report for [project or team name] to [distribution list or email addresses].

Step 1: Search my emails and Teams from the last 7 days for updates related to [project or team name]. Identify: milestones reached, blockers, decisions, risks, and next week's priorities.

Step 2: Compile a status report email with:
- Subject: [Project Name] — Week of [date] Status Update
- This week: 3–5 bullet points
- Blockers: list with owner for each
- Next week: 3 priorities
- Risks: anything flagged in the last 7 days

Step 3: Show me the draft and the recipient list. Wait for my approval.

Step 4: Send the email after I approve. If I do not respond within 30 minutes of the draft being shown, do not send — hold it for my review.
```

**Schedulable:** Yes — Friday 3:30 PM
**Skills used:** Email, Teams, Communications
**Approval required:** Yes — draft + recipient list before sending; auto-hold if no response in 30 minutes

---

## Approval Model

Every prompt in this file requires at least one approval gate before Cowork takes action. The standard sequence is:

1. Cowork researches and drafts
2. Cowork shows you the full content + who it's going to
3. You approve (or edit, or reject)
4. Cowork executes

Never skip the preview step. "Approve All" for multi-action sequences should be used only when you have verified each action individually first.

---

*Part of the [Copilot Cowork collection](README.md) — [awesome-microsoft-copilot-prompts](https://github.com/kesslernity/awesome-microsoft-copilot-prompts) by [NerdyChefs.ai](https://www.nerdychefs.ai)*
