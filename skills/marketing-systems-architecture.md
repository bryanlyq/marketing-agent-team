# Marketing Systems Architecture

## Purpose
Design the marketing technology stack and data infrastructure that enables the strategy to be executed, measured, and optimised — without over-engineering or under-investing in the systems that matter most.

---

## When to Use This Skill
- Building a marketing tech stack from scratch
- Auditing an existing stack for gaps, redundancies, or integration failures
- Scaling marketing operations and finding system bottlenecks
- Data flowing inconsistently between CRM, MAP, and analytics
- Evaluating new technology investments
- Integrating marketing and sales systems after a merger or replatforming

---

## Briefing Checklist
Before starting, confirm:
1. **Business stage** — Startup, scale-up, or enterprise? Systems complexity should match stage.
2. **Current stack** — What tools exist, and what problems are they solving or creating?
3. **Data requirements** — What reporting and attribution does the business need?
4. **Integration constraints** — What systems are fixed (e.g., Salesforce, HubSpot, Shopify)?
5. **Objective** — Audit and fix, or build new?

---

## Marketing Systems Framework

A complete marketing stack covers five functional layers:

```
1. DATA LAYER — Capture, store, and connect customer data
2. ENGAGEMENT LAYER — Reach and communicate with audiences
3. CONVERSION LAYER — Drive actions and manage the funnel
4. INTELLIGENCE LAYER — Measure, analyse, and optimise
5. OPERATIONS LAYER — Coordinate teams and workflows
```

Every system in the stack should belong to one of these layers. If it doesn't, it's likely redundant.

---

## Layer-by-Layer Breakdown

### Layer 1 — Data Layer
**Purpose:** Create a unified customer data foundation across all touchpoints.

| System Type | Function | Example Tools |
|---|---|---|
| CRM | Single source of truth for contacts, accounts, and pipeline | Salesforce, HubSpot, Pipedrive |
| Customer Data Platform (CDP) | Unify first-party data across sources | Segment, Rudderstack, Tealium |
| Data Warehouse | Store and query marketing and product data at scale | Snowflake, BigQuery, Redshift |
| Tag Management | Capture and deploy tracking across web and app | Google Tag Manager, Tealium |

**Key question:** Is there a single record of each customer that connects marketing activity to revenue outcomes?

### Layer 2 — Engagement Layer
**Purpose:** Reach and communicate with audiences at scale.

| System Type | Function | Example Tools |
|---|---|---|
| Marketing Automation Platform (MAP) | Email, nurture, and lifecycle programmes | HubSpot, Marketo, Pardot |
| Paid Media Platforms | Manage and optimise advertising | Google Ads, Meta Ads, LinkedIn Ads |
| SEO / Content | Optimise and publish content | WordPress, Contentful, SEMrush |
| Social Media Management | Publish, engage, and monitor social | Hootsuite, Sprout Social, Buffer |
| Conversational / Chat | Qualify and engage website visitors | Drift, Intercom, HubSpot Chat |

### Layer 3 — Conversion Layer
**Purpose:** Optimise the path from engagement to action.

| System Type | Function | Example Tools |
|---|---|---|
| Landing Page Builder | Create and test conversion pages | Unbounce, Instapage, HubSpot Pages |
| A/B Testing | Experiment on page elements and flows | Optimizely, VWO, Google Optimize |
| Form and Lead Capture | Capture and route leads | HubSpot Forms, Typeform, Gravity Forms |
| Trial / Onboarding | Activate product-led growth | Appcues, Pendo, Userflow |

### Layer 4 — Intelligence Layer
**Purpose:** Measure performance and extract strategic insight.

| System Type | Function | Example Tools |
|---|---|---|
| Web Analytics | Track traffic, behaviour, and conversions | Google Analytics 4, Mixpanel |
| Attribution | Model marketing contribution to revenue | HubSpot, Bizible/Marketo Measure, Triple Whale |
| Business Intelligence | Build dashboards and cross-system reports | Looker, Tableau, Power BI, Metabase |
| Search Intelligence | Keyword research, rank tracking, competitive | Ahrefs, SEMrush, Moz |
| Review and Social Listening | Monitor brand mentions and sentiment | Brandwatch, Mention, Sprinklr |

