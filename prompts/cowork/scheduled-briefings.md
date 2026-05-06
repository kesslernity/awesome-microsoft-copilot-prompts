# Copilot Cowork — Scheduled Briefings & Guardrails

> Set-and-forget recurring workflows plus the foundational guardrail prompt every Cowork user should run first.

[← Back to Cowork Collection](README.md) | [← Back to Main Collection](../../README.md)

---

## Requirements

> **REQUIRES:** Microsoft 365 Copilot licence + Frontier program enrolment + Anthropic sub-processor enabled. See [README.md](README.md) for full setup details.

---

## Guardrails

### 1. What Cowork Should Never Do Without Your Approval

**Use Case:** Understand Cowork's approval model before delegating any action that affects others. Run this prompt first — it sets the expectation for every workflow that follows.

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

## Scheduled Briefings

Use these for recurring work. Run once, verify the output, then schedule via the clock icon. **Maximum 5 scheduled prompts per user** — treat each slot as a high-value decision.

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

## Scheduling Your 5 Slots — Priority Order

| Slot | Prompt | Schedule | Value |
|------|--------|----------|-------|
| 1 | Monday Week-Start Briefing | Mon 7:00 AM | Highest — sets the week |
| 2 | Weekly Commitment Tracker | Wed 9:00 AM | Catches missed promises mid-week |
| 3 | Weekly Calendar Triage | Sun evening or Mon 6:30 AM | Prevents the week from filling before you plan it |
| 4 | Project Status Digest | Mon 8:00 AM | Portfolio-level visibility |
| 5 | Daily Inbox Priority Scan | Weekdays 8:30 AM | Only add if inbox volume justifies it |

The Friday Digest is valuable but if you are already running the Monday Briefing, the two overlap — don't use both unless you have a genuine end-of-week reporting need.

---

*Part of the [Copilot Cowork collection](README.md) — [awesome-microsoft-copilot-prompts](https://github.com/kesslernity/awesome-microsoft-copilot-prompts) by [NerdyChefs.ai](https://www.nerdychefs.ai)*
