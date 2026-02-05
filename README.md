# Awesome Microsoft Copilot Prompts 🍳

[![Prompts](https://img.shields.io/badge/prompts-365-blue)](https://nerdychefs.ai)
[![Categories](https://img.shields.io/badge/categories-17-green)](https://nerdychefs.ai)
[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)](/LICENSE)
[![Enterprise](https://img.shields.io/badge/enterprise-tested-purple)](https://kesslernity.com)

A curated collection of **365 production-tested Microsoft Copilot prompts** for enterprise professionals. From inbox intelligence to role-specific workflows, these prompts help you get the most out of Microsoft 365 Copilot.

> Stop staring at the blank Copilot box. 365 enterprise-tested prompts that actually work—organized by role, not random categories.

## 🧭 Contents

- 📊 [Quick Stats](#-quick-stats)
- 🚀 [Quick Start](#-quick-start)
- 🔄 [Copilot vs ChatGPT: Key Differences](#-copilot-vs-chatgpt-key-differences)
- 📚 [Complete Prompt Collection](#-complete-collection-365-prompts)
- 👔 [Role-Specific Prompt Packs](#-role-specific-collections-203-prompts)
- 💡 [How to Use These Prompts](#-how-to-use-these-prompts)
- 🔥 [Most Popular Prompts](#-most-popular-prompts)
- 🔐 [Governance & Guardrails](#-governance--guardrails)
- 🏢 [Enterprise Deployment](#-enterprise-deployment)
- 🤝 [Contributing](#-contributing)
- 📖 [Prompt Engineering Tips](#-prompt-engineering-tips)
- 📄 [License](#-license)


## 📊 Quick Stats

- **365 Total Prompts** across 17 specialized collections
- **26 Power User Prompts** for advanced Copilot mastery
- **70 Outlook Prompts** for email intelligence and automation
- **66 Standalone Prompts** for any Copilot version
- **203 Role-Specific Prompts** covering 12 business functions
- **Tested in Production** by thousands of enterprise users

## 🚀 Quick Start

### Example: Turn Your Inbox into a Strategic Intelligence System

**Prompt:** "Inbox Intelligence Officer"

```
Analyze all emails I received in the last 30 days. Create a full intelligence briefing including:
1) Key actors and recurring senders
2) Communication tone by sender (supportive, neutral, demanding)
3) Topic clusters and themes
4) Unresolved threads requiring action
5) Projects that appear across multiple emails
6) Status score for each project (on track, at risk, blocked)
7) People I need to engage with more frequently

Format as an executive briefing.
```

**Use Case:** Strategic email management
**Works In:** Outlook Copilot
**Target Users:** Executives, Managers, Project Managers

[See 70 more Outlook prompts →](prompts/outlook/)

### Example: Excel Data Analysis Without Being a Data Scientist

**Prompt:** "Data Storyteller"

```
Analyze this dataset and tell the data story:
1) Key trends over time
2) Notable outliers or anomalies with potential explanations
3) Correlations or relationships between variables
4) Segments or clusters in the data
5) Unexpected findings
6) Business implications of each insight
7) Recommended actions based on analysis

Create visualizations for top 3 insights and provide narrative explanations suitable for presentation.
```

**Use Case:** Business intelligence and reporting
**Works In:** Excel Copilot
**Target Users:** Business Analysts, Managers, Data Analysts

[See more Excel prompts →](prompts/power-users/README.md)

## 🔄 Copilot vs ChatGPT: Key Differences

Even when using the same underlying model (GPT-4/GPT-5), **Copilot behaves differently**:

| Aspect | Microsoft Copilot | ChatGPT |
|--------|-------------------|---------|
| **Safety filters** | Enterprise-grade, strict | Consumer-level, more permissive |
| **Data access** | Your M365 organizational data | No access to your files/emails |
| **Vision capabilities** | Restricted/simplified pipelines | Full multimodal reasoning |
| **Reasoning depth** | Optimized for fast, safe answers | Allows exploratory reasoning |
| **Uncertain results** | Prefers "no result" over guessing | May provide probabilistic answers |
| **Best for** | Business documents & structured data | Creative writing & coding |

### What Copilot Does Well ✅
- Compare structured documents
- Summarize long technical PDFs
- Cross-reference requirements across files
- Answer questions when tags/metadata are explicit
- Reason over text-heavy documents

### What Copilot Struggles With ⚠️
- Dense visual tagging in schematics
- Implicit symbol recognition
- Ambiguous labels in images
- Vision-first analysis without supporting text
- Engineering drawings, P&IDs, EPC schematics

## 📚 Complete Collection (365 Prompts)

### 🎓 Power Users & Advanced Techniques

- [**AI for Microsoft Copilot Power Users**](prompts/power-users/README.md) (26 prompts)
  + Advanced email intelligence
  + Excel data intelligence
  + Outlook email mastery
  + PowerPoint presentation power
  + Teams meeting intelligence
  + Word document excellence

### 📧 Email & Communication Mastery (70 prompts)

- [**Advanced Outlook Automation**](prompts/outlook/advanced-automation.md) (20 prompts)
  + Cognitive load & workload management
  + Compliance & knowledge extraction
  + Email battle planning & prioritization
  + Inbox intelligence & strategic analysis
  + Relationship & stakeholder intelligence
  + Risk detection & early warning systems

- [**Advanced Outlook Prompt Pack**](prompts/outlook/advanced-prompts.md) (50 prompts)
  + Collaboration & communication
  + Customer relations
  + Decision support
  + Documentation & reporting
  + Meeting preparation & follow-up
  + Problem solving
  + Risk & compliance

### 🏢 Enterprise & Quick Start (66 prompts)

- [**Copilot Enterprise Prompts (Standalone)**](prompts/enterprise/standalone-prompts.md) (16 prompts)
  + Analysis & reasoning frameworks
  + Business writing templates
  + Data processing & extraction
  + Document analysis & comparison
  + Image analysis (with limitations noted)
  + Technical documentation

- [**Copilot Quick Start Essentials**](prompts/quick-start/essentials.md) (50 prompts)
  + Analysis & problem-solving
  + Content creation
  + Learning & research
  + Planning & organization
  + Writing & communication

### 👔 Role-Specific Collections (203 prompts)

#### Business Operations & Support

- [**Administrative & Executive Assistants**](prompts/role-specific/admin-executive-assistants.md) (17 prompts)
  + Board support, calendar management, correspondence
  + Document management, event & travel coordination
  + Meeting support, process documentation
  + **Includes ⚠️ Administrative Copilot Guardrails**

- [**Commercial Operations**](prompts/role-specific/commercial-operations.md) (18 prompts)
  + Baseline management, bid management, contract tracking
  + Document control, delay analysis, distribution control
  + **Includes ⚠️ Commercial Operations Copilot Guardrails**

- [**Project Leadership**](prompts/role-specific/project-leadership.md) (18 prompts)
  + Budget management, change tracking, client communication
  + Cost reporting, decision support, stakeholder management
  + **Includes ⚠️ Leadership Copilot Guardrails**

#### Revenue & Growth

- [**Sales & Business Development**](prompts/role-specific/sales-business-development.md) (16 prompts)
  + Account management, competitive analysis, lead qualification
  + Outreach sequences, pipeline management, proposal follow-up
  + **Includes ⚠️ Sales Copilot Guardrails**

- [**Marketing & Communications**](prompts/role-specific/marketing-communications.md) (16 prompts)
  + Campaign management, content creation, event marketing
  + Social media, PR, internal communications
  + **Includes ⚠️ Marketing & Communications Copilot Guardrails**

- [**Customer Success & Support**](prompts/role-specific/customer-success-support.md) (16 prompts)
  + Account health monitoring, QBR preparation, renewal management
  + Escalation handling, onboarding support, expansion opportunities
  + **Includes ⚠️ Customer Success & Support Copilot Guardrails**

#### Professional Services

- [**Consulting & Professional Services**](prompts/role-specific/consulting-professional-services.md) (16 prompts)
  + Advisory services, client management, deliverable development
  + Engagement management, workshop facilitation
  + **Includes ⚠️ Consulting Copilot Guardrails + Client Confidentiality Warnings**

- [**Engineering & Construction**](prompts/role-specific/engineering-construction.md) (16 prompts)
  + Field documentation, meeting prep, problem resolution
  + Project communication, quality management, site coordination
  + **Includes ⚠️ Engineering Copilot Guardrails + ⚠️ Construction Safety Guardrails**

#### Corporate Functions

- [**Finance & HR**](prompts/role-specific/finance-hr.md) (18 prompts)
  + Audit support, budgeting, financial review
  + HR policy, internal comms, onboarding, employee engagement
  + **Includes ⚠️ Finance & HR Copilot Guardrails**

- [**HSE, Legal & Compliance**](prompts/role-specific/hse-legal-compliance.md) (20 prompts)
  + Safety procedures, incident research, environmental compliance
  + Contract negotiation, claims management, legal research
  + **⛔ CRITICAL HSE GUARDRAILS - Safety authorization boundaries**
  + **Includes ⚠️ Legal & IT Copilot Guardrails**

#### Specialized Functions

- [**Research & Development**](prompts/role-specific/research-development.md) (16 prompts)
  + Prior art research, experiment tracking, literature review
  + Publication planning, competitive research, lab management
  + **Includes ⚠️ R&D Copilot Guardrails + IP & Confidentiality Warnings**

- [**Supply Chain & Logistics**](prompts/role-specific/supply-chain-logistics.md) (16 prompts)
  + Supplier management, shipment tracking, inventory optimization
  + Disruption management, customs support, S&OP planning
  + **Includes ⚠️ Supply Chain & Logistics Copilot Guardrails**

## 🗂 Repository Structure

The repository is organized by **Copilot application and user role**, making it easy to browse, reuse, and extend.

```text
prompts/
├── power-users/
│   └── README.md                # Advanced Copilot techniques & mastery prompts
│
├── outlook/
│   ├── advanced-automation.md   # Inbox intelligence & automation
│   ├── advanced-prompts.md      # Advanced Outlook prompt pack
│   └── README.md
│
├── quick-start/
│   └── essentials.md            # Beginner-friendly Copilot essentials
│
├── enterprise/
│   └── standalone-prompts.md    # App-agnostic enterprise prompts
│
└── role-specific/
    ├── admin-executive-assistants.md
    ├── commercial-operations.md
    ├── project-leadership.md
    ├── sales-business-development.md
    ├── marketing-communications.md
    ├── customer-success-support.md
    ├── consulting-professional-services.md
    ├── engineering-construction.md
    ├── finance-hr.md
    ├── hse-legal-compliance.md
    ├── research-development.md
    └── supply-chain-logistics.md
```

## 💡 How to Use These Prompts

### 1. Find Your Use Case

Browse by role or search for your specific need (e.g., "email prioritization", "data analysis", "meeting prep").

### 2. Copy & Customize

Each prompt is designed to work immediately but customize the placeholders:

- `[TOPIC]` → your specific subject
- `[TIMEFRAME]` → your desired period
- `[METRIC]` → your KPI or measurement
- `[ACCOUNT NAME]` → specific client or project

### 3. Run in Copilot

Paste the prompt into the appropriate Microsoft 365 app:

- **Outlook:** Use in Outlook Copilot chat or sidebar
- **Excel:** Use in Excel Copilot sidebar for data analysis
- **Word:** Use in Word Copilot drafting or editing
- **PowerPoint:** Use in PowerPoint Copilot designer
- **Teams:** Use in Teams Copilot chat for meeting intelligence

### 4. Iterate & Improve

Copilot learns from context. If the first result isn't perfect, provide feedback:
- "Make it more concise"
- "Focus on Q4 data only"
- "Add risk assessment"
- "Format as a table"

## 🔥 Most Popular Prompts

1. **360° Relationship Mapper** - Map stakeholder relationships from email patterns
2. **Early Warning System** - Predict which topics will become future problems
3. **Dashboard Insight Generator** - Turn Excel data into executive dashboards
4. **Email Battle Plan Generator** - Strategic inbox prioritization
5. **Context Fusion Engine** - Synthesize project status across all communications
6. **Escalation Radar Detector** - Early crisis detection from email sentiment
7. **Meeting Prep Intelligence Pack** - Comprehensive meeting preparation
8. **QBR Preparation** - Quarterly business review content from communications
9. **Deal Progress Summary** - Complete deal tracking from scattered emails
10. **Shipment Issue Summary** - Logistics intelligence from multiple sources

[See all power user prompts →](prompts/power-users/README.md)

## 🏢 Enterprise Deployment

Using Copilot across your organization? These prompts work even better when deployed enterprise-wide.

**Need help with:**
- Enterprise prompt governance
- Team training and adoption
- Role-based prompt libraries

👉 **[Check out Kesslernity](https://kesslernity.com)** - Enterprise AI deployment platform

## 🌐 Full Searchable Library

This repo contains **365 prompts** optimized for Microsoft Copilot. For the complete searchable library with:

- Advanced filtering by role, use case, and app
- Copy-to-clipboard functionality
- Regular updates with new prompts
- Additional ChatGPT, Claude, and Gemini prompts
- **No signup required**

👉 **Visit [NerdyChefs.ai](https://nerdychefs.ai)** - 1300+ free AI prompts & tools

## 🤝 Contributing

Have a killer Copilot prompt that's made your work life easier? We'd love to add it!

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:

- Prompt format requirements
- Testing standards (must be production-tested)
- Documentation expectations
- Review process

**Quality bar:** We only accept prompts that:

1. Solve real business problems
2. Have been tested in production environments
3. Include clear use cases and target personas
4. Work specifically with Microsoft Copilot (not generic AI prompts)

## 📖 Prompt Engineering Tips

New to Copilot? Here's how to get better results:

### The 4-Question Formula

Transform vague requests into specific prompts:

1. **WHAT** - What exactly do you want? (Be specific)
2. **WHO** - Who is this for? (Audience matters)
3. **WHY** - What's the business context? (Purpose drives output)
4. **HOW LONG** - How detailed? (Scope the response)

**Example:**
❌ "Summarize my emails"
✅ "Summarize emails from the last 7 days related to the Q1 budget review. I need bullet points for my VP—keep it under 5 key points highlighting any blockers."

### Give Copilot Context

- Reference specific data: "Based on the spreadsheet I just opened..."
- Mention timeframes: "In emails from this month..."
- Specify format: "Create as a table" or "Write as a memo"
- Include audience: "For technical team" vs "For executive review"

### Iterate Don't Restart

If the output isn't right:

- Add constraints: "Make it shorter" or "Focus only on risks"
- Provide examples: "Like the format we used last quarter"
- Correct mistakes: "The deadline is March 15, not May 15"
- Request specific changes: "Add a risk assessment section"

## 🔐 Governance & Guardrails

Every role-specific collection includes **critical guardrails** explaining:

- ✅ What Copilot IS good for in that role
- ❌ When NEVER to use Copilot (safety, compliance, legal)
- ⚠️ System limitations and integration notes
- 📝 Golden rules for responsible usage

**Example guardrails included:**
- **HSE/Safety:** ⛔ NEVER for permit-to-work or safety authorization
- **Legal:** NEVER for legal advice or contract interpretation
- **Finance:** NEVER for financial calculations or budget approvals
- **Sales:** NEVER for pricing decisions or contract terms
- **Engineering:** NEVER for engineering calculations or design approval

[See example guardrails →](prompts/role-specific/hse-legal-compliance.md#-hse-critical-guardrails---read-first)

## 📱 Stay Updated

- ⭐ **Star this repo** to get updates when new prompts are added
- 🔔 **Watch releases** for curated prompt pack releases
- 🐦 **Follow on X/Twitter:** [@nerdychefsai](https://x.com/nerdychefsai) for Copilot tips and enterprise AI insights
- 💼 **Follow on LinkedIn:** [Mathieu Kessler](https://linkedin.com/in/mathieukessler) for enterprise AI deployment strategies

## 📄 License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

**This means:**

- ✅ You can use these prompts freely (personal or commercial)
- ✅ You can modify and build upon them
- ✅ You can share them with others
- 📌 You must give appropriate credit
- 📌 Any derivatives must use the same license (stay open-source)

**In practice:**

- Use these prompts in your company ✅
- Build internal tools with them ✅
- Share improvements with the community ✅
- Create a closed-source product repackaging them ❌

## 🙏 Acknowledgments

Built by [Mathieu Kessler](https://linkedin.com/in/mathieukessler) and the team at NerdyChefs.ai.

**Made by people for people who want to work smarter, not harder.**

---

## 🔗 Quick Links

- **[Full Prompt Library](https://nerdychefs.ai)** - 1300+ free AI prompts & tools (no signup)
- **[Kesslernity](https://kesslernity.com)** - Enterprise AI deployment platform
- **[LinkedIn](https://linkedin.com/in/mathieukessler)** - Connect with Mathieu
- **[X/Twitter](https://x.com/nerdychefsai)** - Daily AI productivity tips
- **[Contributing Guide](CONTRIBUTING.md)** - Submit your own prompts
- **[License](LICENSE)** - CC BY-SA 4.0

---

**⚡ Pro Tip:** Star this repo and check back monthly for new prompt additions. We're continuously adding prompts based on enterprise feedback and real-world use cases.
