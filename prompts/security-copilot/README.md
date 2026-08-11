# Microsoft Copilot for Security — Prompting Guide

> A practical guide to Microsoft Copilot for Security: how it works, how SCUs are consumed, and how to write prompts that give you better results without burning unnecessary compute.

---

## What Is Copilot for Security?

Microsoft Copilot for Security is a separate AI product from Microsoft 365 Copilot. It is a security-specific AI assistant that connects to your Microsoft security stack — Defender XDR, Sentinel, Intune, Purview, and Entra — and lets analysts investigate threats, triage incidents, and produce security reports using natural language.

It is **not** a feature of your M365 Copilot license. It runs on its own billing model and its own compute layer.

**Where it lives:**
- Standalone portal: [securitycopilot.microsoft.com](https://securitycopilot.microsoft.com)
- Embedded in Microsoft Defender XDR, Sentinel, Intune, Purview, and Entra (the embedded experience triggers the same SCU consumption)

**What it connects to (plugins/data sources):**
| Plugin | What Copilot can access |
|--------|------------------------|
| Microsoft Defender XDR | Incidents, alerts, devices, users, email threats |
| Microsoft Sentinel | Log data, incidents, watchlists, KQL workspace |
| Microsoft Intune | Device compliance, configuration, app inventory |
| Microsoft Purview | DLP alerts, compliance posture, audit logs |
| Microsoft Entra | Identities, sign-in risk, conditional access, privileged roles |
| Threat Intelligence (MDTI) | Threat actor profiles, CVE enrichment, IOC reputation |
| 3rd-party plugins | ServiceNow, Splunk, and others via the plugin marketplace |

---

## How SCUs Work — The Billing Mechanic

**SCU = Security Compute Unit.** Every interaction with Copilot for Security consumes SCUs. Understanding this mechanic is the most important thing you can do before deploying it at scale.

### SCU Capacity Models

| Model | Cost | How it works |
|-------|------|-------------|
| Provisioned | $4 USD/SCU/hour | Pre-allocated capacity. Billed per hour whether used or not. Stops working when exhausted — analysts see an error until the next hourly cycle. |
| Overage | $6 USD/SCU/hour | Kicks in when provisioned SCUs run out. Must be configured with a cap. |
| M365 E5 Inclusion | Included | 400 SCUs/month per 1,000 paid E5 licenses. Scales with license count. No overage billing — exhaustion = blocked analysts, not surprise charges. |
| M365 E7 | Included | Same inclusion model as E5. |

**Key rule:** Provisioned SCUs are billed per hour, not per minute. One SCU covers roughly one agent skill execution or one AI reasoning step. Complex, open-ended prompts chain multiple reasoning steps and consume multiple SCUs per interaction.

### What Triggers SCU Consumption

| Action | SCU cost |
|--------|---------|
| Simple, specific prompt with clear data source | Low (1–2 SCUs) |
| Open-ended exploratory prompt requiring multi-step reasoning | High (3–8+ SCUs) |
| Promptbook (pre-built workflow) | Medium but predictable |
| KQL skill execution (pre-built query) | Low (~1 SCU per execution) |
| Repeated follow-up prompts to clarify a vague initial prompt | Cumulative — each follow-up burns another SCU |

**The most expensive pattern:** Vague prompt → Copilot reasons broadly → you refine → Copilot reasons again → you refine again. Three prompts where one specific prompt would have done the job.

**The cheapest pattern:** Specific prompt with data source, timeframe, and output format specified → one interaction → done.

---

## The 4 Elements of an Effective Security Prompt

Every prompt to Copilot for Security should include:

| Element | What it does | Example |
|---------|-------------|---------|
| **Goal** | What you want | "Summarize the incident", "List affected devices", "Write an executive summary" |
| **Data source** | Where to look | "in Microsoft Defender XDR", "from Sentinel workspace [name]", "in Entra ID" |
| **Scope** | Timeframe or filter | "from the last 24 hours", "for incident ID 15134", "for user john.doe@company.com" |
| **Output format** | How to present it | "as a bulleted list", "in a paragraph suitable for a manager", "in a table with columns X, Y, Z" |

**Without these elements:** Copilot reasons broadly, uses more SCUs, and returns output you'll need to refine.
**With these elements:** Copilot executes efficiently and returns structured, usable output in one shot.

---

## Prompting Patterns: What Saves SCUs vs. What Burns Them

### ❌ High-cost patterns

```
What threats do I have?
```
No data source. No timeframe. No output format. Copilot reasons across your entire connected environment. Expensive and produces generic output.

```
Tell me everything about this incident.
```
"Everything" triggers maximum reasoning breadth. You'll get a wall of text and need follow-ups to get what you actually need.

```
Is my environment secure?
```
Unanswerable without massive reasoning scope. Never use open-ended posture questions as prompts — use the data source's native dashboard for that.

---

### ✅ Low-cost patterns

```
Summarize incident 15134 in Microsoft Defender XDR. Include: timeline, affected entities (users and devices), root cause if identified, and recommended immediate actions. Format as a structured report I can send to my manager.
```
One data source. One incident ID. Explicit output format. One interaction.

```
You are investigating a potential credential compromise. In Microsoft Entra ID, list all sign-in events for user [UPN] in the last 48 hours. Flag any events with a risk level of medium or higher. Return a table with columns: timestamp, location, IP address, risk level, outcome.
```
Scoped user. Scoped timeframe. Specific risk filter. Structured output format. Executes in one step.

---

## When to Use Promptbooks Instead of Free-Form Prompts

Promptbooks are pre-built prompt sequences for repeatable security workflows. They consume SCUs but in a predictable, controlled way — and they eliminate the back-and-forth that comes from ad-hoc investigation.

**Use Promptbooks when:**
- The workflow runs daily or weekly (e.g., morning threat triage, weekly vulnerability report)
- Multiple analysts run the same investigation steps
- You need consistent, auditable output for compliance or reporting

**Use free-form prompts when:**
- You're investigating a novel incident with no established playbook
- You need to adapt the investigation based on what you find

**Built-in Promptbooks worth knowing:**
- Incident investigation
- Threat actor profile
- Device investigation summary
- Vulnerability impact assessment

You can also create custom Promptbooks in the standalone portal and share them across your team.

---

## KQL-First Principle for Scheduled Work

For repeatable, scheduled work — daily threat checks, compliance reports, audit trail queries — push the intelligence into KQL and use Copilot as the executor, not the reasoner.

**Pattern:**
1. Write the KQL query yourself (or use Copilot to generate it once, then save it)
2. Call the KQL skill from your Copilot prompt or Logic App workflow
3. Ask Copilot to interpret and format the results

This approach costs roughly 1 SCU per execution regardless of query complexity. It scales. Free-form reasoning does not.

---

## Navigation

| File | Contents |
|------|---------|
| [soc-operations.md](./soc-operations.md) | 20 prompts for SOC analysts: incident triage, alert investigation, threat hunting, device and identity investigation |
| [security-reporting.md](./security-reporting.md) | 15 prompts for security managers: executive reporting, vulnerability summaries, compliance posture, post-incident reports |

---

**License:** CC BY-SA 4.0 · [NerdyChefs.ai](https://nerdychefs.ai) · [AI at Work Newsletter](https://newsletter.kesslernity.com/?utm_source=github&utm_medium=readme&utm_campaign=prompts_repo&utm_content=seccopilot_readme)
