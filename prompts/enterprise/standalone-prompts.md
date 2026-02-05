# Copilot Enterprise Prompts (Standalone)

Prompts optimized for Microsoft Copilot Enterprise WITHOUT M365 integration. Designed for Copilot's conservative behavior: explicit instructions, structured outputs, and acknowledgment of limitations. Works with copilot.microsoft.com and Copilot in Edge.

> **Note:** These prompts account for key differences between Copilot and ChatGPT. Copilot has stricter safety filters, vision capabilities are more restricted, prefers "no result" over uncertain guesses, and is optimized for fast, safe, explainable answers.

**Category:** Productivity & Tools

**Prompts:** 16

**Categories:** Analysis & Reasoning, Business Writing, Data Processing, Document Analysis, Image Analysis, Technical

---

## Analysis & Reasoning

### 1. Risk Assessment Framework

**Use Case:** Structured risk assessment for projects, decisions, or initiatives

**Target Personas:** Risk Manager, Project Manager, Business Analyst, Executive, Compliance Officer

**Tags:** `Copilot Enterprise`, `Risk Assessment`, `Analysis`, `Standalone`

**Prompt:**
```
You are conducting a structured risk assessment.

Task: Analyze the provided information for risks.

Framework:
For each identified risk, provide:

| Risk ID | Description | Category | Likelihood | Impact | Risk Score | Mitigation |

Categories: Strategic, Operational, Financial, Compliance, Reputational, Technical

Likelihood scale:
1 = Rare (< 5% chance)
2 = Unlikely (5-25%)
3 = Possible (25-50%)
4 = Likely (50-75%)
5 = Almost Certain (> 75%)

Impact scale:
1 = Negligible
2 = Minor
3 = Moderate
4 = Major
5 = Severe

Risk Score = Likelihood × Impact

Instructions:
- Only identify risks explicitly mentioned or strongly implied
- Provide specific, actionable mitigations
- Do not catastrophize or invent unlikely scenarios
- Focus on the top 5-10 most significant risks
- Note any assumptions made

Output also includes:
- Risk heat map summary (High/Medium/Low counts)
- Top 3 risks requiring immediate attention
- Information gaps that prevent complete assessment
```

---

### 2. SWOT Analysis Generator

**Use Case:** Strategic analysis for business planning or competitive assessment

**Target Personas:** Business Analyst, Strategist, Manager, Consultant, Executive

**Tags:** `Copilot Enterprise`, `SWOT`, `Strategy`, `Standalone`

**Prompt:**
```
You are conducting a SWOT analysis.

Task: Generate a structured SWOT analysis from the provided information.

Framework:

**STRENGTHS** (Internal, Positive)
What advantages exist? What is done well?
- [Strength 1]: [Evidence/source]
- [Strength 2]: [Evidence/source]

**WEAKNESSES** (Internal, Negative)
What could be improved? What is done poorly?
- [Weakness 1]: [Evidence/source]
- [Weakness 2]: [Evidence/source]

**OPPORTUNITIES** (External, Positive)
What trends or changes could be beneficial?
- [Opportunity 1]: [Evidence/source]
- [Opportunity 2]: [Evidence/source]

**THREATS** (External, Negative)
What obstacles or risks exist externally?
- [Threat 1]: [Evidence/source]
- [Threat 2]: [Evidence/source]

**Strategic Implications:**
- SO Strategies (use Strengths to capture Opportunities)
- WO Strategies (overcome Weaknesses via Opportunities)
- ST Strategies (use Strengths to mitigate Threats)
- WT Strategies (minimize Weaknesses and avoid Threats)

Constraints:
- Only include items supported by provided information
- Mark items based on assumptions with [Assumed]
- Limit to 3-5 items per quadrant (focus on significant ones)
- Do not invent factors not mentioned or implied
```

---

### 3. Decision Matrix Builder

**Use Case:** Evaluating options for business decisions systematically

**Target Personas:** Manager, Business Analyst, Project Manager, Executive, Procurement Specialist

**Tags:** `Copilot Enterprise`, `Decision Making`, `Analysis`, `Standalone`

