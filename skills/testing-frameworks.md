# Testing Frameworks

## Purpose
Build a structured test-and-learn culture with rigorous hypotheses, controlled experiments, and systematised learnings — so that marketing decisions compound in quality over time rather than repeating the same mistakes with more confidence.

---

## When to Use This Skill
- Marketing decisions are based on intuition or HiPPO (Highest Paid Person's Opinion)
- A/B test results are inconsistent, inconclusive, or poorly interpreted
- Learnings from tests are not captured or applied
- Building a marketing function that scales on data, not assumptions
- Entering a new channel, audience, or market that requires fast learning

---

## Briefing Checklist
Before starting, confirm:
1. **Testing maturity** — Is the team running ad-hoc tests or is there an existing programme?
2. **Traffic / sample volumes** — Are there sufficient volumes for statistically valid tests?
3. **Testing infrastructure** — Is there a testing platform and analytics setup in place?
4. **Culture** — Is leadership comfortable with tests producing null or negative results?
5. **Scope** — What will the testing programme cover? (Messaging, channels, creative, UX?)

---

## Types of Marketing Tests

| Test Type | What It Optimises | Examples |
|---|---|---|
| **A/B test (split test)** | One variable at a time | Headline copy, CTA, hero image, email subject line |
| **Multivariate test** | Multiple variables simultaneously | Multiple page elements tested in combination |
| **Split URL test** | Two entirely different page designs | Radical page redesign vs control |
| **Message test** | Value proposition or messaging variants | Two different landing page value prop framings |
| **Channel test** | Performance of a new or untested channel | LinkedIn Ads vs programmatic display |
| **Audience test** | Different segments or targeting approaches | Segment A vs Segment B response to same campaign |
| **Offer test** | Different commercial offers | 14-day trial vs 30-day trial vs free tier |
| **Creative test** | Ad or content creative variants | Video vs static, testimonial vs data, lifestyle vs product |

---

## The Testing Framework

### Phase 1 — Observe
Before hypothesising, gather evidence:
- Analytics data (where are the biggest drop-offs or performance gaps?)
- Qualitative data (session recordings, user interviews, support tickets)
- Competitive benchmarks (what are industry norms for this metric?)
- Prior test results (what has already been tested and what were the findings?)

### Phase 2 — Hypothesise
A well-formed hypothesis has three components:
> "We believe that **[specific change]** will **[improve specific metric]** because **[evidence-backed reason]**."

Examples:
- "We believe that changing the CTA from 'Start free trial' to 'Get instant access' will increase click-through rate because exit surveys indicate visitors don't understand what 'trial' means in context"
- "We believe that adding a customer logo bar above the fold will increase demo request conversion rate because heatmap data shows visitors who scroll to the social proof section convert at 3x the rate of those who don't"

Reject vague hypotheses. "Let's test a shorter form to see if conversions go up" is an observation, not a hypothesis.

### Phase 3 — Design
Before running any test, define the complete test specification:

**Test specification:**
- **Hypothesis:** (full statement)
- **Control:** Description of the current version
- **Variant(s):** Description of each change being tested
- **Primary metric:** The single conversion event that defines success
- **Secondary metrics:** Guardrail metrics that must not significantly degrade
- **Minimum detectable effect (MDE):** The smallest change worth detecting (e.g., a 10% lift in CVR)
- **Required sample size:** Calculated from MDE, baseline conversion rate, and significance threshold
- **Test duration:** At least 2 weeks; stop only when sample size is reached (not before)
- **Statistical significance threshold:** 95% (0.05 p-value) as standard
- **Owner and launch date**

### Phase 4 — Run
Test hygiene:
- Only test one primary variable at a time in an A/B test
- Ensure both versions receive traffic simultaneously (not sequentially)
- Do not make other changes to the page or campaign during the test
- Monitor for data quality issues: bot traffic, tracking errors, sample ratio mismatch (SRM)
- Do not peek at results and stop early if one variant appears to be winning

### Phase 5 — Read
How to interpret test results:

**Statistical significance:** Has the observed result met the confidence threshold? (Use a significance calculator — don't eyeball it)
**Practical significance:** Even if statistically significant, is the effect large enough to matter?
**Secondary metrics check:** Did the variant improve the primary metric while degrading an important secondary metric?
**Segment analysis:** Did the result hold across all traffic segments, or did it win for one segment and lose for another?

**Possible outcomes:**
| Outcome | Meaning | Action |
|---|---|---|
| Significant winner | Variant beats control with confidence | Implement variant; update the learning log |
| Significant loser | Control beats variant with confidence | Keep control; document the hypothesis failure |
| Inconclusive | No significant difference | Extend the test (if feasible) or close; note the null result |
| Segment win | Variant wins for specific segment only | Consider personalisation; document the segment insight |

Do not celebrate a null result as failure. A null result is a valuable data point: it tells you the variable you tested isn't the constraint.

### Phase 6 — Systematise
Testing generates compound value only if learnings are captured and shared:

**Learning repository entry:**
| Field | Content |
|---|---|
| Test ID | Unique reference |
| Date run | Period of the test |
| Area | Page / channel / asset |
| Hypothesis | Full hypothesis statement |
| What was changed | Control vs variant description |
| Primary metric result | Effect size and significance |
| Confidence level | Statistical confidence % |
| Key insight | What did we learn about our audience / message / behaviour? |
| Where else applies | Other contexts where this insight is relevant |
| Recommended next test | What does this result suggest testing next? |

---

## Sample Size and Duration Guidelines

**Sample size calculation inputs:**
- Baseline conversion rate (e.g., 3%)
- Minimum detectable effect (e.g., 10% relative improvement = 3.3% target)
- Statistical significance level (95%)
- Statistical power (80%)

Use a sample size calculator (AB Testguide, Optimizely, or Evan Miller's calculator) to generate required sample per variant.

**Duration guidance:**
- Never run for less than 7 days (day-of-week effects)
- Aim for 14–21 days for most tests
- If sample size isn't reached after 4 weeks, the test is likely underpowered — redesign with a larger MDE or acquire more traffic

---

## Common Testing Mistakes

| Mistake | Why It's Dangerous | Fix |
|---|---|---|
| Stopping early on a "winner" | Inflates false positive rate dramatically | Stop only when sample size is reached |
| Testing multiple variables in A/B | Makes it impossible to know which variable drove the effect | One variable per A/B test |
| No hypothesis | Produces results with no interpretable meaning | Always write a hypothesis before designing the test |
| Ignoring secondary metrics | A variant can win on primary metric while damaging downstream quality | Define guardrail metrics before running |
| Calling inconclusive tests "failures" | Discourages experimentation | Null results are valid; document them |
| Not sharing learnings | CRO knowledge siloed; same mistakes recur | Maintain a shared learning repository |

---

## Output Formats

### Testing Framework Document
- Programme scope and objectives
- Prioritisation methodology (ICE or equivalent)
- Test design requirements (specification template)
- Statistical standards (significance threshold, power, duration rules)
- Learning repository structure
- Review cadence and governance

### Test Design Template
Standardised test specification (see Phase 3 above)

### Learning Repository
Running log with all past tests, outcomes, and insights. Searchable by area (page, channel, audience), outcome, and date.

### Testing Roadmap
Priority-ordered backlog of planned tests with:
- ICE score
- Test description
- Status (planned, running, complete)
- Expected launch date

---

## Quality Check
Before submitting, ask:
- [ ] Does every test have a full hypothesis including the "because" rationale?
- [ ] Is sample size calculated before the test launches — not estimated post-hoc?
- [ ] Are secondary metrics and guardrails defined for every test?
- [ ] Is there a process to stop the test only when sample size is reached?
- [ ] Is there a learning repository that captures null results as well as wins?
