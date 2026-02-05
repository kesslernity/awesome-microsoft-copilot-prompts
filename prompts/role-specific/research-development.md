# Copilot for Research & Development

> Master Microsoft 365 Copilot for research and development roles. Contains production-safe prompts for R&D Engineers, Product Researchers, and Scientists with role-specific guardrails.

---

**REQUIRES:** Microsoft 365 Copilot with full M365 integration (Outlook, Teams, SharePoint). These prompts access your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

---

**Category:** Engineering & DevOps

**Prompts:** 16

---

## R&D Copilot Guardrails

> **IMPORTANT:** Read these guardrails before using any R&D prompts. These limitations protect your intellectual property and ensure appropriate use.

### When NOT to Use Copilot for Research & Development

**R&D ENGINEERS — NEVER use Copilot for:**
- Engineering calculations (use proper tools)
- Simulation or modeling (use simulation software)
- CAD or design work
- Code development (use IDE with proper tools)
- Patent drafting (requires IP counsel)
- Safety-critical design decisions
- Test data analysis (use analysis tools)
- Quality certifications

**PRODUCT RESEARCHERS — NEVER use Copilot for:**
- Statistical analysis (use R, SPSS, etc.)
- Survey creation (use survey tools)
- Participant recruitment (use proper channels)
- PII handling (follow privacy protocols)
- Research ethics decisions
- Data collection (use research tools)
- Quantitative analysis (use analytics tools)

**SCIENTISTS — NEVER use Copilot for:**
- Data analysis (use proper statistical tools)
- Lab calculations (verify independently)
- Protocol design (requires peer review)
- Safety assessments
- Regulatory submissions
- Clinical decisions
- Intellectual property filing
- Peer review responses (personal judgment)

### IP & Confidentiality Warnings

- Never include proprietary formulas or algorithms
- Be careful with pre-patent disclosure
- Remember prompts may be logged
- Competitive technology discussions need care
- Export control considerations apply
- Research data handling follows specific protocols

### Golden Rules

- **R&D Engineers:** "Copilot retrieves — engineers innovate"
- **Product Researchers:** "Copilot synthesizes — researchers discover"
- **Scientists:** "Copilot organizes — scientists discover"

### System Integration Note

Copilot does NOT integrate with:
- Lab information management systems (LIMS)
- Electronic lab notebooks (ELN)
- PLM/PDM systems
- Statistical software (R, SPSS, SAS)
- CAD/CAE tools
- Research databases (PubMed, etc.)

---

## Prompts

### Collaboration

---

### 1. Collaboration Network Search

**Use Case:** Map research collaboration network from communications.

**Target Personas:** Research Scientist, Principal Investigator, Research Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `collaboration`, `network`

**Prompt:**
```
Search for mentions of collaborations or collaborators in [Research Field]. Identify:
- External researchers we've worked with
- Institutions mentioned
- Successful collaborations
- Potential collaboration opportunities
- Conference connections
- Co-authorship history

This is for collaboration planning.
```

---

### 2. Cross-Team Collaboration Summary

**Use Case:** Track cross-team R&D collaboration from communications.

**Target Personas:** R&D Engineer, Project Lead, Research Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `collaboration`, `cross-team`

**Prompt:**
```
Search for discussions about collaboration with [Other Team/Department] on [Topic]. Summarize:
- What was agreed upon
- Who the key contacts are
- Deliverables committed
- Timeline discussed
- Open items
- Any conflicts or concerns

This is for coordination planning.
```

---

### Competitive Research

---

### 3. Competitive Analysis Research

**Use Case:** Gather internal competitive insights from discussions.

**Target Personas:** Product Researcher, Product Manager, Strategy Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `competitive`, `analysis`

**Prompt:**
```
Search for internal discussions about [Competitor] or competitive products. Find:
- Feature comparisons mentioned
- Strengths and weaknesses discussed
- Customer feedback about competitors
- Pricing information shared
- Strategic responses considered

Compile as competitive intelligence summary. Validate with current market data.
```

---

### Experiment Tracking

---

### 4. Experiment Documentation Search

