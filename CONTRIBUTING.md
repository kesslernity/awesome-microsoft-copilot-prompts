# Contributing to Awesome Microsoft Copilot Prompts

Thank you for your interest in contributing to our collection of Microsoft Copilot prompts! This guide will help you submit high-quality prompts that benefit the entire community.

## 📋 Table of Contents

- [Quality Standards](#-quality-standards)
- [Prompt Format Requirements](#-prompt-format-requirements)
- [How to Submit](#-how-to-submit)
- [Review Process](#-review-process)
- [Categories and Tags](#-categories-and-tags)
- [Code of Conduct](#-code-of-conduct)
- [Questions?](#-questions)

## 🎯 Quality Standards

We only accept prompts that meet the following criteria:

### Must Have

1. **Production-Tested** - The prompt must have been used in real work scenarios, not just theoretically designed
2. **Copilot-Specific** - Must work specifically with Microsoft Copilot (not generic AI prompts)
3. **Business Value** - Solves a real business problem or significantly improves productivity
4. **Clear Use Case** - Includes specific scenarios where the prompt is useful
5. **Target Audience** - Defines who would benefit from this prompt

### Nice to Have

- Multiple variations for different contexts
- Tips for customization
- Known limitations documented
- Examples of expected output

### Not Accepted

- Generic prompts that work the same on any AI (ChatGPT, Claude, etc.)
- Prompts for personal/non-work use
- Prompts that could violate enterprise policies
- Prompts that attempt to bypass safety features
- Prompts with placeholder-only content (no actual substance)

## 📝 Prompt Format Requirements

All prompts must follow this exact structure:

```markdown
### [Prompt Number]. [Prompt Name]

**Use Case:** [Specific scenario where this prompt is useful]

**Target Personas:** [Job roles that would benefit, comma-separated]

**Tags:** `tag1`, `tag2`, `tag3`

**Prompt:**

\```
[The actual prompt text goes here]
\```

---
```

### Example

```markdown
### 1. Weekly Status Synthesis

**Use Case:** Synthesize a week of scattered communications into a coherent status report

**Target Personas:** Project Manager, Program Manager, Delivery Manager

**Tags:** `Microsoft Copilot`, `Microsoft 365`, `Status Report`, `Project Management`

**Prompt:**

\```
Review all my emails, Teams messages, and meeting notes from the past week related to [Project Name]. Provide:

1. Progress highlights — what got done
2. Key issues raised — with who raised them
3. Decisions made or pending
4. Risks or concerns mentioned
5. Client/stakeholder feedback
6. Actions assigned and their status

Format as a draft status report. Flag areas where information seems incomplete or conflicting.
\```

---
```

## 🚀 How to Submit

### Option 1: Pull Request (Preferred)

1. **Fork** this repository
2. **Create a branch** for your contribution: `git checkout -b add-prompt-name`
3. **Add your prompt** to the appropriate category file in `/prompts/`
4. **Follow the format** exactly as specified above
5. **Test your prompt** in Microsoft 365 Copilot before submitting
6. **Submit a Pull Request** with:
   - Clear title: "Add: [Prompt Name] to [Category]"
   - Description of what the prompt does
   - Confirmation that you've tested it in production

### Option 2: Issue Submission

If you're not comfortable with pull requests:

1. Open a new **Issue**
2. Use the title format: "[Prompt Submission] Your Prompt Name"
3. Include all required fields from the format above
4. Describe your testing and use case

## 🔍 Review Process

All submissions go through the following review:

1. **Format Check** - Does it follow the required structure?
2. **Quality Review** - Does it meet our quality standards?
3. **Technical Review** - Does it work correctly with Microsoft Copilot?
4. **Category Fit** - Is it in the right collection?
5. **Duplicate Check** - Is there already a similar prompt?

### Timeline

- Initial response: Within 7 days
- Full review: Within 14 days
- Revisions may be requested

### Review Feedback

We may ask you to:
- Clarify the use case
- Add more specific target personas
- Adjust the prompt for better Copilot compatibility
- Move to a different category
- Combine with an existing similar prompt

## 🏷️ Categories and Tags

### Available Categories

| Category | Description | Location |
|----------|-------------|----------|
| Power Users | Advanced cross-app prompts | `/prompts/power-users/` |
| Outlook Automation | Email-specific prompts | `/prompts/outlook/` |
| Enterprise Standalone | Works without M365 integration | `/prompts/enterprise/` |
| Quick Start | Universal beginner prompts | `/prompts/quick-start/` |
| Role-Specific | Job function prompts | `/prompts/role-specific/` |

### Required Tags

Every prompt must include these tag types:

- **Platform tag:** `Microsoft Copilot`, `Microsoft 365`
- **App tag (if applicable):** `Outlook`, `Excel`, `Word`, `PowerPoint`, `Teams`
- **Category tag:** `Productivity`, `Analysis`, `Communication`, etc.
- **Audience tag:** `Executive`, `Manager`, `Individual Contributor`, etc.

### Common Tags

```
Microsoft Copilot, Microsoft 365, Productivity, Office, Work Users,
Outlook, Email Management, Meeting Prep, Status Report, Analysis,
Executive, Manager, Project Manager, Team Lead, Individual Contributor,
Enterprise, Governance, Guardrails, Safety
```

## 📜 Code of Conduct

### Be Respectful

- Provide constructive feedback on others' submissions
- Welcome newcomers and help them improve their contributions
- Respect different work cultures and industries

### Be Professional

- All prompts should be appropriate for enterprise use
- No prompts that could be used for harmful purposes
- No discriminatory or offensive content

### Be Honest

- Only submit prompts you've actually tested
- Acknowledge if a prompt has limitations
- Don't claim others' work as your own

### Be Collaborative

- Build on existing prompts rather than duplicating
- Share improvements to existing prompts
- Help document edge cases and limitations

## 🆘 Questions?

### Before Submitting

- **Is my prompt Copilot-specific?** If it works the same on ChatGPT without modification, it's probably too generic.
- **Have I tested it?** We require real-world testing, not theoretical prompts.
- **Does it add value?** Compare to existing prompts in the same category.

### Getting Help

- Open an **Issue** with the label "question"
- Tag maintainers in your PR if stuck
- Check existing issues for similar questions

### Contact

- **GitHub Issues:** For prompt-related questions
- **Twitter/X:** [@nerdychefsai](https://x.com/nerdychefsai)
- **LinkedIn:** [Mathieu Kessler](https://linkedin.com/in/mathieukessler)

---

## 🎉 Recognition

Contributors who submit accepted prompts will be:

- Listed in the Contributors section of the README
- Credited in the prompt itself (if desired)
- Featured in our monthly contributor highlights

Thank you for helping make Microsoft Copilot more useful for everyone!

---

**Made with ❤️ by [NerdyChefs.ai](https://nerdychefs.ai)**