**Prompt:**
```
You are building a decision matrix to evaluate options.

Task: Create a structured comparison of alternatives.

Instructions:
1. List all options/alternatives being considered
2. Identify evaluation criteria (from context or suggest common ones)
3. Assign weights to criteria (if not provided, use equal weights)
4. Score each option against each criterion (1-5 scale)
5. Calculate weighted scores
6. Provide recommendation with rationale

Output Format:

**Options:** [List of alternatives]

**Criteria & Weights:**
| Criterion | Weight | Rationale for Weight |

**Scoring Matrix:**
| Option | Criterion 1 | Criterion 2 | ... | Weighted Total |

**Scores Legend:**
1 = Poor, 2 = Below Average, 3 = Average, 4 = Good, 5 = Excellent

**Analysis:**
- Top recommendation: [Option] (Score: X)
- Runner-up: [Option] (Score: Y)
- Key differentiators: [What separates top options]

**Caveats:**
- Assumptions made in scoring
- Criteria that may need expert input
- Factors not captured in this analysis

Constraints:
- Be explicit about scoring rationale
- Note where scores are uncertain
- Do not force a recommendation if options are too close
```

---

## Business Writing

### 4. Meeting Minutes Formatter

**Use Case:** Converting rough meeting notes into professional documentation

**Target Personas:** Administrative Assistant, Project Manager, Executive Assistant, Team Lead, Scrum Master

**Tags:** `Copilot Enterprise`, `Meetings`, `Documentation`, `Enterprise AI`

**Prompt:**
```
You are formatting meeting notes into professional minutes.

Task: Convert raw meeting notes into structured minutes.

Required sections:
1. **Meeting Header**
   - Meeting title
   - Date and time
   - Attendees (present and absent if noted)
   - Meeting type (recurring/ad-hoc)

2. **Agenda Items Discussed**
   - Topic
   - Key discussion points
   - Decisions made

3. **Action Items**
   | Action | Owner | Due Date | Status |

4. **Parking Lot** (items deferred)

5. **Next Meeting** (if mentioned)

Constraints:
- Only include what was explicitly discussed
- Mark unclear ownership as "TBD - needs assignment"
- If due dates not mentioned, mark as "TBD"
- Do not infer decisions that were not explicitly made
- Flag any topics that seem unresolved

Output the formatted minutes, then provide:
- Confidence level for action item extraction
- Questions for meeting organizer (if clarification needed)
```

---

### 5. Professional Email Drafter

**Use Case:** Drafting professional emails for various business situations

**Target Personas:** Professional, Manager, Executive, Sales Representative, Account Manager

**Tags:** `Copilot Enterprise`, `Email`, `Communication`, `Standalone`

**Prompt:**
```
You are drafting a professional business email.

Context needed:
- Recipient: [who is receiving this]
- Purpose: [what you want to achieve]
- Tone: [formal/professional/friendly]
- Key points: [what must be communicated]

Task: Draft an email following business communication best practices.

Structure:
Subject: [Clear, actionable subject line]

[Greeting]

[Opening - context/purpose in 1-2 sentences]

[Body - key points, organized logically]

[Call to action - what you need from recipient]

[Professional closing]

[Signature placeholder]

Guidelines:
- Keep paragraphs to 2-3 sentences
- Use bullet points for multiple items
- Be specific about dates, deadlines, and expectations
- Avoid jargon unless recipient is technical
- Include specific next steps

Output:
Provide the draft email, then list:
- Assumptions made (if context was incomplete)
- Suggested attachments (if applicable)
- Alternative subject lines (2 options)
```

---

### 6. Executive Summary Generator

**Use Case:** Summarizing reports, proposals, or lengthy documents for executives

**Target Personas:** Executive Assistant, Manager, Business Analyst, Project Manager, Consultant

**Tags:** `Copilot Enterprise`, `Summarization`, `Executive`, `Standalone`

**Prompt:**
```
You are creating an executive summary from a longer document.

Task: Generate a concise executive summary.

Instructions:
1. Identify the document purpose and key stakeholders
2. Extract the 3-5 most critical points
3. Note any decisions required or actions recommended
4. Highlight risks or concerns mentioned
5. Keep summary under 250 words

Structure:
**Purpose:** [One sentence on why this document exists]

**Key Findings:**
1. [Most important point]
2. [Second most important]
3. [Third most important]

**Recommendations/Actions:**
- [Action item with owner if mentioned]

**Risks/Concerns:**
- [Any flagged issues]

**Next Steps:**
- [What happens next]

Constraints:
- Use language from the original document
- Do not add opinions or interpretations
- Flag if the document lacks clear conclusions
- If document is too complex for summary, recommend section-by-section approach
```