**Use Case:** Find historical experiment documentation from communications.

**Target Personas:** R&D Engineer, Research Scientist, Lab Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `experiments`, `documentation`

**Prompt:**
```
Search for documentation and discussions about experiments related to [Project/Technology]. Find:
- Experiment designs discussed
- Results shared
- Parameter variations tested
- Failures and their causes
- Success criteria defined
- Data locations mentioned

Compile as experiment history reference.
```

---

### Funding

---

### 5. Grant/Funding Research

**Use Case:** Gather funding and grant context from internal discussions.

**Target Personas:** Research Scientist, Principal Investigator, Research Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `funding`, `grants`

**Prompt:**
```
Search for discussions about funding or grants related to [Research Area]. Find:
- Funding sources mentioned
- Application experiences shared
- Success/failure lessons
- Collaborators for proposals
- Deadlines discussed
- Budget guidance

This is for funding application planning.
```

---

### Lab Management

---

### 6. Lab/Equipment Discussion Summary

**Use Case:** Track lab and equipment discussions for resource planning.

**Target Personas:** Research Scientist, Lab Manager, Research Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `lab`, `equipment`

**Prompt:**
```
Search for discussions about [Equipment/Facility/Resource]. Find:
- Availability discussions
- Booking or scheduling mentions
- Technical issues reported
- Training requirements
- Maintenance concerns
- Alternative resources mentioned

This is for resource planning.
```

---

### Literature Review

---

### 7. Literature Discussion Summary

**Use Case:** Organize literature review discussions and references.

**Target Personas:** Research Scientist, Data Scientist, Principal Investigator

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `literature`, `review`

**Prompt:**
```
You are assisting a research scientist. Search for discussions about [Paper/Topic/Author]. Compile:
- Papers mentioned and their relevance
- Key findings discussed
- Methodological critiques raised
- Application ideas proposed
- Follow-up reading suggested
- Experts identified internally

This is for literature review organization.
```

---

### Publication

---

### 8. Publication Planning Summary

**Use Case:** Track publication planning from research communications.

**Target Personas:** Research Scientist, Principal Investigator, Research Fellow

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `publication`, `planning`

**Prompt:**
```
Search for discussions about publishing research on [Topic]. Compile:
- Journals considered
- Timeline discussions
- Co-author coordination
- Reviewer feedback mentioned
- Revision strategies
- Submission requirements discussed

This is for publication project management.
```

---

### Requirements

---

### 9. Technical Specifications Search

**Use Case:** Gather technical requirements from R&D discussions.

**Target Personas:** R&D Engineer, Systems Engineer, Technical Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `specifications`, `requirements`

**Prompt:**
```
Find technical specifications and requirements discussed for [Component/System]. Compile:
- Performance requirements mentioned
- Interface specifications discussed
- Constraints identified
- Test criteria discussed
- Standards references
- Design trade-offs debated

I need this for specification documentation.
```

---

### Research Communication

---

### 10. Stakeholder Research Brief

**Use Case:** Create stakeholder research briefs from findings discussions.

**Target Personas:** Product Researcher, UX Researcher, Research Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `research`, `stakeholder`

**Prompt:**
```
Draft a research findings brief for [Stakeholder/Team] about [Research Topic]. Based on recent research discussions:
- Key findings to highlight
- Recommendations mentioned
- Data points shared
- Implications for product decisions
- Next steps proposed

Format as executive summary. I will add visuals and detailed data.
```

---

### Research Planning

---

### 11. Prior Art Research Summary

**Use Case:** Gather internal knowledge about previous R&D efforts. Formal IP search requires legal.

**Target Personas:** R&D Engineer, Research Scientist, Innovation Engineer

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `research`, `prior-art`

**Prompt:**
```
You are assisting an R&D engineer. Search my emails, Teams, and SharePoint for discussions about [Technology/Approach]. Compile:
- Previous attempts or prototypes mentioned
- Lessons learned documented
- Technical challenges encountered
- Solutions that worked
- Team members with relevant experience
- Related patents or IP discussions

This is internal research only. Formal prior art search requires legal/IP team.
```

---

### 12. Research Study Planning