### Layer 5 — Operations Layer
**Purpose:** Coordinate people, projects, and workflows.

| System Type | Function | Example Tools |
|---|---|---|
| Project Management | Plan and track marketing work | Asana, Monday, Notion, ClickUp |
| Asset Management | Store and organise creative assets | Bynder, Brandfolder, Google Drive |
| Collaboration | Brief, review, and approve content | Notion, Confluence, Loom |
| AI and Automation | Accelerate content, research, and analysis | Claude, ChatGPT, Jasper, Zapier |

---

## Process

### Step 1 — Audit the Current Stack
For each existing tool:
- What layer does it serve?
- What is it actually used for (vs intended purpose)?
- Is it integrated with the CRM and analytics?
- Who owns it and is it actively managed?
- What is the licence cost?
- Is it redundant with another tool?

Build a stack map showing all current tools, their layer, integration status, and utilisation.

### Step 2 — Identify Gaps and Breakdowns
Common failure patterns:
- **Data silos:** Leads in the MAP don't sync to the CRM; product usage data doesn't connect to marketing data
- **Attribution blind spots:** No way to connect marketing touchpoints to pipeline and revenue
- **Tool redundancy:** Two tools doing the same job in different teams
- **Under-utilisation:** High-cost platforms used for only 20% of their capability
- **Manual workarounds:** Teams exporting and re-importing data because integrations don't work

### Step 3 — Define the Ideal Architecture
Map the desired data flows:
- Visitor → lead → contact → opportunity → customer: where does the data live and move?
- How does marketing activity connect to CRM pipeline?
- How does revenue data flow back into marketing analytics?
- Where are the integration points that must not break?

Draw the architecture as a data flow diagram: systems as nodes, data flows as arrows.

### Step 4 — Prioritise Investments
Rank system improvements by:
- Revenue impact (does this fix a measurement blind spot or enable a new programme?)
- Integration dependency (does this unblock other systems?)
- Cost vs capability (is there a cheaper tool that does 80% of the job?)

### Step 5 — Build the Implementation Roadmap
Sequence investments:
- **Foundation first:** CRM + MAP integration and basic attribution before anything else
- **Analytics second:** Ensure measurement is in place before scaling spend
- **Optimisation third:** Testing, personalisation, and intelligence layers once foundation is stable

---

## Output Formats

### Tech Stack Audit
Table showing:
- Tool name
- Layer
- Primary function
- Integration status
- Utilisation level (High/Medium/Low)
- Annual cost
- Assessment: Keep / Upgrade / Replace / Retire

### Systems Architecture Diagram
Visual data flow showing:
- All active systems
- Integration connections
- Data flow directions
- Key handoff points

### Vendor Selection Criteria Framework
For new tool evaluations:
- Must-have requirements
- Nice-to-have features
- Integration requirements
- Data sovereignty and security requirements
- Pricing model
- Support and implementation quality
- Vendor roadmap and stability

### Implementation Roadmap
- Phase 1: Foundation (CRM, MAP, basic tracking)
- Phase 2: Attribution and analytics
- Phase 3: Conversion optimisation
- Phase 4: Intelligence and scale

---

## Common Mistakes to Avoid
- **Buying tools before defining the strategy.** The strategy defines the required data and workflows; the stack serves those requirements.
- **Point solutions without integration.** A tool that doesn't connect to the CRM creates a data silo.
- **Enterprise tools at startup scale.** Match the complexity of the stack to the maturity of the team.
- **No attribution model.** Without attribution, you can't evaluate channel ROI or justify budget.
- **Tool ownership gaps.** Every system needs a named owner. Ownerless tools become shelfware.

---

## Quality Check
Before submitting, ask:
- [ ] Is there a single customer record that connects marketing activity to revenue?
- [ ] Does the stack cover all five layers: data, engagement, conversion, intelligence, operations?
- [ ] Are integration flows mapped and tested?
- [ ] Is attribution connected from first touch to closed-won revenue?
- [ ] Does every tool have a named owner and a defined use case?
