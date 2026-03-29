# Revenue Attribution Analysis

## Purpose
Design multi-touch attribution models appropriate to the sales cycle and channel mix, evaluate model options, and communicate attribution limitations to prevent over-indexing on imperfect data.

---

## When to Use This Skill
- Evaluating which channels and campaigns are driving revenue
- Justifying or reallocating marketing budget
- Setting up or auditing attribution infrastructure
- Responding to leadership questions about marketing's revenue contribution

---

## Briefing Checklist
Before starting, confirm:
1. **Business objective** — Budget decisions, channel evaluation, or reporting improvement?
2. **Sales cycle length** — Short (days) or long (months)? Determines model suitability.
3. **Channel mix** — Which channels are in scope for attribution?
4. **Data infrastructure** — What CRM, MAP, and analytics systems are available?
5. **Output audience** — CFO, CMO, or marketing team? Determines precision required.

---

## Process

### Step 1 — Understand the Attribution Landscape
Attribution models distribute credit for a conversion across touchpoints:

| Model | How It Works | Best For |
|---|---|---|
| First-touch | 100% credit to the first interaction | Awareness and acquisition analysis |
| Last-touch | 100% credit to the final interaction before conversion | Short sales cycles, direct response |
| Linear | Equal credit to all touchpoints | Multi-channel awareness campaigns |
| Time-decay | More credit to touchpoints closer to conversion | Mid-length sales cycles |
| U-shaped (Position-based) | 40% first, 40% last, 20% middle | Balanced multi-touch analysis |
| Data-driven | Algorithmic credit based on actual conversion contribution | High-volume, data-rich environments |

### Step 2 — Select the Right Model(s)
Matching model to context:

| Sales Cycle | Recommended Models |
|---|---|
| < 2 weeks | Last-touch or first-touch |
| 2 weeks – 3 months | U-shaped or time-decay |
| 3+ months | Multi-touch (linear or data-driven) |
| Enterprise/complex | Marketing Mix Modelling + qualitative overlay |

Use multiple models in parallel and compare results — divergence reveals where debate should be focused.

### Step 3 — Map the Touchpoint Data
Document all trackable touchpoints in the customer journey:
- Paid channels: search, social, display, sponsorships
- Owned channels: email, organic search, website, events
- Offline: trade shows, outbound calls, direct mail
- Partner: referrals, resellers, integrations

Identify tracking gaps (offline touchpoints, dark social, long-tail channels) and note them explicitly in the output.

### Step 4 — Run the Attribution Analysis
For each model and channel, calculate:
- Revenue attributed
- Pipeline attributed
- Number of touchpoints in winning journeys
- Average number of touches before conversion

Then compare:
- Which channels look most valuable under which model?
- Where does model selection change the budget case significantly?
- What does the data say vs what intuition says?

### Step 5 — Layer in Incrementality
Attribution tells you what touched a buyer. Incrementality tells you what caused the conversion:
- Would this customer have converted without this touchpoint?
- Use holdout tests, geo-tests, or media mix modelling to estimate true incremental impact
- Flag where attribution overstates or understates channel impact

### Step 6 — Communicate Limitations Clearly
Every attribution report must include a caveats section:
- Model chosen and why
- Touchpoints not tracked and their estimated scale
- Why the model may over- or undervalue specific channels
- What decisions this data should and should not drive

---

## Output Formats

### Attribution Model Document
- Model selection rationale
- Touchpoint map
- Data sources and limitations
- Model comparison (first, last, multi-touch side by side)
- Recommended model for budget decisions

### Channel Contribution Report
- Revenue and pipeline attributed by channel and model
- Share of contribution vs share of spend
- ROI by channel under chosen model
- Recommended investment shifts

### Media Mix Analysis
- Cross-channel performance summary
- Diminishing returns analysis by channel
- Optimal budget allocation recommendation
- Scenario modelling (what happens if we shift 10% of budget from X to Y)

---

## Common Mistakes to Avoid
- **Treating attribution as truth.** All models are approximations. Communicate this clearly.
- **Defaulting to last-touch.** Last-touch systematically undervalues awareness and mid-funnel activity.
- **Ignoring offline touchpoints.** In B2B especially, sales conversations drive decisions that analytics can't see.
- **Over-engineering for low data volumes.** Data-driven attribution requires volume; use simpler models for small datasets.
- **Using attribution to justify existing budget.** Attribution should challenge allocations, not validate them.

---

## Quality Check
Before submitting, ask:
- [ ] Is the model selection justified for this sales cycle and channel mix?
- [ ] Are tracking gaps documented and sized?
- [ ] Have multiple models been compared, not just one?
- [ ] Are incrementality caveats included?
- [ ] Does the output clearly state what decisions this analysis should and should not drive?
