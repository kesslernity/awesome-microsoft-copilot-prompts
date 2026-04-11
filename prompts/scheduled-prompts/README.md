# Scheduled Prompts for Microsoft 365 Copilot

> 15 prompts designed to run automatically on a recurring schedule — daily briefings, weekly summaries, and pipeline reviews that run without you. Requires M365 Copilot paid license.

**Category:** Automation & Scheduled Workflows

**Prompts:** 15

**Roles:** All roles · Sales & BD · Project Management · Finance · HR · Executive

---

## What Are Scheduled Prompts?

Microsoft 365 Copilot lets you schedule any prompt to run automatically at a set day and time. The result saves to your Copilot conversation history. You can optionally receive a Teams or email notification when it finishes.

Scheduled prompts run against your Outlook email, calendar, and Teams data. They do not access SharePoint files, OneDrive documents, or Excel workbooks.

**Status:** Generally Available (GA) since January 2026  
**License required:** M365 Copilot paid add-on ($30/user/month) — not available on free Copilot Chat  
**Limit:** Up to 10 scheduled prompts per user

---

## How to Set Up a Scheduled Prompt

**4 steps, under 2 minutes:**

**Step 1 — Run the prompt once**  
Go to [m365.cloud.microsoft/chat](https://m365.cloud.microsoft/chat) or open Copilot in Microsoft Teams. Paste any prompt from this collection and send it. Let it run to completion.

**Step 2 — Open the schedule option**  
Hover over the prompt in your chat history. Select **Schedule this prompt**.

**Step 3 — Configure the schedule**  
Set your preferences:
- **Time** — e.g. every weekday at 08:00 (your local timezone)
- **Frequency** — Daily or Weekdays only
- **Notifications** — optional email when the result is ready

**Step 4 — Save**  
Click **Save**. The prompt is now active. Results appear in your Copilot chat history each time it runs.

**To manage or delete scheduled prompts:**  
Copilot Chat → click your profile or the settings icon → **Scheduled prompts**.

**Source:** [Microsoft Support — Schedule Copilot prompts](https://support.microsoft.com/en-us/topic/schedule-copilot-prompts-29dfd5fb-211a-4515-88a6-730b8074e489)

---

## Design Rules for Scheduled Prompts

These prompts are written for unattended execution. They follow four rules:

1. **Relative time windows** — "last 24 hours", "this week", "since Monday" — not "today's meeting" or "the email you sent me" which require context you won't provide at runtime.
2. **Self-contained output** — the result is useful without follow-up questions.
3. **Actionable format** — structured output (priority lists, tables, action items) not open-ended summaries.
4. **Scoped to available data** — Outlook email, calendar events, Teams messages only.

---

## Daily Productivity

### 1. Morning Email Briefing

**Use Case:** Start each day knowing what needs your attention before opening your inbox

**Recommended schedule:** Weekdays at 7:00 AM

**Target Personas:** All roles

**Tags:** `Scheduled`, `Outlook`, `Email`, `Daily`, `Productivity`

**Prompt:**

```
Summarise the emails I received in the last 18 hours. Group them into three categories:
1. Requires response today — list sender, subject, and one sentence on what they need
2. Requires action but no reply — list what the action is
3. FYI only — list in one line each

Flag anything marked urgent or with a deadline mentioned. Keep the whole summary under 200 words.
```

---

### 2. Daily Calendar Prep

**Use Case:** Know what today requires before the first meeting starts

**Recommended schedule:** Weekdays at 7:30 AM

**Target Personas:** Manager, Executive, Project Lead, EA

**Tags:** `Scheduled`, `Calendar`, `Meetings`, `Daily`, `Preparation`

**Prompt:**

```
List my meetings for today. For each meeting show:
- Time and duration
- Attendees (names only, not email addresses)
- One sentence on what the meeting is likely about based on the invite subject and any related emails from the last 3 days
- Any open action items from previous meetings with the same people

Flag any back-to-back blocks with no break.
```

---

### 3. End-of-Day Commitment Tracker

**Use Case:** Close the day knowing what you promised and to whom

**Recommended schedule:** Weekdays at 5:30 PM

**Target Personas:** Manager, Consultant, Project Lead, Sales

**Tags:** `Scheduled`, `Outlook`, `Teams`, `Accountability`, `Daily`

**Prompt:**

```
Review my emails and Teams messages from today. Extract every commitment I made — things I said I would do, send, or follow up on. For each one list:
- What I committed to
- Who I committed to
- Deadline if mentioned (or "no deadline stated")

List in priority order. Flag anything promised for tomorrow or sooner at the top.
```

---

## Sales & Business Development

### 4. Weekly Pipeline Pulse

**Use Case:** Start Monday knowing which deals need attention this week

**Recommended schedule:** Every Monday at 7:00 AM

**Target Personas:** Account Executive, Sales Manager, Business Development

**Tags:** `Scheduled`, `Sales`, `Pipeline`, `Weekly`, `Outlook`

**Prompt:**

```
Review my emails and Teams messages from the last 7 days. Identify every active prospect or client deal I have been communicating about. For each one:
- Company or contact name
- Last communication date
- Current status based on the conversation (active, waiting for response, stalled, at risk)
- Suggested next action

Flag any deals where there has been no communication for more than 5 days. Sort by urgency.
```

---

### 5. Prospect Follow-Up Reminder

**Use Case:** Never let a warm lead go cold

**Recommended schedule:** Every Wednesday at 8:00 AM

**Target Personas:** Account Executive, Sales Rep, Business Development Manager

**Tags:** `Scheduled`, `Sales`, `Follow-up`, `Outlook`, `Pipeline`

**Prompt:**

```
Check my sent emails from the last 14 days. Identify every email I sent to a prospect or external contact where I have not received a reply. For each:
- Contact name and company
- What I sent and when
- Days since sent with no response

Exclude internal colleagues. List oldest first. Flag anyone I sent more than one follow-up to already.
```

---

### 6. Competitive Intelligence Digest

**Use Case:** Track competitor mentions without manually scanning every thread

**Recommended schedule:** Every Friday at 4:00 PM

**Target Personas:** Sales Manager, Account Executive, Strategy, Marketing

**Tags:** `Scheduled`, `Competitive`, `Sales`, `Weekly`, `Intelligence`

**Prompt:**

```
Search my emails and Teams messages from this week for any mention of competitors or alternative solutions to what I sell. List every instance:
- Who mentioned it
- Which competitor or alternative was named
- Context (objection, comparison, evaluation, news)

If no competitor mentions found, confirm that directly. Do not invent examples.
```

---

## Project & Team Management

### 7. Weekly Project Status Brief

**Use Case:** Know where every project stands before the week begins

**Recommended schedule:** Every Monday at 8:00 AM

**Target Personas:** Project Manager, Programme Manager, Delivery Lead

**Tags:** `Scheduled`, `Project Management`, `Teams`, `Weekly`, `Status`

**Prompt:**

```
Review my Teams messages and emails from the last 7 days. For each active project I am involved in:
- Project name
- Progress signals from the week (what moved forward, what stalled)
- Open blockers or risks mentioned
- Decisions still pending

Group by project. Flag anything where no activity was recorded this week.
```

---

### 8. Monday Blocker Check

**Use Case:** Surface blockers before they become escalations

**Recommended schedule:** Every Monday at 9:00 AM

**Target Personas:** Project Manager, Engineering Lead, Delivery Manager

**Tags:** `Scheduled`, `Blockers`, `Teams`, `Project`, `Weekly`

**Prompt:**

```
Search my Teams messages and emails from the last 5 days for anything flagged as blocked, waiting on someone, or at risk of delay. For each item:
- What is blocked
- Who owns it
- Who is needed to unblock it
- How many days it has been waiting

If nothing is blocked, confirm that directly.
```

---

### 9. Friday Team Communication Summary

**Use Case:** Weekly record of key decisions and communications for your team

**Recommended schedule:** Every Friday at 5:00 PM

**Target Personas:** Team Lead, Manager, Project Manager

**Tags:** `Scheduled`, `Teams`, `Summary`, `Weekly`, `Team`

**Prompt:**

```
Summarise my Teams channel activity and email threads from this week that involved my direct team. Extract:
1. Key decisions made
2. Commitments made to stakeholders outside the team
3. Issues raised that are still open
4. Information shared that the team should remember

Keep it factual. No interpretation. Under 250 words.
```

---

## Finance & Reporting

### 10. Weekly Budget Alert Digest

**Use Case:** Catch cost overruns and approvals before they escalate

**Recommended schedule:** Every Monday at 8:30 AM

**Target Personas:** Finance Manager, Controller, Project Finance, CFO

**Tags:** `Scheduled`, `Finance`, `Budget`, `Weekly`, `Outlook`

**Prompt:**

```
Review my emails from the last 7 days for any mention of budget, cost, spend, invoice, PO, approval, or overrun. For each relevant thread:
- Subject and sender
- What the financial issue or request is
- Amount mentioned (if any)
- Action required (approve, review, escalate, note)

Flag any amount above [your threshold — e.g. $10,000] at the top of the list.
```

---

### 11. Monthly Expense and Approval Review

**Use Case:** Ensure nothing requiring finance sign-off slips through at month-end

**Recommended schedule:** Last Monday of each month at 9:00 AM (set as specific recurring date)

**Target Personas:** Finance Controller, Finance Manager, CFO

**Tags:** `Scheduled`, `Finance`, `Approvals`, `Monthly`, `Outlook`

**Prompt:**

```
Search my emails from the last 30 days for any pending financial approvals, invoices awaiting sign-off, or expense reports submitted but not yet approved. List each one:
- What requires approval
- Submitted by whom
- Date submitted
- Amount (if mentioned)
- Current status

Sort by oldest first. Flag anything overdue based on a standard 14-day approval window.
```

---

## HR & People

### 12. Weekly Hiring Pipeline Update

**Use Case:** Keep hiring momentum visible without a manual status call

**Recommended schedule:** Every Monday at 8:00 AM

**Target Personas:** HR Manager, Recruiter, Hiring Manager, HRBP

**Tags:** `Scheduled`, `HR`, `Recruiting`, `Pipeline`, `Weekly`

**Prompt:**

```
Review my emails and Teams messages from the last 7 days related to hiring, candidates, interviews, or job openings. For each active role:
- Role title
- Stage of the most recent candidate (screening, interview, offer, closed)
- Next action required and who owns it
- Any delays or candidate drop-offs noted

Flag any role with no activity in the last 7 days.
```

---

### 13. Employee Check-In Follow-Up Tracker

**Use Case:** Track one-on-one commitments and follow through on them

**Recommended schedule:** Every Friday at 4:30 PM

**Target Personas:** Manager, Team Lead, HRBP, Director

**Tags:** `Scheduled`, `HR`, `Management`, `1on1`, `Weekly`

**Prompt:**

```
Review my emails and Teams messages from this week for any commitments I made to team members in one-on-ones or direct conversations — feedback promised, actions to investigate, connections to make, information to share. List each one:
- Team member name
- What I committed to
- Deadline if mentioned

Do not include project or client commitments — only internal people management items.
```

---

## Executive

### 14. Executive Monday Morning Brief

**Use Case:** Weekly situational awareness before the day begins

**Recommended schedule:** Every Monday at 6:30 AM

**Target Personas:** CEO, COO, CTO, CFO, VP, Director

**Tags:** `Scheduled`, `Executive`, `Weekly`, `Briefing`, `Outlook`

**Prompt:**

```
Summarise the most important communications I received in the last 72 hours. Organise into four sections:
1. Decisions I need to make this week (with deadline if stated)
2. Escalations or issues raised by my team or stakeholders
3. Key external communications requiring a response
4. Upcoming commitments this week I should be aware of

Maximum 300 words. No detail beyond what I need to prioritise my Monday.
```

---

### 15. Weekly Stakeholder Communication Audit

**Use Case:** Ensure no critical relationship goes quiet

**Recommended schedule:** Every Friday at 4:00 PM

**Target Personas:** CEO, VP, Director, Account Director, Senior Manager

**Tags:** `Scheduled`, `Executive`, `Stakeholders`, `Weekly`, `Relationships`

**Prompt:**

```
Review my outbound emails and Teams messages from this week. List every key stakeholder (board members, investors, major clients, direct reports, executive peers) I communicated with. Then list key stakeholders I have NOT communicated with in the last 14 days.

Flag anyone in the "not communicated with" list where a 14-day gap is unusual based on recent communication frequency. Suggest a one-line reason I might want to reach out.
```

---

## Tips for Best Results

**Write for silence.** The prompt runs when you are not there. Every ambiguous reference (this, that, the current project) will produce a generic response. Be explicit about time windows and data scope.

**Start with one.** Set up the Monday morning brief first. Run it for two weeks before adding more. Adjust the prompt based on what it misses.

**10 is the limit.** Choose the prompts that replace the most manual effort. A daily email brief and a weekly pipeline review will save more time than five niche trackers.

**Check notification settings.** Set your top three to send a Teams notification. For lower-priority ones, let results accumulate in history and review them when you want to.

---

## Related Collections

- [Power Users & Advanced Techniques](../power-users/) — multi-step prompts for manual use
- [Role-Specific Collections](../role-specific/) — prompts by job function
- [Security Copilot Prompts](../security-copilot/) — SOC and reporting prompts

---

*Part of the [Awesome Microsoft Copilot Prompts](https://github.com/kesslernity/awesome-microsoft-copilot-prompts) library.*  
*NerdyChefs.ai · CC BY-SA 4.0*
