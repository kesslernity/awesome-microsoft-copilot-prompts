# Copilot for Supply Chain & Logistics

> Master Microsoft 365 Copilot for supply chain and logistics roles. Contains production-safe prompts for Supply Chain Managers, Logistics Coordinators, and Inventory Planners with role-specific guardrails.

> [!WARNING]
> **REQUIRES: Microsoft 365 Copilot** with full M365 integration (Outlook, Teams, SharePoint). These prompts access your organizational data and will NOT work with the free Microsoft Copilot web version, ChatGPT, or other AI assistants.

**Category:** Operations & Support

**Prompts:** 16

---

## Supply Chain & Logistics Copilot Guardrails

> [!CAUTION]
> **Essential guardrails for supply chain and logistics professionals using Copilot.**

### When NOT to Use Copilot for Supply Chain & Logistics

**SUPPLY CHAIN MANAGERS - NEVER use Copilot for:**
- Purchase order creation (use ERP)
- Supplier payments or approvals
- Contract execution
- Demand forecasting (use planning tools)
- Inventory calculations (use WMS/ERP)
- Supplier qualification decisions
- Compliance certifications
- Risk scoring (use risk tools)

**LOGISTICS COORDINATORS - NEVER use Copilot for:**
- Shipment booking (use TMS)
- Carrier rate negotiations
- Customs declarations
- Dangerous goods documentation
- Delivery commitments to customers
- Tracking data (use TMS)
- Claims processing
- Route optimization (use routing tools)

**INVENTORY PLANNERS - NEVER use Copilot for:**
- Reorder point calculations (use planning tools)
- Safety stock calculations
- Demand forecasting (use forecasting tools)
- Inventory valuation (use ERP)
- Write-off approvals
- Cycle count reconciliation
- ABC classification (use analytics)
- MRP runs (use ERP)

**Data & Compliance Warnings:**
- Never include pricing details in prompts
- Be careful with supplier confidential information
- Follow trade compliance requirements
- Customs data requires proper systems
- Hazmat information requires certified systems

**Golden Rules:**
- Supply Chain: "Copilot researches - supply chain decides"
- Logistics: "Copilot tracks context - logistics executes"
- Inventory: "Copilot finds context - planners optimize"

**System Integration Note:**
Copilot does NOT integrate with:
- ERP systems (SAP, Oracle, NetSuite)
- WMS (Warehouse Management Systems)
- TMS (Transportation Management Systems)
- Demand planning tools
- Customs/trade compliance systems

---

## Carrier Management

### 1. Carrier Performance Research

**Use Case:** Gather carrier feedback from communications for performance review.

**Target Personas:** Logistics Coordinator, Transportation Manager, Freight Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `logistics`, `carrier`, `performance`

**Prompt:**
```
Search for discussions about [Carrier Name] performance. Find:
- On-time delivery mentions
- Damage or loss incidents
- Pricing concerns
- Service issues raised
- Communication quality
- Claims discussions

This is input for carrier scorecard. Formal metrics from TMS.
```

---

## Contract Management

### 2. Contract Negotiation Research

**Use Case:** Research contract context from discussions. Legal review required for terms.

**Target Personas:** Supply Chain Manager, Procurement Manager, Category Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `supply-chain`, `contract`, `negotiation`

**Prompt:**
```
Search for discussions related to our contract with [Supplier Name]. Find:
- Terms that have been pain points
- Pricing history mentioned
- Volume commitments discussed
- SLA concerns raised
- Competitor pricing mentioned
- Relationship dynamics

This is research for negotiation prep. Actual contract terms require legal review.
```

---

## Customer Communication

### 3. Customer Delivery Communication

**Use Case:** Draft customer delivery updates for review and verification.

**Target Personas:** Logistics Coordinator, Customer Service, Order Management

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `logistics`, `customer`, `communication`

**Prompt:**
```
Draft an update email to [Customer Name] about their order [Order Number]. Include:
- Current shipment status
- Expected delivery date
- Any delays and reasons (carefully worded)
- Tracking information placeholder
- Apology if applicable
- Contact for questions

Keep tone professional and helpful. I will verify details before sending.
```

---

## Customs & Compliance

### 4. Customs Issue Research

**Use Case:** Find precedents for customs issues to inform resolution.

**Target Personas:** Logistics Coordinator, Import/Export Specialist, Customs Broker

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `logistics`, `customs`, `compliance`

