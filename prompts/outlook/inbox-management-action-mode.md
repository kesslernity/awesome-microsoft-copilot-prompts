# Copilot Inbox Management — Action Mode Prompts

> 9 prompts for Copilot's new action mode in Outlook: inbox triage, rule creation, non-responder follow-ups, post-vacation recovery, and intelligent drafting. These prompts issue commands — Copilot acts on your inbox, not just talks about it.

⚠️ **REQUIRES — all three must be active:**
1. **Microsoft 365 Copilot license** (Copilot add-on, M365 E5 + Copilot, or M365 E7)
2. **Frontier program enrollment** — action mode is the default Copilot Chat experience in Frontier as of April 27, 2026
3. **Anthropic subprocessor enabled** — action mode runs on Claude (same stack as Copilot Cowork). Your admin must accept the updated data processing terms and enable Anthropic model access (`admin.microsoft.com` → Copilot → Settings, or via group-level controls). This is the most common silent blocker — Frontier can be on and action mode still won't appear if Claude access hasn't been granted. Regional note: in **EU/EFTA/UK tenants**, Anthropic is off by default — your admin must explicitly opt in. In **Government and Sovereign cloud tenants**, Anthropic models are fully excluded and cannot be enabled.

To verify you're in action mode: look for the **"default mode" dropdown** above the Copilot prompt box in Outlook. **Not available to EU users.**

**Category:** Productivity & Tools

**Prompts in this pack:** 12

---

## Overview

These prompts use Copilot as an inbox operator — not an inbox summarizer. The distinction matters: instead of asking Copilot to describe what's in your inbox, you're asking it to act on it. Draft a reply, create a rule, triage everything from the past week, flag non-responders, and clean up after a vacation.

### What's Included

- **Triage & Prioritization** (3 prompts) — Get to inbox zero with Copilot doing the sorting
- **Non-Responder Detection & Follow-Up** (1 prompt) — Never lose a thread because someone went quiet
- **Inbox Rules & Automation** (3 prompts) — Create rules conversationally, review before applying
- **Tagging & Categorization** (3 prompts) — Apply color categories and flags automatically, by project or status
- **Post-Vacation & Absence Recovery** (1 prompt) — Return to inbox without the panic
- **Complex Draft Assembly** (1 prompt) — Pull context from past threads to write replies that land

### Folder Visibility Note

When Copilot moves emails to custom folders (Reading, CC — Low Priority, Return Reading), those emails stay fully accessible to Copilot — but only if you ask about them explicitly. Default triage and "what needs my attention" queries scope to your primary Inbox. After any triage run that moves emails to folders, follow up with: *"Check my [folder name] folder — anything I should revisit?"*

---

## 📋 Triage & Prioritization

### 1. The Three-Day Triage

**Use Case:** Rapid inbox prioritization after a busy period or Monday morning catch-up

**Target Personas:** Manager, Executive, Project Manager, Individual Contributor, Team Lead

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Triage`, `Productivity`

**Prompt:**

```
Triage everything in my inbox from the last 3 days. Sort into three groups: (1) Needs my reply today — flag each with a one-line summary of what's being asked. (2) Needs my attention this week but not urgent — list with subject and sender. (3) No action required — archive or move to a Reading folder. Show me the plan before applying any moves.
```

---

### 2. The Daily Priority Commander

**Use Case:** Start-of-day inbox focus — surface what actually matters before anything else

**Target Personas:** Manager, Executive, Director, Individual Contributor, Professional

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Prioritization`, `Daily Workflow`

**Prompt:**

```
Scan my inbox and identify everything that needs a response from me today. Rank by urgency: (1) Blocking someone else's work — queue a brief holding reply for each so they know I've seen it, (2) Time-sensitive decision required — draft my response options so I can choose and send, (3) Routine reply needed — list with a suggested one-line reply I can approve. Show all drafts before anything is sent.
```

---

### 3. The High-Priority Auto-Tagger

**Use Case:** Create permanent rules so future important emails surface automatically

**Target Personas:** Manager, Executive, Chief of Staff, Operations Manager, Team Lead

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Inbox Rules`, `Automation`

**Prompt:**

```
Create inbox rules to automatically flag as high priority: (1) Emails from my direct manager or skip-level, (2) Emails where I am the only recipient in the To field, (3) Emails with "urgent", "deadline", "blocking", "escalation", or "action required" in the subject line, (4) Emails from external clients or partners I've corresponded with in the last 30 days. Show me the proposed rules before creating them, and let me edit the sender list if needed.
```

---

## 🔔 Non-Responder Detection & Follow-Up

### 4. The Non-Responder Scanner

**Use Case:** Recover stalled threads — surface everything that went quiet after you sent it

**Target Personas:** Project Manager, Account Manager, Sales Manager, Team Lead, Individual Contributor

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Follow-Up`, `Non-Responder`

**Prompt:**

```
Scan my sent emails from the last 10 days. Find every email I sent that has not received a reply. Group them by urgency: (1) Blocking a decision or deliverable, (2) Time-sensitive but not yet critical, (3) Routine follow-up. For each email in groups 1 and 2, draft a short, professional follow-up. Keep the tone warm — assume good intent, not negligence. Show drafts before sending.
```

---

## ⚙️ Inbox Rules & Automation

### 5. The Inbox Organizer

**Use Case:** Create a smart folder structure based on how emails already cluster in your inbox

