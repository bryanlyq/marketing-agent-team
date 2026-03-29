# Marketing Automation Architecture

## Purpose
Design automation workflows for lead nurturing, lifecycle marketing, and operational efficiency — so marketing scales without proportional headcount growth, and every contact receives relevant, timely communication based on their behaviour and stage.

---

## When to Use This Skill
- Marketing is manually managing communications that could be automated
- Lead nurture is inconsistent — some contacts get follow-up; others don't
- Email sends are batch-and-blast rather than trigger-based
- Building or restructuring a MAP (Marketing Automation Platform) instance
- Scaling the marketing function without scaling the team proportionally

---

## Briefing Checklist
Before starting, confirm:
1. **Platform** — Which MAP is in use or being evaluated? (HubSpot, Marketo, Pardot, ActiveCampaign, Klaviyo?)
2. **Use case scope** — What workflows are in scope? (Lead nurture, lifecycle, ops, all?)
3. **Data model** — What properties and behaviours are tracked in the CRM/MAP?
4. **Current state** — What automation already exists? What's working and what's failing?
5. **Integration requirements** — What other systems must the MAP connect to? (CRM, product, support, billing?)

---

## Automation Programme Types

| Programme Type | Purpose | Trigger |
|---|---|---|
| **Lead nurture** | Educate and qualify prospects; move MQLs toward SQLs | Content download, webinar registration, ad click |
| **Welcome** | Set expectations; deliver first value; begin relationship | List subscribe, lead form submission |
| **Trial onboarding** | Drive activation; reduce time to first value | Trial sign-up |
| **Customer lifecycle** | Sustain engagement; prompt adoption; drive expansion | Lifecycle milestones, usage triggers |
| **Re-engagement** | Reactivate cold or disengaged contacts | 60–90 days of inactivity |
| **Lead routing** | Assign leads to the right sales owner immediately | Lead score threshold, form submission |
| **Internal notifications** | Alert sales or CS to high-intent behaviour | Pricing page visit, demo request, score spike |
| **Data hygiene** | Keep database clean and actionable | Contact inactivity, data gap detection |

---

## Automation Design Principles

### 1. Trigger-Based, Not Time-Based
Time-based sequences (send email on Day 3, Day 7, Day 14) are inferior to behaviour-triggered workflows. A contact who visits the pricing page on Day 2 should receive conversion-focused content immediately — not on Day 14 because that's when the nurture sequence gets to it.

Design for behaviour first; use time as a fallback when no behavioural signal is present.

### 2. One Workflow, One Job
Each workflow should have a single purpose. A workflow that nurtures, onboards, and re-engages simultaneously becomes unmanageable and produces irrelevant communications.