**Prompt:**
```
Search for discussions about customs issues with [Shipment/Product/Country]. Find:
- Clearance problems encountered
- Documentation requirements discussed
- Broker communications
- Resolution approaches used
- Compliance concerns raised
- Delays and impacts

This is research to resolve current customs issue.
```

---

## Demand Planning

### 5. Demand Signal Summary

**Use Case:** Gather qualitative demand signals from communications for planning input.

**Target Personas:** Inventory Planner, Demand Planner, Supply Planner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `inventory`, `demand`, `planning`

**Prompt:**
```
You are assisting an inventory planner. Search for discussions about demand for [Product/SKU/Category]. Compile:
- Sales forecasts mentioned
- Customer order discussions
- Promotion impacts discussed
- Seasonal patterns mentioned
- New customer/market signals
- Cannibalization concerns

This is input for demand planning. Actual forecast in planning system.
```

---

## Disruption Management

### 6. Disruption Response Summary

**Use Case:** Document disruption response from communications for review and lessons learned.

**Target Personas:** Supply Chain Manager, Logistics Manager, Operations Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `supply-chain`, `disruption`, `crisis`

**Prompt:**
```
Search for all communications about the [disruption event - e.g., port closure, supplier issue]. Compile:
- Timeline of impact
- Affected products/shipments
- Actions taken
- Stakeholder communications
- Recovery timeline discussed
- Lessons mentioned

This is for the disruption debrief.
```

---

## Inventory Management

### 7. Stock Issue Research

**Use Case:** Research stock issue history from communications.

**Target Personas:** Inventory Planner, Inventory Analyst, Supply Chain Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `inventory`, `stockout`, `investigation`

**Prompt:**
```
Search for discussions about stock issues with [Product/SKU]. Find:
- Stockout incidents mentioned
- Root causes discussed
- Customer impact reported
- Resolution actions taken
- Prevention measures proposed
- Responsible parties

This is for stock issue investigation.
```

---

## Inventory Optimization

### 8. Excess Inventory Discussion

**Use Case:** Research excess inventory discussions for optimization planning.

**Target Personas:** Inventory Planner, Inventory Manager, Finance Partner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `inventory`, `excess`, `optimization`

**Prompt:**
```
Search for discussions about excess or slow-moving inventory. Find:
- Products flagged as excess
- Root causes discussed
- Disposition options mentioned
- Write-off discussions
- Promotion possibilities
- Prevention ideas

Compile for inventory optimization review.
```

---

## Launch Planning

### 9. Product Launch Planning

**Use Case:** Gather product launch context for inventory planning.

**Target Personas:** Inventory Planner, New Product Planner, Supply Chain Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `inventory`, `launch`, `planning`

**Prompt:**
```
Search for discussions about the launch of [New Product]. Compile:
- Launch timeline discussions
- Initial quantity estimates
- Supplier readiness mentioned
- Distribution requirements
- Ramp-up plans
- Risk concerns raised

This is input for launch inventory planning.
```

---

## Planning

### 10. S&OP Meeting Preparation

**Use Case:** Prepare for S&OP meetings with context from cross-functional discussions.

**Target Personas:** Supply Chain Manager, Demand Planner, Operations Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `supply-chain`, `sop`, `planning`

**Prompt:**
```
I have a Sales & Operations Planning meeting. Search for recent discussions about:
- Demand signals from sales
- Supply constraints mentioned
- Capacity issues raised
- New product launches discussed
- Inventory concerns
- Budget or cost pressures

Compile as S&OP prep notes. Actual data comes from ERP/planning systems.
```

---

## Process Improvement

### 11. Inventory Pattern Analysis

**Use Case:** Identify inventory planning themes from discussions. Use analytics for metrics.

**Target Personas:** Inventory Planner, Supply Chain Manager, Operations Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `inventory`, `analytics`, `experimental`

**Prompt:**
```
Review inventory-related discussions over the past quarter. Identify patterns in:
- Recurring stockout causes
- Forecast accuracy concerns
- Lead time variability
- Safety stock debates
- Planning process issues

This is input for process improvement.

EXPERIMENTAL: Email analysis may not capture all inventory dynamics. Use inventory analytics for comprehensive analysis.
```

---

## Reporting

### 12. Weekly Operations Summary

**Use Case:** Create weekly logistics summary from communications.

**Target Personas:** Logistics Coordinator, Operations Manager, Shipping Supervisor

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `logistics`, `reporting`, `weekly`

