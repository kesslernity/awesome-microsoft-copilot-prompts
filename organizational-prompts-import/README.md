# Organizational prompts: an import-ready starter library

> [!IMPORTANT]
> **This Microsoft feature is in preview.** Organizational prompts are in the Frontier preview program now; Microsoft's roadmap targets general availability in July 2026. The CSV here is ready to use, but the admin surface may not appear in your tenant until your organization has preview or GA access. No new licence: it uses the existing Microsoft 365 Copilot add-on. See the status section below.

Microsoft 365 Copilot now lets admins publish a curated prompt library to the whole tenant ("organizational prompts"). The catch in Microsoft's own rollout note: it tells you to "draft and publish an initial prompt library," then hands you a bulk importer with **no prompts in it**.

This folder fills that gap. **44 production-safe prompts, a mix of quick everyday prompts and richer structured ones, across 8 departments, already formatted into Microsoft's exact `prompt-import-template.csv` schema.** Download `organizational-prompts-starter.csv`, import it, publish. Free.

These are carved from [awesome-microsoft-copilot-prompts](../README.md), the most-starred M365 Copilot prompt library on GitHub.

> Independent practitioner resource. Not affiliated with Microsoft. Microsoft is cited only as a neutral source.

---

## What you get

`organizational-prompts-starter.csv`, 44 prompts across 8 departments (5 to 7 each):

| Department | Department | 
|---|---|
| Finance | Project Management |
| HR | IT |
| Sales | Procurement |
| Marketing | Customer Success |

It is a **mix of two kinds**: quick everyday prompts (one task, paste and go) and richer structured prompts that bake in the grounding, guardrails, and output format for heavier workflows like weekly status reports, account briefings, audit-response prep, and incident write-ups. The rich ones use a clear role line, a "work only from what is there, never invent, mark [VERIFY]" rule, a numbered output structure, and a "draft for you to verify, do not send" close.

Every prompt is a **drafting, summarizing, or research aid that works on the user's own work data** (their email, Teams, SharePoint, meetings). None of them perform calculations, approvals, scoring, or decisions. The prompt prepares; the person decides. The "never use Copilot for" rules from the source packs (no financial calculations, no hiring or performance decisions, no legal determinations) are baked into the selection.

---

## The status, stated honestly (June 2026)

- **In Frontier preview now.** Per [Microsoft Learn](https://learn.microsoft.com/en-us/microsoft-365/copilot/organizational-prompts) (doc updated 2026-06-18), the feature needs the Frontier preview program for early access.
- **GA targeted July 2026.** Microsoft's roadmap (ID 486695 / Message Center MC1396361) targets general availability worldwide in July 2026, available by default, with no change to Copilot licensing.
- **Requires a Microsoft 365 Copilot licence** (the existing $30 per-user add-on). No new SKU.

If you are reading this before GA in your tenant, the admin surface may not be visible yet.

---

## The limits nobody mentions

These are the load-bearing facts that decide how you build your library. All from the Microsoft Learn doc.

| Limit | Value |
|---|---|
| Prompts per tenant | **1,000** (publishing more throws "published items limit reached") |
| Prompts you can pin | **Only 4** (the "Suggested" prompts every user sees) |
| Bulk import per file | 100 prompts, 5 MB max, UTF-8 CSV |
| Time to appear | About **3 hours** after publish or edit |
| Translation | **None.** One prompt per language; you set the `Locale` |
| Character limits | Title **35**, Display Prompt **132**, Prompt Text **8,000**, Department **120**, Description **200** |
| Required fields | Title, Display Prompt, Prompt Text, Locale, Task Type, Products |

**The 4-pin reality is the one that bites.** You can publish 1,000 prompts, but only 4 are pinned as "Suggested" on the Copilot Chat home page. Everything else lives in the prompt lab, found by search or filter. So pinning is a prioritization decision, not a nice-to-have. Pick the 4 most universal prompts your whole org would use.

Suggested starting pins from this pack (edit to fit your org): **Weekly status synthesis** (Project Management), **Account research briefing** (Sales), **Internal announcement draft** (Marketing), **Maintenance notice draft** (IT). These are marked with `PIN:` in their Description column.

---

## How to import

1. Microsoft 365 admin center (admin.microsoft.com) → expand **Copilot** → **Prompts**. You need the **AI Administrator** or **Search Editor** role.
2. Select **Import prompts** → **Download prompts template (.csv)** so you have Microsoft's current template to compare against.
3. Use `organizational-prompts-starter.csv` from this folder. Open it, keep or edit the rows, and **save as CSV UTF-8 (comma delimited)**.
4. Upload and **review the validation preview** before you commit.
5. Wait about 3 hours, then check the prompt lab.

### Three gotchas that will reject your import

- **Match the template columns and their exact order:** `Title`, `Description`, `Display Prompt`, `Prompt Text`, `Products`, `Department`, `Task Type`, `Locale`. This CSV already matches. If you exported your existing prompts to edit them, delete any extra columns (like `Last Updated`) before re-importing.
- **Task Type must be one of Microsoft's supported values.** A value outside the list (for example "Manage") rejects the whole import. The supported task types, from the import flyout's **View all supported task types**, are: Analyze, Ask, Assist, Catch up, Code, Create, Design, Edit, Execute, Find, Learn, Prepare, Schedule, Understand. This pack uses only valid ones (Analyze, Create, Find).
- **Products must match the supported-apps list.** The two valid values are `Copilot web` and `Copilot work`. This pack uses both (`Copilot web, Copilot work`) so prompts appear on each surface. Note: the prompts that pull from your work data (email, Teams, SharePoint) only ground on **Copilot work**; on **Copilot web** they have no access to your files, so treat web as the surface for the general drafting prompts.

---

## Do not confuse these three things

The naming around this feature is genuinely messy. Be precise:

- **Organizational prompts** (this feature): admin-published prompts in the M365 admin center, surfaced in Copilot Chat, Teams, and Edge.
- **Copilot Prompt Gallery** / **prompt lab**: the user-facing library where these appear. Admin docs say "prompt lab," user docs say "Prompt Gallery." Same place.
- **Organizational messages**: a completely different admin feature for adoption nudges and onboarding emails. Not prompts.

A "GA May 2025" claim is circulating from a third party. It is wrong for this admin-center feature; it describes the older Prompt Gallery sharing capability.

---

## Governing the library after you publish

Publishing is the easy part. Keeping it useful is the work:

- **Give it an owner.** A 1,000-prompt library with no owner becomes a junk drawer.
- **Use the built-in analytics.** Each prompt shows Active users and Submissions over 7, 14, or 28 days. Prune the prompts nobody uses; promote the ones that land.
- **Review the 4 pins quarterly.** They are your most valuable real estate.

This is the operational layer. If you want the full governance model (the owner role, the quarterly review cadence, the pin-prioritization, and the honest read on where Copilot does not belong), that is what [The Honest M365 Copilot Kit](https://store.kesslernity.com/l/honest-m365-copilot-kit) covers.

---

## Source and licence

Carved from [awesome-microsoft-copilot-prompts](../README.md). Licence: CC BY-SA 4.0. Verify every output before you rely on it. AI prepares, you decide.