---

## Data Processing

### 7. Table Data Extractor with Validation

**Use Case:** Extracting data from tables in PDFs or images

**Target Personas:** Data Analyst, Business Analyst, Accountant, Administrative Assistant, Researcher

**Tags:** `Copilot Enterprise`, `Data Extraction`, `Tables`, `Standalone`

**Prompt:**
```
You are extracting data from a table (image or text).

Task: Extract table data into a structured format.

Instructions:
1. Identify column headers (or describe columns if no headers)
2. Extract each row of data
3. Validate data types in each column:
   - Numbers: Note if they appear to be currency, percentages, counts
   - Dates: Note the format used
   - Text: Note if they appear to be codes, names, or descriptions
4. Flag any cells that are unclear or potentially misread

Output Format:
Table Structure:
- Columns: [number]
- Rows: [number, excluding header]
- Data Types: [column → type mapping]

Extracted Data:
[Reproduce table in markdown format]

Validation Notes:
- Uncertain cells: [list with row/column reference]
- Format inconsistencies: [list any issues]
- Missing data: [list empty cells]

Confidence: [HIGH/MEDIUM/LOW] based on clarity

Constraints:
- Mark uncertain values with [?]
- Do not fill in missing values
- Preserve original formatting of numbers/dates
- If table spans multiple pages, note this limitation
```

---

### 8. JSON/XML Structure Generator

**Use Case:** Converting documents or text into machine-readable formats

**Target Personas:** Developer, Data Engineer, Business Analyst, Integration Specialist

**Tags:** `Copilot Enterprise`, `Data Transformation`, `JSON`, `Enterprise AI`

**Prompt:**
```
You are converting unstructured text into structured data.

Task: Parse the provided text and output as structured JSON.

Instructions:
1. Identify all entities mentioned (people, organizations, dates, amounts, etc.)
2. Identify relationships between entities
3. Create a logical JSON structure to represent the information
4. Use consistent naming conventions (camelCase for keys)
5. Use appropriate data types (strings, numbers, booleans, arrays)

Output Format:
{"documentType": "[identified type]", "extractedDate": "[today or document date]", "confidence": "[HIGH/MEDIUM/LOW]", "data": {}, "uncertainFields": []}

Constraints:
- Only include information explicitly stated
- Use null for missing values, not guesses
- Include an "uncertainFields" array for anything ambiguous
- Validate that numbers are actually numbers (not strings)
- Escape special characters properly
```

---

## Document Analysis

### 9. Structured Document Comparison

**Use Case:** Comparing contracts, specifications, or technical documents

**Target Personas:** Business Analyst, Legal Professional, Project Manager, Contract Manager

**Tags:** `Copilot Enterprise`, `Document Analysis`, `Comparison`, `Standalone`

**Prompt:**
```
You are analyzing two documents for comparison.

Task: Compare these documents systematically.

Instructions:
1. First, identify the document type (contract, specification, report, etc.)
2. List all sections/headings present in EACH document
3. For each section, note:
   - Present in Doc A only
   - Present in Doc B only
   - Present in both (compare content)
4. Highlight substantive differences (not formatting)
5. Flag any contradictions or conflicts

Output Format:
Use a structured table with columns:
| Section | Doc A Status | Doc B Status | Key Differences |

Constraints:
- Focus on explicit text content only
- Do not infer meaning from formatting
- If uncertain about a difference, state "Requires human review"
- List findings by importance (critical → minor)
```

---

### 10. Compliance Checklist Generator

**Use Case:** Converting regulations into actionable compliance checklists

**Target Personas:** Compliance Officer, Legal Professional, Risk Manager, Quality Manager, Auditor

**Tags:** `Copilot Enterprise`, `Compliance`, `Checklist`, `Enterprise AI`

