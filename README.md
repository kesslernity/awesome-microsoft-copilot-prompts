# Awesome Microsoft Copilot Prompts 🍳

[![Prompts](https://img.shields.io/badge/prompts-299-blue)](https://nerdychefs.ai)
[![Categories](https://img.shields.io/badge/categories-15-green)](https://nerdychefs.ai)
[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)](/LICENSE)
[![Enterprise](https://img.shields.io/badge/enterprise-tested-purple)](https://kesslernity.com)

> The definitive Microsoft 365 Copilot prompt library for enterprise professionals. **349 prompts total** - from Quick Start basics to battle-tested enterprise workflows—not generic AI fluff.

**Why this repo exists:** Most AI prompt libraries are generic ChatGPT recycling. This collection focuses exclusively on **Microsoft Copilot** across Office 365 apps, built from real enterprise deployments and proven in production environments.

**New to Copilot?** Start with our [Quick Start Guide](prompts/QUICK-START.md) - 50 prompts that work in any Copilot (free or M365).  
**Using M365 Copilot?** Explore our 299 advanced prompts that leverage your organizational data.

## 🎯 What Makes This Different

- **Copilot-Specific:** Every prompt optimized for Microsoft Copilot
- **Role-Based:** Organized by job function, not random categories
- **Enterprise-Ready:** Real prompts from production deployments, not theoretical examples
- **Zero Fluff:** No "write me a poem about spreadsheets"—these solve actual business problems

## 🤔 Why ChatGPT Prompts Don't Work in Copilot

**Short answer:** Copilot and ChatGPT are fundamentally different tools. Same AI foundation, completely different capabilities.

### Key Differences

| Feature | ChatGPT | Microsoft Copilot |
|---------|---------|-------------------|
| **Data Access** | None - you paste content | Full access to your M365 data (emails, files, meetings) |
| **Integration** | Standalone chat | Embedded in Office apps |
| **Actions** | Text responses only | Can edit files, send emails, create charts |
| **Context** | Conversation only | Your entire work environment |
| **Safety Mode** | Exploratory | Enterprise-safe (conservative by design) |

### Why This Matters for Prompts

**Generic ChatGPT Prompt:**
```
"Summarize my emails from this week"
```
❌ **Result:** "I don't have access to your emails. Please paste them here."

**Copilot-Optimized Prompt:**
```
"Analyze emails from the last 7 days about the Q2 budget review. 
Create a summary table with: key decisions, action items, blockers, 
and budget impact. Format for my VP."
```
✅ **Result:** Copilot accesses Outlook directly, analyzes threads with full context, creates formatted output

### Copilot's Strengths & Limitations

**✅ What Copilot Does Well:**
- Compare multiple documents (PDFs, specs, procedures)
- Summarize long technical content
- Cross-reference requirements across files
- Reason over text-heavy documents
- Assist with review, clarification, and consistency checks

**⚠️ Known Limitations (By Design):**
- Conservative with visual analysis (better to say "I don't know" than guess wrong)
- Limited OCR on complex diagrams, P&IDs, or dense schematics
- No pixel-level precision on images
- Strict confidence thresholds (enterprise-safe execution mode)

**🎯 Bottom Line:** Copilot is a production assistant, not an exploratory lab tool. It helps you work faster with your actual data — but humans still validate.

### Want to Master Copilot Prompting?

👉 **[Free Course: Copilot Prompt Engineering](https://www.nerdychefs.ai/copilot/module-7)** - Learn why these prompts work

Topics: Architecture differences, the 4-question framework, common mistakes, advanced techniques.

## 🚀 Quick Start - Universal Prompts

**New to Copilot?** Start here with prompts that work in **BOTH** free Copilot (web) and M365 Copilot.

### ✨ Works Everywhere
These 50 prompts don't require M365 integration - perfect for:
- Testing Copilot before buying M365 license
- One-off tasks outside your organizational data
- Learning prompt basics
- Anyone using free Copilot (copilot.microsoft.com)

### 📚 Categories in Quick Start Guide:
- **Writing & Communication** (10 prompts) - Professional emails, responses, difficult conversations
- **Learning & Research** (10 prompts) - Concept explanations, comparisons, decision frameworks
- **Content Creation** (10 prompts) - Blog outlines, social captions, presentations, video scripts
- **Planning & Organization** (10 prompts) - Meeting agendas, priority planning, goal breakdowns, delegation
- **Analysis & Problem-Solving** (10 prompts) - Data analysis, root cause, risk assessment, troubleshooting

👉 **[View Quick Start Guide →](prompts/QUICK-START.md)**

**Ready for advanced workflows?** The 299 prompts below require M365 Copilot (they access your actual emails, files, and organizational data for deeper intelligence).

---

## 📊 Quick Stats

- **299 Total Prompts** across 15 specialized collections
- **26 Power User Prompts** for advanced Copilot mastery
- **70 Outlook Prompts** for email intelligence and automation
- **203 Role-Specific Prompts** covering 12 business functions
- **Tested in Production** by enterprise users

## 🚀 Advanced Start

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

[See 69 more Outlook prompts →](prompts/outlook/)

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

[See more Excel prompts →](prompts/power-users/)

## 📚 Browse by Category

### Power Users & Advanced Techniques
- [**AI for Microsoft Copilot Power Users**](prompts/power-users/) (26 prompts)
  - Advanced email intelligence
  - Excel data intelligence
  - PowerPoint automation
  - Cross-app workflows

### Email & Communication Mastery
- [**Advanced Outlook Automation**](prompts/outlook/advanced-automation.md) (20 prompts)
- [**Advanced Outlook Prompt Pack**](prompts/outlook/advanced-prompts.md) (50 prompts)

### Role-Specific Collections

#### Business Operations
- [**Administrative & Executive Assistants**](prompts/role-specific/admin-executive-assistants.md) (17 prompts)
- [**Commercial Operations**](prompts/role-specific/commercial-operations.md) (18 prompts)
- [**Project Leadership**](prompts/role-specific/project-leadership.md) (18 prompts)

#### Revenue & Growth
- [**Sales & Business Development**](prompts/role-specific/sales-business-development.md) (16 prompts)
- [**Marketing & Communications**](prompts/role-specific/marketing-communications.md) (16 prompts)
- [**Customer Success & Support**](prompts/role-specific/customer-success-support.md) (16 prompts)

#### Professional Services
- [**Consulting & Professional Services**](prompts/role-specific/consulting-professional-services.md) (16 prompts)
- [**Engineering & Construction**](prompts/role-specific/engineering-construction.md) (16 prompts)

#### Corporate Functions
- [**Finance & HR**](prompts/role-specific/finance-hr.md) (18 prompts)
- [**HSE, Legal & Compliance**](prompts/role-specific/hse-legal-compliance.md) (20 prompts)

#### Specialized Functions
- [**Research & Development**](prompts/role-specific/research-development.md) (16 prompts)
- [**Supply Chain & Logistics**](prompts/role-specific/supply-chain-logistics.md) (16 prompts)

## 💡 How to Use These Prompts

### 1. Find Your Use Case
Browse by role or search for your specific need (e.g., "email prioritization", "data analysis", "meeting prep").

### 2. Copy & Customize
Each prompt is designed to work immediately but customize the placeholders:
- `[TOPIC]` → your specific subject
- `[TIMEFRAME]` → your desired period
- `[METRIC]` → your KPI or measurement

### 3. Run in Copilot
Paste the prompt into the appropriate Microsoft 365 app:
- **Outlook:** Use in Outlook Copilot chat
- **Excel:** Use in Excel Copilot sidebar
- **Word:** Use in Word Copilot drafting
- **PowerPoint:** Use in PowerPoint Copilot designer
- **Teams:** Use in Teams Copilot chat

### 4. Iterate & Improve
Copilot learns from context. If the first result isn't perfect, provide feedback: "Make it more concise" or "Focus on Q4 data only".

## 🔥 Most Popular Prompts

1. **360° Relationship Mapper** - Map stakeholder relationships from email patterns
2. **Early Warning System** - Predict which topics will become future problems
3. **Dashboard Insight Generator** - Turn Excel data into executive dashboards
4. **Email Battle Plan Generator** - Strategic inbox prioritization
5. **Context Fusion Engine** - Synthesize project status across all communications

[See all power user prompts →](prompts/power-users/)

## 🏢 Enterprise Deployment

Using Copilot across your organization? These prompts work even better when deployed enterprise-wide.

**Need help with:**
- Microsoft 365 Copilot rollout strategy
- Custom Copilot Studio agents
- Enterprise prompt governance
- Team training and adoption

👉 **[Check out Kesslernity](https://kesslernity.com)** - Enterprise AI deployment platform ($249-$1,999/month + training services)

## 🌐 Full Prompt Library

This repo contains **299 prompts** optimized. For the complete searchable library with:
- Advanced filtering by role, use case, and app
- Copy-to-clipboard functionality
- Regular updates with new prompts
- No signup required

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

### Iterate Don't Restart
If the output isn't right:
- Add constraints: "Make it shorter" or "Focus only on risks"
- Provide examples: "Like the format we used last quarter"
- Correct mistakes: "The deadline is March 15, not May 15"

For comprehensive prompt engineering guidance:  
👉 [Anthropic's Prompt Engineering Guide](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)

## 📱 Stay Updated

- ⭐ **Star this repo** to get updates when new prompts are added
- 🔔 **Watch releases** for curated prompt pack releases
- 🐦 **Follow on X/Twitter:** [@nerdychefsai](https://x.com/nerdychefsai) for Copilot tips and enterprise AI insights

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

**Made with ❤️ for people who want to work smarter, not harder.**

---

**🔗 Links:**
- [NerdyChefs.ai](https://nerdychefs.ai) - Full prompt library (1300+ prompts)
- [Kesslernity](https://kesslernity.com) - Enterprise AI deployment
- [LinkedIn](https://linkedin.com/in/mathieukessler) - Connect with Mathieu
- [X/Twitter](https://x.com/nerdychefsai) - Daily AI productivity tips