**Use Case:** Research study planning using past study learnings.

**Target Personas:** Product Researcher, UX Researcher, Research Lead

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `research`, `planning`

**Prompt:**
```
I'm planning a research study on [Topic]. Search for:
- Similar studies we've conducted
- Methodologies that worked
- Participant recruitment approaches
- Tools and platforms used
- Lessons learned from past studies
- Stakeholders to involve

Compile as study planning reference.
```

---

### Research Strategy

---

### 13. Research Theme Analysis

**Use Case:** Identify research themes from discussions. Use research tools for formal analysis.

**Target Personas:** Product Researcher, Research Manager, Head of Research

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `themes`, `experimental`

**Prompt:**
```
Review research-related discussions over the past [timeframe]. Identify emerging themes:
- Recurring user problems
- Feature requests patterns
- Market trends mentioned
- Technology directions discussed
- Strategic opportunities noted

This is input for research roadmap planning.

EXPERIMENTAL: May miss insights from formal research reports. Use research repository for comprehensive analysis.
```

---

### Technical Review

---

### 14. Technical Review Preparation

**Use Case:** Prepare for R&D technical reviews with comprehensive context.

**Target Personas:** R&D Engineer, Technical Lead, Engineering Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `review`, `preparation`

**Prompt:**
```
I have a technical review meeting for [Project Name]. Search for:
- Technical progress discussed
- Challenges raised by the team
- Design decisions made
- Open questions or debates
- Resource needs mentioned
- Timeline concerns

Compile as technical review prep notes.
```

---

### User Research

---

### 15. User Research Summary

**Use Case:** Synthesize user research findings from communications.

**Target Personas:** Product Researcher, UX Researcher, Product Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `r&d`, `user-research`, `synthesis`

**Prompt:**
```
You are assisting a product researcher. Search for user research discussions related to [Feature/Product]. Compile:
- User feedback captured
- Pain points identified
- Feature requests mentioned
- Usability issues discussed
- User segments mentioned
- Research methodologies used

This is for research synthesis.
```

---

### Governance

---

### 16. R&D Copilot Guardrails Reference

**Use Case:** Essential guardrails for R&D professionals using Copilot.

**Target Personas:** R&D Engineer, Product Researcher, Research Scientist

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `r&d`, `research`

**Prompt:**
```
## When NOT to Use Copilot for Research & Development

**R&D ENGINEERS — NEVER use Copilot for:**
- Engineering calculations (use proper tools)
- Simulation or modeling (use simulation software)
- CAD or design work
- Code development (use IDE with proper tools)
- Patent drafting (requires IP counsel)
- Safety-critical design decisions
- Test data analysis (use analysis tools)
- Quality certifications

**PRODUCT RESEARCHERS — NEVER use Copilot for:**
- Statistical analysis (use R, SPSS, etc.)
- Survey creation (use survey tools)
- Participant recruitment (use proper channels)
- PII handling (follow privacy protocols)
- Research ethics decisions
- Data collection (use research tools)
- Quantitative analysis (use analytics tools)

**SCIENTISTS — NEVER use Copilot for:**
- Data analysis (use proper statistical tools)
- Lab calculations (verify independently)
- Protocol design (requires peer review)
- Safety assessments
- Regulatory submissions
- Clinical decisions
- Intellectual property filing
- Peer review responses (personal judgment)

**IP & Confidentiality Warnings:**
- Never include proprietary formulas or algorithms
- Be careful with pre-patent disclosure
- Remember prompts may be logged
- Competitive technology discussions need care
- Export control considerations apply
- Research data handling follows specific protocols

**Golden Rules:**
- R&D Engineers: "Copilot retrieves — engineers innovate"
- Product Researchers: "Copilot synthesizes — researchers discover"
- Scientists: "Copilot organizes — scientists discover"

**System Integration Note:**
Copilot does NOT integrate with:
- Lab information management systems (LIMS)
- Electronic lab notebooks (ELN)
- PLM/PDM systems
- Statistical software (R, SPSS, SAS)
- CAD/CAE tools
- Research databases (PubMed, etc.)
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1300+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
