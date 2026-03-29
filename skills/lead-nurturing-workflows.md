# Lead Nurturing Workflows

## Purpose
Build nurture sequences that move leads from initial interest to sales-ready status — by delivering relevant, progressive content at the right time — so that the marketing database works as a revenue asset rather than an idle list.

---

## When to Use This Skill
- Large volume of MQLs failing to convert to SQLs
- Leads going cold between first contact and sales follow-up
- No structured nurture programme exists; sales follows up once and drops
- Database of cold leads that haven't been re-engaged
- Building a demand generation programme that generates pipeline over time, not just leads

---

## Briefing Checklist
Before starting, confirm:
1. **Audience** — Which leads are entering nurture? (By source, segment, persona, or funnel stage?)
2. **Sales cycle length** — How long does it typically take from first contact to purchase?
3. **Existing content** — What content assets are available to build the nurture sequences?
4. **MAP capability** — What trigger and branching logic is available in the platform?
5. **Lead scoring** — Is there a lead scoring model that will trigger graduation out of nurture?

---

## Nurture vs Drip

| Nurture | Drip |
|---|---|
| Adapts based on behaviour | Fixed sequence regardless of engagement |
| Branches on opens, clicks, page views | Sends to all contacts on the same schedule |
| Progressive: each email builds on prior engagement | Repetitive: each email is independent |
| Moves faster for engaged contacts; slower for unengaged | Same pace for everyone |

Build nurture sequences with branching logic. Time-based drip sequences are better than nothing, but behaviour-triggered nurture dramatically outperforms them.

---

## Nurture Workflow Types

| Workflow | Audience | Purpose |
|---|---|---|
| **Awareness nurture** | Top-of-funnel leads; educational intent | Build problem awareness; introduce the category |
| **Consideration nurture** | Mid-funnel leads; evaluating options | Build credibility; differentiate from alternatives |
| **Re-engagement nurture** | Cold leads (60+ days inactive) | Revive interest; identify still-active prospects |
| **Trial / product nurture** | Free trial users | Drive activation; convert to paid |
| **Competitive nurture** | Leads using a competitor | Plant a seed; stay present until they're ready to switch |
| **Event nurture** | Webinar or event registrants / attendees | Convert event interest to sales conversation |

---

## Process

### Step 1 — Segment the Nurture Audience
Not all leads need the same nurture content. Segment by:
- **Funnel stage at entry:** Is this a TOFU lead (content download) or a warmer lead (demo page visit)?
- **Persona / role:** A technical buyer and a commercial buyer need different content
- **Segment / industry:** Use cases and proof points vary by vertical
- **Behaviour at entry:** What action triggered the nurture? (This is the strongest signal of intent)

A prospect who downloaded a "how-to" guide needs different nurture than one who visited the pricing page three times.

### Step 2 — Map Content to Nurture Stages
Build a content map for each nurture type:

| Stage | Content Job | Example Assets |
|---|---|---|
| **Stage 1 (Educate)** | Validate the problem; build resonance | Blog posts, research reports, thought leadership |
| **Stage 2 (Credentialize)** | Demonstrate expertise; build trust | Data, case studies, third-party proof |
| **Stage 3 (Differentiate)** | Introduce why your approach is distinctive | Comparison content, product value content |
| **Stage 4 (Convert)** | Invite a commercial action | Demo request, trial offer, consultation |

Don't lead with commercial content. Earn the right to the conversion request by delivering value first.

### Step 3 — Design the Workflow Logic

**Standard consideration nurture (6–8 emails, 4–6 weeks):**

```
[TRIGGER: Contact downloads guide]
    ↓
Email 1 (Day 0): Deliver asset + brief welcome; set expectations
    ↓
Wait 3 days
    ↓
Email 2 (Day 3): Related insight; educational content on the problem
    ↓ [BRANCH: Did they click?]
    → YES (engaged path): Move to email 3 after 2 days
    → NO (passive path): Wait 5 more days before email 3
        ↓
Email 3: Social proof — case study or customer story
    ↓ [BRANCH: Have they visited pricing page since enrolment?]
    → YES: Skip to conversion email (Email 6)
    → NO: Continue to email 4
        ↓
Email 4: Differentiation content (how your approach is different)
    ↓
Email 5: Objection handling content (address the most common hesitation)
    ↓
Email 6: Conversion CTA — demo, trial, or consultation
    ↓
[BRANCH: Did they convert?]
    → YES: Exit to sales handoff workflow
    → NO: Continue to re-engagement or long-term nurture
```

### Step 4 — Define Email Content for Each Step

For each nurture email, define:

**Subject line:**
- Test: specificity over cleverness
- Examples: "How [Company] reduced churn by 40%" vs "The approach most teams miss"

**Structure:**
1. Open with relevance (reference their context or prior action)
2. Deliver value first (content, insight, or proof)
3. One clear CTA — not multiple options

**Length:**
- Nurture emails should be shorter than expected — 150–300 words for most steps
- Long-form works for delivering substantive content (e.g., a research summary)
- Never write more than the contact will read

**CTA progression:**
- Emails 1–3: Low-commitment CTAs (read this, watch this, see the data)
- Emails 4–5: Medium-commitment (check out this case study, see how [company] did it)
- Email 6+: High-commitment (book a demo, start your trial, speak to our team)

Don't ask for the sale before you've earned trust.

### Step 5 — Define Graduation Criteria
Define precisely when a lead graduates from nurture to sales:
- Lead score reaches SQL threshold (fit + engagement combined)
- Specific high-intent behaviour (demo request, pricing page visit 3x, trial sign-up)
- Explicit request for sales contact

When graduation conditions are met:
- Remove contact from active nurture workflow
- Notify the assigned SDR or AE immediately (internal notification email or CRM task)
- SLA: SDR follows up within [X hours]

### Step 6 — Define Long-Term Nurture (for leads not ready)
Not every lead will graduate on the first pass. Define the programme for long-term leads:
- Monthly newsletter (low-frequency; high-value; non-pushy)
- Quarterly re-evaluation: is the lead now showing intent signals?
- Suppress from bulk emails if disengaged for 90+ days
- Run targeted re-engagement before removing from the database

---

## Email Sequence Templates

### Re-Engagement Sequence (3 emails, 3 weeks)

**Email 1 — The re-introduction**
Subject: "It's been a while — here's what's new"
- Brief acknowledgement that they haven't heard from you in a while
- Genuinely new or useful content since last contact
- Low-commitment CTA

**Email 2 — The value prompt**
Subject: "[Resource] that [Company type] teams are finding useful"
- Share a high-value, directly relevant piece
- Reference their original interest (content they downloaded, topic they engaged with)
- Invite engagement; not a sales push

**Email 3 — The honest ask**
Subject: "Should we stay in touch?"
- Direct, honest tone
- Acknowledge they may not be ready or interested
- Binary CTA: "Yes, keep sharing useful content" / "No, remove me from this list"
- Anyone who doesn't engage: suppress from further automated nurture

### Event Follow-Up Sequence (3 emails, 10 days)

**Email 1 (Day 0): Immediate follow-up**
- Thank them for attending / express regret they missed it
- Deliver the recording or key summary
- Ask one qualifying question (reply-based or form-based)

**Email 2 (Day 3): Deepen the theme**
- Build on the event topic with a related resource
- "Given your interest in [topic], you might also find [X] useful"

**Email 3 (Day 10): The next step**
- Based on engagement with emails 1 and 2, offer an appropriate next step
- High-engagers: demo or consultation offer
- Low-engagers: lower-commitment resource with gentle check-in

---

## Output Formats

### Nurture Workflow Design Document
Per workflow:
- Trigger and audience definition
- Content map by stage
- Logic diagram (including branches and exits)
- Email-by-email brief (subject line, message, CTA)
- Graduation criteria
- Connection to next workflow

### Nurture Content Audit
Table of available content assets mapped to:
- Nurture stage (1–4)
- Persona or segment
- Format
- Quality rating
- Gap identification

### Nurture Performance Report
Per sequence:
- Open rate and CTR per email step
- Drop-off rate at each step
- Graduation rate (nurture → SQL)
- Time in nurture before graduation
- Revenue influence from nurtured leads

---

## Common Mistakes to Avoid
- **Leading with a demo request in Email 1.** Trust is earned before a commercial ask lands.
- **One nurture sequence for all leads.** A pricing-page visitor and a guide-downloader have different intent. Segment accordingly.
- **No graduation logic.** Leads who are ready for sales should exit nurture immediately, not wait for the end of the sequence.
- **Nurture content that doesn't advance the relationship.** If each email is self-contained and unconnected to the prior one, it's a drip, not nurture.
- **Ignoring disengaged contacts.** Sending nurture to contacts who haven't engaged in 90+ days damages deliverability. Suppress or re-engage specifically.

---

## Quality Check
Before submitting, ask:
- [ ] Is the nurture sequence segmented by entry behaviour and persona?
- [ ] Does content progression build trust before requesting a commercial action?
- [ ] Are there branch conditions based on engagement behaviour, not just time?
- [ ] Is graduation criteria defined — and does it trigger an immediate sales notification?
- [ ] Is there a long-term nurture or suppression path for leads that don't graduate?
