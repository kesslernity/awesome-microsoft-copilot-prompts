# Copilot Cowork — Agentic Workflow Prompts

> 28 production-ready prompts for Microsoft 365 Copilot Cowork. Cowork is the agentic execution layer inside M365 Copilot — you describe an outcome, Cowork plans the steps, searches across your Outlook, Teams, Calendar, and SharePoint, and executes the work with your approval at each action.

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md)

---

## Collections

### [Scheduled Briefings & Guardrails](scheduled-briefings.md) — 5 prompts

Set-and-forget recurring workflows plus the foundational guardrail prompt every Cowork user should run first:

- Guardrail: What Cowork Should Never Do Without Approval
- Monday Week-Start Briefing (schedulable)
- Friday End-of-Week Digest (schedulable)
- Daily Inbox Priority Scan (schedulable)
- Weekly Commitment Tracker (schedulable)

### [Research & Synthesis Workflows](research-workflows.md) — 13 prompts

Prompts that pull, synthesise, and structure information from across your M365 environment. Read-only outputs — Cowork searches and drafts; you review before anything is sent:

- Meeting & Stakeholder Prep (Pre-Meeting Brief, Stakeholder Update, Post-Meeting Capture, Executive Pre-Read)
- Project & Portfolio Management (Project Status Digest, Risk & Blocker Sweep)
- Document Generation (Document from Meeting Notes, Presentation from Brief)
- Research & Analysis (Deep Research, Competitive Signal Sweep, Stakeholder Onboarding Brief)
- Calendar Management (Weekly Calendar Triage, Recurring Meeting Prep)

### [Action-Taking Workflows](action-workflows.md) — 10 prompts

Prompts that do things Chat cannot. Chat drafts — Cowork executes. Every prompt here ends with Cowork taking an action after showing you a full preview for approval:

- Send Meeting Follow-Up Email
- Schedule a Meeting Based on Calendar Availability
- Post Weekly Project Update to Teams Channel (schedulable)
- Inbox Triage — Reply to Flagged Emails
- Send Stakeholder Update After Approval (end-to-end)
- Block Focus Time on Calendar (schedulable)
- Reschedule Calendar Conflicts
- Draft and Send Renewal Reminder
- Create and Share a Document with Stakeholders
- End-to-End Weekly Status Report (schedulable)

---

## Requirements

> **REQUIRES:**
> - Microsoft 365 Copilot licence
> - Cowork switched on by your admin. It reached general availability worldwide on 16 June 2026 and is **off by default**
> - Anthropic models enabled as sub-processor in M365 Admin Center
> - Budget for **Copilot Credits**. Cowork is metered on top of the licence, so every run costs credits (model use, context retrieval, tool calls, runtime). Admins can set spend limits and usage alerts per tenant, group and user
> - Access at: [m365.cloud.microsoft](https://m365.cloud.microsoft)

**NOT compatible with:** Copilot Chat, ChatGPT, Claude.ai, or any non-Cowork interface.

---

## How Cowork Prompts Differ from Chat Prompts

Chat and Cowork both search M365 data. That is not the difference.

The difference is what happens after the research. Chat hands you a draft and stops. Cowork can **send the email, schedule the meeting, post to Teams, create the calendar block** — with your explicit approval before each action. The prompts in [action-workflows.md](action-workflows.md) are where this distinction is visible.

**The Delegation Brief format — use this structure for every Cowork prompt:**

1. **Goal** — the outcome you want (not the steps)
2. **Inputs** — which M365 sources to pull from (Outlook, Teams, Calendar, SharePoint)
3. **Output** — what to produce and in what format
4. **Boundaries** — what not to do; what needs your approval before action is taken

**Show sources before drafting:** Include "show me what you found before moving to Step 2" in any multi-step prompt where accuracy matters. Cowork will pause after the search phase and display source messages before writing.

---

## Notes & Limitations

- **Scheduled runs are a standing cost.** Every execution consumes Copilot Credits, so a recurring slot bills every time it fires, not once. If you are picking a short list to start with, this order earns its keep: Monday Briefing, Commitment Tracker, Calendar Triage, Project Digest, Daily Inbox Scan
- **Approval model** — Cowork shows a full preview before sending emails, posting to Teams, or modifying calendar events. Always verify recipients, content, and timing before approving
- **Attach files explicitly** — for document generation prompts, drag and drop the file rather than asking Cowork to find it from SharePoint (more reliable in testing)
- **Custom skills** — for workflows you run frequently, save the prompt as a custom skill at `/Documents/Cowork/skills/` in OneDrive as a Markdown file. Up to 50 custom skills supported
- **EU tenants** — Cowork requires Anthropic models enabled. EU/EFTA tenants have Anthropic off by default — admin must enable separately in M365 Admin Center before Cowork is fully functional

---

*Prompts first tested in Microsoft 365 Copilot Cowork in May 2026, during the Frontier preview that preceded general availability on 16 June 2026. Production use: review all outputs before sending or sharing.*

*Part of the [awesome-microsoft-copilot-prompts](https://github.com/kesslernity/awesome-microsoft-copilot-prompts) collection*
