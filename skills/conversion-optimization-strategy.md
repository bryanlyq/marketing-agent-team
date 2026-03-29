# Conversion Optimisation Strategy

## Purpose
Build a structured, evidence-based programme for improving conversion rates across the funnel — using heuristic evaluation, data analysis, and disciplined testing — so that more of the existing traffic and lead volume converts to revenue.

---

## When to Use This Skill
- Conversion rates are below benchmarks or declining
- Paid media spend is high but post-click performance is poor
- Landing pages, forms, or checkout flows have high abandonment
- High traffic volumes not converting to leads or customers
- Building a test-and-learn culture within the marketing team

---

## Briefing Checklist
Before starting, confirm:
1. **Focus area** — Which part of the funnel? (Landing page, sign-up flow, onboarding, checkout?)
2. **Current conversion rate** — What is the baseline? What is the benchmark?
3. **Traffic volume** — Is there enough traffic for statistically valid A/B testing?
4. **Data access** — What analytics, session recording, and heatmap data is available?
5. **Technical capability** — Can changes be implemented quickly? Is a CMS or A/B testing platform in place?

---

## CRO vs Funnel Design

| CRO (Conversion Rate Optimisation) | Funnel Design |
|---|---|
| Improving an existing conversion flow | Building a new conversion flow |
| Incremental optimisation | Structural redesign |
| Data-led testing | Strategy-led architecture |
| Works when the right audience is already arriving | Works when the wrong audience or wrong message is the root cause |

CRO assumes the audience and offer are broadly right. If conversion is low because the wrong traffic is arriving or the product isn't the right fit, CRO won't fix it.

---

## CRO Diagnostic Framework

Before testing, diagnose. Low conversion has several distinct root causes requiring different fixes:

| Root Cause | Symptom | Fix |
|---|---|---|
| **Wrong audience** | High bounce rate; very low time on page | Fix targeting and traffic quality upstream |
| **Message mismatch** | High traffic; low scroll depth; high exit rate on hero section | Align headline to traffic source intent |
| **Credibility gap** | Long time on page; no conversion | Add social proof, case studies, security signals |
| **Unclear offer** | High pricing page drop-off | Simplify pricing; improve tier differentiation |
| **Form friction** | High form abandonment rate | Reduce fields; progressive disclosure; clearer labels |
| **CTA weakness** | Low click rate on primary CTA | Rewrite CTA copy; improve placement; increase visibility |
| **Mobile UX failure** | Mobile conversion rate significantly lower than desktop | Mobile-first redesign of key pages |
| **Page speed** | High exit rate; low engagement on first load | Improve Core Web Vitals; reduce page weight |

Diagnose before testing. Testing the wrong variable produces false positives and wastes time.

---

## Process

### Step 1 — Audit the Conversion Funnel
Map every step from traffic entry to conversion:
- What are the conversion rates at each step?
- Where is the biggest drop-off?
- Is drop-off consistent across segments, sources, and devices?

Tools: GA4 funnel exploration, Hotjar session recordings, heatmaps, scroll maps, form analytics.

### Step 2 — Run a Heuristic Evaluation
Before using data, conduct an expert review of the conversion experience using established heuristics:

**Clarity:** Is the value proposition immediately clear within 5 seconds?
**Relevance:** Does the page match the intent of the traffic arriving at it?
**Trust:** Are there sufficient credibility signals for a first-time visitor?
**Friction:** How many steps, clicks, or fields stand between the visitor and conversion?
**Urgency:** Is there a reason to act now rather than later?
**Distraction:** Are there competing elements that pull attention from the primary CTA?

Rate each dimension 1–5. Focus testing efforts on the lowest-scored dimensions.

