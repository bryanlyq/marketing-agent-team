# Demand Pipeline Tracking

## Purpose
Build pipeline tracking from MQL through to closed revenue, define pipeline velocity and conversion rates by stage, and identify health risks with recommended interventions.

---

## When to Use This Skill
- Setting up or auditing pipeline reporting infrastructure
- Weekly, monthly, or quarterly pipeline reviews
- When pipeline coverage or velocity is below target
- Aligning marketing and sales on shared pipeline definitions

---

## Briefing Checklist
Before starting, confirm:
1. **Business objective** — Revenue target, pipeline coverage ratio required, or audit?
2. **Current state** — What pipeline data exists and where is it held (CRM, spreadsheet)?
3. **Shared definitions** — Are MQL, SQL, opportunity, and stage definitions agreed with sales?
4. **Time horizon** — Current quarter, trailing 12 months, or forward-looking?
5. **Output format** — Live dashboard, snapshot report, or planning document?

---

## Process

### Step 1 — Define the Pipeline Waterfall
Establish agreed definitions for each stage before measuring:

| Stage | Definition | Owner |
|---|---|---|
| MQL | Marketing Qualified Lead — meets scoring threshold | Marketing |
| SAL | Sales Accepted Lead — sales reviewed and agreed to pursue | Sales |
| SQL | Sales Qualified Lead — confirmed need, budget, and timeline | Sales |
| Opportunity | Active deal with defined close date and value | Sales |
| Closed Won | Contract signed, revenue recognised | Sales/Finance |
| Closed Lost | Deal ended without conversion | Sales |

### Step 2 — Build the Pipeline Waterfall Report
Track volume and conversion at each stage:

| Stage | Volume (Period) | Conversion to Next Stage | Avg. Days in Stage |
|---|---|---|---|
| MQL | — | —% to SAL | — days |
| SAL | — | —% to SQL | — days |
| SQL | — | —% to Opportunity | — days |
| Opportunity | — | —% to Closed Won | — days |

### Step 3 — Calculate Pipeline Velocity
Pipeline velocity = (Number of Opportunities × Win Rate × Avg. Deal Value) ÷ Sales Cycle Length

Track velocity changes over time — a slowing velocity is an early warning signal.

### Step 4 — Assess Pipeline Coverage
Coverage ratio = Total Pipeline Value ÷ Revenue Target

| Coverage Level | Status |
|---|---|
| 3× or above | Healthy — sufficient buffer for conversion losses |
| 2–3× | Manageable — monitor closely |
| Below 2× | At risk — demand generation intervention needed |

Segment coverage by:
- Segment or product line
- Sales rep or region
- Channel source (to identify which demand sources are most productive)

### Step 5 — Identify Pipeline Health Risks
Review for:
- **Stale opportunities** — Deals that haven't progressed in 30+ days
- **Stage concentration** — Too many deals stuck at one stage
- **Source imbalance** — Over-reliance on a single demand source
- **Coverage gaps** — Quarters with insufficient pipeline already in the system

### Step 6 — Recommend Interventions
For each health risk, define a specific action:

| Risk | Recommended Intervention |
|---|---|
| Low MQL volume | Increase demand gen activity or expand ICP definition |
| Poor MQL → SAL conversion | Review lead quality or scoring model |
| Low win rate | Investigate competitive loss reasons or pricing |
| Long sales cycle | Add mid-funnel nurture or executive engagement |

---

## Output Formats

### Pipeline Dashboard (live)
- Current period MQL, SQL, opportunity volume
- Pipeline coverage ratio vs target
- Stage-by-stage conversion rates
- Pipeline by source, segment, and rep
- Stale deal alerts

### Pipeline Velocity Report
- Velocity calculation and trend
- Conversion rate trends by stage
- Average deal cycle length
- Revenue forecast based on current pipeline

### Pipeline Health Review (quarterly)
- Coverage assessment vs next 2 quarters
- Risk identification and severity scoring
- Marketing contribution to pipeline (sourced and influenced)
- Recommended demand generation adjustments

---

## Common Mistakes to Avoid
- **Inconsistent stage definitions.** If marketing and sales define SQL differently, all reporting breaks.
- **Tracking volume without velocity.** A large pipeline that doesn't move is not healthy.
- **Ignoring source attribution.** Knowing which channels build the best pipeline is as important as knowing total volume.
- **Reporting pipeline without coverage context.** 50 opportunities means nothing without knowing if that's enough.
- **Conflating marketing-sourced with marketing-influenced.** Both matter, but they're different metrics.

---

## Quality Check
Before submitting, ask:
- [ ] Are stage definitions agreed with sales before measuring?
- [ ] Is pipeline coverage calculated and benchmarked against target?
- [ ] Are conversion rates tracked at every stage, not just top and bottom?
- [ ] Are stale deals and concentration risks identified?
- [ ] Does the output end with specific interventions, not just observations?