**Target Personas:** Manager, Executive, Individual Contributor, Knowledge Worker, Operations Manager

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Inbox Rules`, `Organization`

**Prompt:**

```
Analyze my inbox from the last 45 days. Identify the top 5–7 recurring categories of emails (e.g. weekly reports, newsletters, internal HR comms, project updates, vendor invoices). For each category, propose an inbox rule that routes future emails to a dedicated folder. Show me the proposed folder names and routing logic before creating anything. I'll confirm, adjust, or reject each rule individually.
```

---

### 6. The Newsletter Declutterer

**Use Case:** Surgically remove newsletter noise without losing content you actually read

**Target Personas:** Individual Contributor, Manager, Executive, Knowledge Worker, Professional

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Inbox Rules`, `Focus`

**Prompt:**

```
Identify all newsletters, marketing emails, and automated digests that landed in my inbox in the last 30 days. Group them into: (1) I actually open these — create a rule to route future emails to a "Reading" folder so they're available when I want them, (2) I never open these — create delete rules so they never reach my inbox. Show me the groupings before creating any rules. Don't touch emails from real people or internal senders.
```

---

### 7. The Reply-All Blocker

**Use Case:** Stop reply-all threads from flooding your inbox while staying in the loop

**Target Personas:** Manager, Executive, Individual Contributor, Team Lead, Director

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Inbox Rules`, `Noise Reduction`

**Prompt:**

```
Find email threads from the last 30 days where I was CC'd and the thread has more than 10 replies, and I have not replied myself. These are likely reply-all chains I don't need to monitor closely. Create rules to route future emails in these threads to a "CC — Low Priority" folder rather than my main inbox. Show me the proposed threads and rules before applying anything. Flag any thread where I'm expected to act eventually.
```

---

## 🏷️ Tagging & Categorization

### 8. The Project Auto-Tagger

**Use Case:** Keep project emails visible at a glance — automatically color-code by project as they arrive

**Target Personas:** Project Manager, Manager, Executive, Team Lead, Individual Contributor

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Categories`, `Organization`

**Prompt:**

```
Create inbox rules that automatically apply Outlook color categories to incoming emails by project. For each project, I'll specify the category color and the matching criteria: [list each project, e.g., "Project Alpha → Blue — match subject keywords: Alpha, Phase 2; Client X → Green — match sender domain: clientx.com; Budget Review → Yellow — match subject keywords: budget, Q3 forecast"]. After creating the rules, apply them retroactively to all emails in my inbox from the last 60 days. Show me the rule definitions and the match count per project before applying anything.
```

---

### 9. The Inbox Color-Code System

**Use Case:** Make action status visible at a glance — apply a consistent category system across your existing inbox

**Target Personas:** Manager, Executive, Individual Contributor, Chief of Staff, Operations Manager

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Categories`, `Triage`

**Prompt:**

```
Apply Outlook categories to emails in my inbox from the last 30 days based on action status: Red = I need to reply and haven't yet, Yellow = I'm waiting on a reply from someone else, Green = informational — read but no action needed, Purple = meeting or calendar-related. Show me the proposed categorization and the count per color before applying. Flag any email where you're unsure which category fits — I'll decide those manually.
```

---

### 10. The VIP Contact Flagger

**Use Case:** Ensure emails from your most important contacts are always flagged for follow-up, even if they slip through triage

**Target Personas:** Executive, Manager, Account Manager, Chief of Staff, Sales Manager

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Flags`, `Follow-Up`

**Prompt:**

```
Create an inbox rule that automatically flags for follow-up any email that arrives from: [list names or domains — e.g., "my direct manager, skip-level, and these external contacts: name@domain.com, @clientdomain.com"]. Then scan my inbox from the last 14 days and flag any emails from these contacts that aren't already flagged. Show me the rule and the list of emails it would flag before applying anything.
```

---

## 🏖️ Post-Vacation & Absence Recovery

### 11. The Vacation Recovery Commander

**Use Case:** Return from time off without spending half a day triaging email

**Target Personas:** Manager, Executive, Individual Contributor, Team Lead, Professional

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Post-Vacation`, `Triage`

**Prompt:**

```
I've been out of office for [X days / from DATE to DATE]. Triage everything that arrived while I was away. Sort into: (1) Needs my response today — summarize what's being asked and draft a brief reply, (2) Was resolved without me — archive, (3) Should read but no action needed — move to a "Return Reading" folder, (4) Can be deleted. Show me the plan and all draft replies before anything is sent or moved.
```

---

## ✍️ Complex Draft Assembly

### 12. The Context-Aware Reply Builder

**Use Case:** Write replies that reference history, project context, and past commitments — not just the latest email

**Target Personas:** Project Manager, Account Manager, Executive, Manager, Individual Contributor

**Tags:** `Microsoft Copilot`, `Outlook`, `Inbox Management`, `Action Mode`, `Frontier`, `Drafting`, `Context-Aware`

**Prompt:**

```
I need to reply to the most recent email from [NAME] about [TOPIC or PROJECT]. Search our full email history on this topic from the last 90 days. Extract: what I've already committed to, what's still open, any deadlines I mentioned, and the tone of our recent exchanges. Draft a reply that addresses their latest message, references the relevant commitments, and moves the conversation forward — under 200 words. Queue it as a draft in my Drafts folder so I can review, edit, and send from there.
```

---

## 📚 Additional Resources

- [Back to Main Collection](../../README.md)
- [Advanced Outlook Automation Pack](advanced-automation.md)
- [Advanced Outlook Prompts](advanced-prompts.md)
- [Role-Specific Collections](../role-specific/)

---

> **Feature note:** These prompts use Copilot's action mode introduced in Frontier on April 27, 2026 (MC1293485). Action mode is the default experience in Copilot Chat for Outlook in the Frontier program. To revert to chat-only mode, use the "default mode" dropdown above the prompt box. Not available to users in the EU.

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

For the complete library of prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