### Step 3 — Gather Qualitative Data
Numbers show what is happening; qualitative data shows why:
- **Session recordings** (Hotjar, FullStory): Watch how real visitors navigate the page
- **Heatmaps**: Where are visitors clicking, hovering, and ignoring?
- **User testing**: Have 5 people in the ICP attempt to complete the conversion task; observe without helping
- **Exit surveys**: Ask one question to visitors about to leave: "What stopped you from completing your action today?"
- **Support tickets**: What questions do people ask before converting? These signal information gaps on the page.

### Step 4 — Build the Test Backlog
Generate hypotheses and score with ICE:

**Hypothesis format:**
> "We believe that [changing X] will [increase Y] because [reason based on evidence Z]"

**ICE Score:**
- **Impact (1–10):** How much will this move the conversion rate if it works?
- **Confidence (1–10):** How strong is the evidence that this will work?
- **Ease (1–10):** How quickly and easily can this be implemented and measured?
- **ICE Score = Impact × Confidence × Ease**

Rank the backlog by ICE score. Run highest-scoring tests first.

### Step 5 — Design the Test
For each test, define before running:
- **Control:** Current version
- **Variant(s):** The change being tested
- **Primary metric:** The conversion event being optimised
- **Secondary metrics:** Guardrail metrics that should not degrade
- **Sample size:** Minimum visitors needed per variant (use a significance calculator)
- **Duration:** Run for at least 2 weeks to account for day-of-week effects; don't stop early
- **Statistical threshold:** Minimum 95% confidence before declaring a winner

### Step 6 — Run, Read, and Systematise

**Running:**
- Use a proper A/B testing tool (Optimizely, VWO, Google Optimize, or built-in MAPs)
- Ensure no other changes are made to the page during the test
- Monitor for data quality issues (tracking errors, bot traffic)

**Reading results:**
- Only declare a winner when statistical significance is reached
- Check secondary metrics — did the test improve conversion but damage AOV or downstream quality?
- Analyse results by segment: a test that fails overall may win for a specific audience

**Systematising learnings:**
- Document every test in a learning repository: hypothesis, result, confidence level, applicable insights
- Share learnings across the team — CRO insights inform copywriting, design, and product decisions
- Build an insights library: what do we know about what works for our audience?

---

## Output Formats

### CRO Audit Report
- Funnel map with conversion rates at each step
- Heuristic evaluation scores and observations
- Qualitative data summary (session recording themes, user test observations)
- Root cause diagnosis
- Prioritised test backlog (ICE scored)

### Test Prioritisation Matrix
| Hypothesis | Impact | Confidence | Ease | ICE Score | Priority | Status |
|---|---|---|---|---|---|---|

### Test Design Brief
- Test ID and name
- Hypothesis
- Control description
- Variant description(s)
- Primary metric and target
- Secondary / guardrail metrics
- Sample size requirement
- Duration
- Owner and launch date

### Learning Repository
Running log of all tests with:
- Date run
- Page / flow
- Hypothesis
- Result (winner / loser / inconclusive)
- Confidence level
- Key insight
- Applicability (where else does this insight apply?)

---

## Common Mistakes to Avoid
- **Testing without a hypothesis.** "Let's change the button colour and see what happens" is not a test.
- **Stopping tests early.** Stopping at the first sign of positive results inflates false positive rates dramatically.
- **Underpowered tests.** Small sample sizes produce unreliable results. Calculate required sample size before starting.
- **Testing the wrong variable.** If headline clarity is the root cause of low conversion, testing button colour is wasted effort.
- **Not systematising learnings.** CRO generates valuable knowledge about the audience. If learnings aren't captured and shared, the value of each test compounds only in the tester's head.

---

## Quality Check
Before submitting, ask:
- [ ] Has the root cause of low conversion been diagnosed before tests are designed?
- [ ] Does each hypothesis include a "because" grounded in evidence?
- [ ] Is the ICE backlog prioritised — not just a flat list of ideas?
- [ ] Are test designs specified with sample size, duration, and significance threshold?
- [ ] Is there a learning repository that will capture and compound test insights?