**Prompt:**
```
You are creating a compliance checklist from a regulatory document.

Task: Generate an actionable compliance checklist.

Instructions:
1. Identify the regulation/standard being referenced
2. Extract each requirement as a discrete checklist item
3. For each item, determine:
   - Requirement ID (if provided) or generate sequential ID
   - Requirement text (verbatim or summarized)
   - Action required (what must be done)
   - Evidence needed (how to prove compliance)
   - Responsible party type (who typically handles this)

Output Format:
| Req ID | Requirement | Action | Evidence | Owner Type | Status |

Status column should be left as "Pending" for all items.

Constraints:
- Use exact regulatory language where possible
- Do not interpret ambiguous requirements
- Flag items that require legal/expert interpretation
- Group by section or theme for easier review
```

---

### 11. Technical Specification Extractor

**Use Case:** Extracting requirements from RFPs, specs, or technical docs

**Target Personas:** Business Analyst, Engineer, Project Manager, Technical Writer, Procurement Specialist

**Tags:** `Copilot Enterprise`, `Requirements`, `Extraction`, `Enterprise AI`

**Prompt:**
```
You are extracting structured data from a technical document.

Task: Extract all specifications, requirements, and constraints.

Instructions:
1. Identify the document type and domain
2. Extract specifications in these categories:
   - Functional requirements (what it must DO)
   - Technical specifications (measurements, materials, standards)
   - Constraints (limitations, exclusions, boundaries)
   - Dependencies (what it relies on)
   - Acceptance criteria (how to verify)

Output Format:
For each extracted item, provide:
| ID | Category | Specification Text | Source (page/section) | Confidence |

Confidence levels:
- HIGH: Explicitly stated with clear values
- MEDIUM: Stated but requires interpretation
- LOW: Implied or partially visible

Constraints:
- Only extract what is explicitly written
- Do not infer specifications from context
- Mark any ambiguous items for human review
- Preserve original terminology and units
```

---

## Image Analysis

### 12. Engineering Drawing Tag Identifier

**Use Case:** Identifying equipment tags in P&IDs, schematics, or site photos

**Target Personas:** Engineer, Technician, Inspector, Operations Manager, Maintenance Planner

**Tags:** `Copilot Enterprise`, `Vision`, `Engineering`, `Standalone`

**Prompt:**
```
You are assisting with visual inspection of an engineering image.

Task: Visually identify any clearly readable tags in the image.

Pattern to look for: Tags following format like:
- XXX-AAAA-0000 (digits-letters-digits)
- AA-000-BBB (letters-digits-letters)
- Or similar alphanumeric equipment tags

Guidelines:
- Tags may appear horizontally or vertically
- Consider rotated text if clearly legible to a human reader
- Only report tags you can see with HIGH confidence
- Do NOT guess or infer partially visible tags
- Do NOT attempt to read blurry or obscured text

Output Format (plain text table):
| Tag Text | Location (e.g., top-left) | Orientation | Confidence |

Confidence levels:
- HIGH: Clearly readable, no ambiguity
- MEDIUM: Readable but some characters unclear
- (Do not report LOW confidence items)

If no tags are clearly visible, state:
"No confidently readable tags detected. The image may contain tags that require higher resolution or human inspection."
```

---

### 13. Document Layout Analyzer

**Use Case:** Pre-processing document images before detailed analysis

**Target Personas:** Document Controller, Business Analyst, Data Entry Specialist, Administrative Assistant

**Tags:** `Copilot Enterprise`, `Vision`, `Document Processing`, `Enterprise AI`

**Prompt:**
```
You are analyzing the layout and structure of a document image.

Task: Describe the document structure WITHOUT interpreting content.

Instructions:
1. Identify document type (form, letter, report, table, diagram, etc.)
2. Describe the layout structure:
   - Number of columns
   - Presence of headers/footers
   - Tables (rows x columns approximately)
   - Images or diagrams (location, not content)
   - Text blocks (location and approximate size)
3. Note any quality issues affecting readability

Output Format:
Document Type: [identified type]

Layout Structure:
- Columns: [number]
- Header: [yes/no, description]
- Footer: [yes/no, description]
- Tables: [count, approximate dimensions]
- Images: [count, locations]
- Text Blocks: [count, locations]

Quality Assessment:
- Readability: [good/fair/poor]
- Issues: [list any problems]

Constraints:
- Describe structure only, not content
- Do not attempt to OCR or transcribe text
- If layout is unclear, state what is uncertain
- This is a structural assessment, not content analysis
```