**Prompt:**
```
Summarize logistics operations discussions from the past week:
- Key shipments and their status
- Issues that arose
- Resolutions achieved
- Pending items
- Escalations needed
- Wins to highlight

Format as weekly ops summary for my manager.
```

---

## Risk Management

### 13. Supply Chain Risk Assessment

**Use Case:** Gather supply chain risk discussions for formal risk assessment.

**Target Personas:** Supply Chain Manager, Risk Manager, Operations Director

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `supply-chain`, `risk`, `assessment`

**Prompt:**
```
Search for discussions about supply chain risks related to [Product/Component/Region]. Compile:
- Risks mentioned by the team
- Mitigation strategies discussed
- Alternative suppliers considered
- Lead time impacts discussed
- Cost implications mentioned
- Contingency plans proposed

This is input for risk planning. Formal assessment requires proper analysis.
```

---

## Shipment Management

### 14. Shipment Issue Summary

**Use Case:** Compile shipment issue context from communications. TMS is source of tracking data.

**Target Personas:** Logistics Coordinator, Shipping Manager, Transportation Analyst

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `logistics`, `shipment`, `tracking`

**Prompt:**
```
You are assisting a logistics coordinator. Search for all communications about shipment [Tracking Number/PO Number]. Compile:
- Current status discussions
- Issues or delays reported
- Carrier communications
- Customer notifications sent
- Resolution actions taken
- ETA updates

This is for my shipment status report. Actual tracking data from TMS.
```

---

## Supplier Management

### 15. Supplier Performance Summary

**Use Case:** Gather qualitative supplier context from communications. Use SCM system for metrics.

**Target Personas:** Supply Chain Manager, Procurement Manager, Vendor Manager

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `supply-chain`, `supplier`, `performance`

**Prompt:**
```
You are assisting a supply chain manager. Search my emails and Teams for all correspondence with [Supplier Name] over the past [timeframe]. Summarize:
- Delivery performance discussions
- Quality issues raised
- Lead time concerns
- Pricing discussions
- Capacity constraints mentioned
- Any escalations or disputes

This is for my supplier review. Actual metrics come from our SCM system.
```

---

## Governance

### 16. Supply Chain & Logistics Copilot Guardrails

**Use Case:** Essential guardrails for supply chain and logistics professionals using Copilot.

**Target Personas:** Supply Chain Manager, Logistics Coordinator, Inventory Planner

**Tags:** `copilot`, `microsoft-365`, `enterprise`, `guardrails`, `governance`, `supply-chain`, `logistics`

**Prompt:**
```
## When NOT to Use Copilot for Supply Chain & Logistics

**SUPPLY CHAIN MANAGERS - NEVER use Copilot for:**
- Purchase order creation (use ERP)
- Supplier payments or approvals
- Contract execution
- Demand forecasting (use planning tools)
- Inventory calculations (use WMS/ERP)
- Supplier qualification decisions
- Compliance certifications
- Risk scoring (use risk tools)

**LOGISTICS COORDINATORS - NEVER use Copilot for:**
- Shipment booking (use TMS)
- Carrier rate negotiations
- Customs declarations
- Dangerous goods documentation
- Delivery commitments to customers
- Tracking data (use TMS)
- Claims processing
- Route optimization (use routing tools)

**INVENTORY PLANNERS - NEVER use Copilot for:**
- Reorder point calculations (use planning tools)
- Safety stock calculations
- Demand forecasting (use forecasting tools)
- Inventory valuation (use ERP)
- Write-off approvals
- Cycle count reconciliation
- ABC classification (use analytics)
- MRP runs (use ERP)

**Data & Compliance Warnings:**
- Never include pricing details in prompts
- Be careful with supplier confidential information
- Follow trade compliance requirements
- Customs data requires proper systems
- Hazmat information requires certified systems

**Golden Rules:**
- Supply Chain: "Copilot researches - supply chain decides"
- Logistics: "Copilot tracks context - logistics executes"
- Inventory: "Copilot finds context - planners optimize"

**System Integration Note:**
Copilot does NOT integrate with:
- ERP systems (SAP, Oracle, NetSuite)
- WMS (Warehouse Management Systems)
- TMS (Transportation Management Systems)
- Demand planning tools
- Customs/trade compliance systems
```

---

---

**Made with care by [NerdyChefs.ai](https://nerdychefs.ai)**

[← Back to Main Collection](../../README.md) | [Browse All Prompts](../README.md) | [Role-Specific Prompts](./README.md)

For the complete library of 1300+ AI prompts, visit [nerdychefs.ai](https://nerdychefs.ai)
