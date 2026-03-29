# Lifetime Value Modeling

## Purpose
Build LTV models segmented by cohort, channel, product, and geography to inform CAC targets, channel investment decisions, and retention priorities.

---

## When to Use This Skill
- Setting CAC targets and marketing budget allocations
- Evaluating which customer segments are most valuable
- Justifying retention investment to leadership
- Pricing and offer strategy decisions

---

## Briefing Checklist
Before starting, confirm:
1. **Business objective** — CAC benchmarking, segment prioritisation, retention ROI, or pricing?
2. **Business model** — SaaS/subscription, e-commerce, marketplace, or transactional?
3. **Data access** — Revenue, churn, margin, and cohort data available?
4. **Segmentation** — Which dimensions matter: cohort, channel, product, segment, geography?
5. **Time horizon** — 12-month, 24-month, or full lifetime LTV?

---

## Process

### Step 1 — Choose the Right LTV Formula
**Simple LTV (transactional):**
LTV = Average Order Value × Purchase Frequency × Customer Lifespan

**Subscription LTV:**
LTV = (ARPU × Gross Margin %) ÷ Monthly Churn Rate

**Discounted LTV (investor-grade):**
LTV = Σ (Revenue_t × Margin_t) ÷ (1 + Discount Rate)^t

Choose based on business model. Document the formula and its assumptions clearly.

### Step 2 — Build the Core LTV Model
Define inputs:

| Input | Definition | Source |
|---|---|---|
| ARPU / AOV | Average revenue per user or order | Finance / CRM |
| Gross margin % | Revenue minus COGS | Finance |
| Churn rate | % of customers lost per period | CRM / Product |
| Purchase frequency | Orders per customer per year | CRM |
| Retention rate | 1 − churn rate | Calculated |

Build the model in a spreadsheet with clearly labelled inputs so assumptions can be tested.

### Step 3 — Segment the LTV Analysis
Calculate LTV separately for:
- **Acquisition cohort** (when did they sign up?)
- **Acquisition channel** (where did they come from?)
- **Product or plan tier** (what do they pay for?)
- **Customer segment or ICP fit** (which type of customer?)
- **Geography or region** (where are they?)

Segment-level LTV often varies 3–10× across groups — averages hide the strategic picture.

### Step 4 — Sensitivity Analysis
LTV is driven by a small number of key levers. Model the impact of each:

| Driver | 10% Improvement → LTV Impact |
|---|---|
| Gross margin | Proportional to margin — high leverage |
| Churn rate | Disproportionate — biggest LTV lever in subscription |
| ARPU / expansion revenue | Direct multiplier on LTV |
| Initial purchase / activation | Affects cohort LTV, not unit LTV |

Present a sensitivity table showing LTV range under optimistic, base, and conservative assumptions.

### Step 5 — Benchmark LTV:CAC
For each segment and channel, calculate the LTV:CAC ratio:
- ≥ 3:1 — Healthy; consider increasing investment
- 2–3:1 — Manageable; improve CAC or LTV before scaling
- < 2:1 — Unsustainable at scale; prioritise efficiency before growth

Flag which segments have the most favourable economics and which are subsidised.

### Step 6 — Derive Strategic Implications
Connect LTV findings to specific decisions:

| LTV Finding | Strategic Implication |
|---|---|
| LTV varies 5× by channel source | Shift acquisition budget toward highest-LTV channels |
| LTV for enterprise 4× SMB | Increase ICP weighting toward enterprise in campaigns |
| LTV declines in month 3 cohort | Investigate onboarding or product experience at 60–90 days |
| Expansion revenue adds 40% to LTV | Build upsell programme into customer success motion |

---

## Output Formats

### LTV Model (spreadsheet)
- Input assumptions (clearly labelled)
- Core LTV calculation with formula
- Segmentation table (LTV by cohort, channel, product)
- Sensitivity table (optimistic/base/conservative)
- LTV:CAC ratio matrix

### Cohort Analysis
- Revenue retention curves by acquisition cohort
- LTV at 6, 12, 24 months post-acquisition
- Cohort comparison: which vintages perform best?

### LTV:CAC Dashboard
- Ratio by channel, segment, and period
- Trend over time
- Investment implication by segment

---

## Common Mistakes to Avoid
- **Using average LTV for all decisions.** Segment LTV varies massively — averages mislead.
- **Ignoring gross margin.** Revenue LTV is not the same as profit LTV. Always use margin-adjusted figures.
- **Underestimating churn impact.** In subscription models, reducing churn 1% can increase LTV 10–25%.
- **Treating LTV as a fixed number.** LTV is a model with assumptions — update it when the business changes.
- **Forgetting expansion revenue.** In SaaS and B2B, upsell/cross-sell can add 30–50% to LTV.

---

## Quality Check
Before submitting, ask:
- [ ] Is the LTV formula appropriate for the business model?
- [ ] Are assumptions documented and sourced?
- [ ] Is LTV segmented beyond an overall average?
- [ ] Does the sensitivity analysis show the range of realistic outcomes?
- [ ] Are LTV findings connected to specific investment and strategy decisions?