---

### 14. Chart and Graph Interpreter

**Use Case:** Extracting data from charts in reports or presentations

**Target Personas:** Business Analyst, Data Analyst, Manager, Executive, Researcher

**Tags:** `Copilot Enterprise`, `Vision`, `Data Visualization`, `Standalone`

**Prompt:**
```
You are interpreting a chart or graph image.

Task: Extract the key information from this visualization.

Instructions:
1. Identify chart type (bar, line, pie, scatter, etc.)
2. Read axis labels and title (if visible)
3. Identify data series/categories shown
4. Extract key values that are CLEARLY labeled
5. Note the overall trend or message

Output Format:
Chart Type: [type]
Title: [if visible, otherwise "Not visible"]

Axes:
- X-axis: [label and range if visible]
- Y-axis: [label and range if visible]

Data Points (only clearly labeled values):
| Category/Series | Value | Notes |

Key Observations:
- [Main trend or insight #1]
- [Main trend or insight #2]

Limitations:
- [What could not be determined from this image]

Constraints:
- Only report values that are explicitly labeled
- Do not estimate or interpolate between data points
- If legend is unclear, describe colors/patterns instead
- State what information is missing or unclear
```

---

## Technical

### 15. Technical Documentation Improver

**Use Case:** Improving clarity and completeness of technical docs

**Target Personas:** Technical Writer, Developer, Product Manager, Documentation Specialist

**Tags:** `Copilot Enterprise`, `Documentation`, `Technical Writing`, `Enterprise AI`

**Prompt:**
```
You are improving technical documentation.

Task: Review and enhance the provided documentation.

Assessment areas:
1. **Completeness**: Are all necessary sections present?
2. **Clarity**: Is it understandable to the target audience?
3. **Accuracy**: Are technical details correct?
4. **Structure**: Is information logically organized?
5. **Examples**: Are there sufficient examples?

Output Format:

**Current State Assessment:**
| Area | Rating (1-5) | Notes |

**Recommended Improvements:**
| Priority | Section | Issue | Suggested Fix |

**Missing Sections:**
- [Section that should be added]

**Revised Version:**
[If requested, provide improved version]

**Style Guide Compliance:**
- [Note any inconsistencies]

Constraints:
- Preserve technical accuracy (don't change facts)
- Maintain author's voice where appropriate
- Note where subject matter expertise is needed
- Focus on clarity over comprehensiveness
- Flag any technical claims you cannot verify
```

---

### 16. Code Review Assistant

**Use Case:** Reviewing code for quality, security, and best practices

**Target Personas:** Developer, Software Engineer, Tech Lead, Code Reviewer, Security Engineer

**Tags:** `Copilot Enterprise`, `Code Review`, `Development`, `Standalone`

**Prompt:**
```
You are reviewing code for quality and issues.

Task: Review the provided code systematically.

Review checklist:
1. **Correctness**: Does it do what it is supposed to?
2. **Security**: Any obvious vulnerabilities?
3. **Performance**: Any inefficiencies?
4. **Readability**: Is it understandable?
5. **Maintainability**: Will it be easy to modify?

Output Format:

**Summary:** [One sentence overall assessment]

**Issues Found:**
| Severity | Line(s) | Issue | Recommendation |

Severity levels:
- Critical: Must fix before merge
- Major: Should fix, significant impact
- Minor: Nice to fix, low impact
- Suggestion: Style/preference

**What is Done Well:**
- [Positive observation 1]
- [Positive observation 2]

**Questions for Author:**
- [Clarification needed]

Constraints:
- Focus on substantive issues, not style nitpicks
- Do not rewrite the code unless asked
- Note if you need more context to review properly
- Be specific about line numbers and issues
- Acknowledge limitations (cannot run the code, do not see full codebase)
```

---

## Footer

**Curated by NerdyChefs** - Enterprise AI prompt engineering for Microsoft Copilot

For more prompts and resources, visit the [awesome-microsoft-copilot-prompts](https://github.com/nerdychefs/awesome-microsoft-copilot-prompts) repository.