### 3. Suppression Logic is Mandatory
Every workflow must have suppression conditions — criteria that exclude a contact from entering:
- Already a customer (don't send trial nurture to paying customers)
- Already in another active workflow (prevent double-messaging)
- Opted out or unsubscribed
- Flagged as "do not contact" by sales

### 4. Exit Logic Defines the Journey
Every workflow must have defined exit conditions:
- Desired exit: contact converts (demo booked, trial started, purchase made)
- Undesired exit: contact opts out, disengages, or is disqualified
- Time-based exit: maximum duration regardless of behaviour

Contacts who exit one workflow should be enrolled in the appropriate next workflow automatically.

### 5. Human Escalation Points
Automation handles volume; humans handle complexity. Define where in each workflow a human should take over:
- When a contact's lead score crosses the SQL threshold → route to SDR
- When a customer health score drops below a threshold → CS notification
- When a high-value prospect requests contact → immediate AE alert

---

## Process

### Step 1 — Map the Automation Universe
List all automation needed across the full marketing and CS function:
- What manual communications currently exist that should be automated?
- What behaviours or events should trigger a communication but currently don't?
- What internal notifications does the sales or CS team need?
- What data hygiene tasks are currently done manually?

Group into workflow types. Prioritise by business impact.

### Step 2 — Design Each Workflow

For every workflow, document before building:

**Workflow brief:**
- **Name:** Clear, descriptive name
- **Purpose:** One sentence on what this workflow achieves
- **Trigger:** The exact event or condition that enrols a contact
- **Audience:** Who qualifies for this workflow (and who is suppressed)
- **Content summary:** What communications will be sent
- **Branches:** What conditions cause the workflow to split?
- **Exit conditions:** What removes a contact from the workflow?
- **Human escalation:** When does the workflow trigger a human action?
- **Connected workflows:** What workflow does a contact move to on exit?
- **Success metric:** How will the workflow's performance be measured?

### Step 3 — Map the Workflow Logic

Build a logic map before configuration:

```
[TRIGGER: Contact downloads guide]
    ↓
[FILTER: Is this contact already a customer?]
    → YES: Exit; enrol in Customer Programme
    → NO: Continue
        ↓
    [FILTER: Is contact already in another nurture workflow?]
        → YES: Exit; no action
        → NO: Continue
            ↓
        [WAIT: 1 hour]
            ↓
        [SEND: Email 1 — deliver guide + welcome]
            ↓
        [WAIT: 3 days]
            ↓
        [BRANCH: Did contact open Email 1?]
            → YES: Send Email 2 (engaged path)
            → NO: Send Re-engagement prompt
```

Every branch must have a defined path. Dead ends in workflows produce stuck contacts and data quality issues.

### Step 4 — Define Lead Scoring Logic
Lead scoring is the automation that determines when a contact is ready for sales. Define:

**Fit score (demographic/firmographic):**
Set during data capture or enrichment:
- Correct ICP industry: +15
- Correct company size: +15
- Correct geography: +10
- Correct job title/function: +20

**Engagement score (behavioural):**
Incremented automatically based on behaviour:
- Email open: +2
- Email click: +5
- Blog post view: +3
- Key page view (pricing, demo, case study): +15–25
- Form submission: +10–20
- Webinar attendance: +20
- Score decay: −5 per week of inactivity after 30 days

**SQL threshold:** Define the score at which a contact is automatically routed to sales (e.g., ≥75 combined score).

### Step 5 — Configure and QA
Before going live:
- Test every trigger condition with test contacts
- Test all branches (including unhappy paths)
- Test suppression logic (verify excluded contacts don't enter)
- Test exit conditions
- Send test emails to real inboxes — check rendering on desktop and mobile
- Verify all tracking links fire correctly
- Confirm CRM sync is working (leads are being created/updated correctly)

### Step 6 — Monitor and Optimise
Post-launch monitoring:
- Workflow completion rate (are contacts completing or getting stuck?)
- Email performance per step (where does engagement drop off?)
- SQL conversion rate (is the lead scoring threshold right?)
- Suppression errors (are wrong contacts entering?)

Review all workflows quarterly. A workflow built 18 months ago may no longer reflect the current product, ICP, or message.

---

## Output Formats

### Automation Architecture Diagram
Visual map of all workflows showing:
- Workflow names and types
- Trigger conditions
- Connections between workflows
- Human escalation points

### Workflow Design Document (per workflow)
Complete brief including trigger, audience, logic map, email content summaries, and exit conditions.

### Lead Scoring Model
- Fit criteria and point values
- Engagement criteria and point values
- Score decay logic
- SQL threshold
- Routing rules at threshold

### MAP Configuration Checklist
Per workflow, pre-launch QA checklist:
- [ ] Trigger tested
- [ ] Suppression logic verified
- [ ] All branches mapped and tested
- [ ] Emails render correctly on mobile and desktop
- [ ] All links tracked and firing
- [ ] CRM sync confirmed
- [ ] Exit conditions tested
- [ ] Internal notifications confirmed

---

## Common Mistakes to Avoid
- **Workflows without suppression logic.** Customers enrolled in prospect nurture, or contacts receiving two simultaneous workflows, undermine trust and deliverability.
- **No exit conditions.** Contacts stuck in workflows indefinitely inflate active contact counts and produce irrelevant ongoing messaging.
- **Building before designing.** Configuring in the MAP without a documented logic map creates workflows that are impossible to audit or debug.
- **Lead scoring never calibrated.** If the SQL threshold was set at launch and never adjusted, it's almost certainly miscalibrated. Review quarterly against MQL → SQL conversion data.
- **No QA before go-live.** Automation errors reach hundreds or thousands of contacts before anyone notices.

---

## Quality Check
Before submitting, ask:
- [ ] Is every workflow documented with trigger, suppression, logic, exit, and success metric?
- [ ] Does the lead scoring model have both fit and engagement dimensions?
- [ ] Are all workflows connected — does every exit route to an appropriate next programme?
- [ ] Is there a QA checklist and review process before any workflow goes live?
- [ ] Is there a quarterly review cadence to audit and update workflows?
