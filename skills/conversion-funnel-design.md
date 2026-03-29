# Conversion Funnel Design

## Purpose
Architect end-to-end conversion flows that move prospects efficiently from first awareness to purchase decision — reducing friction, building trust, and increasing the proportion of visitors who take the desired action.

---

## When to Use This Skill
- Low conversion rates at any stage of the funnel
- Launching a new product, offer, or campaign
- Redesigning a website, landing page, or onboarding flow
- Moving from a generalist website to targeted landing pages
- Scaling paid media and needing better post-click conversion

---

## Briefing Checklist
Before starting, confirm:
1. **Conversion goal** — What is the primary conversion event? (Demo request, trial sign-up, purchase, lead form)
2. **Audience** — Which segment and persona are we designing for?
3. **Traffic source** — Paid, organic, direct, referral? (Source shapes intent and prior exposure)
4. **Current baseline** — What are the current conversion rates at each stage?
5. **Constraints** — Technology platform, brand guidelines, legal requirements?

---

## Funnel Structure

A conversion funnel has four layers. Each must be explicitly designed:

```
ATTRACT → ENGAGE → CONVERT → CONFIRM
```

| Layer | Goal | Lever |
|---|---|---|
| **Attract** | Get the right visitor to the right page | Traffic targeting, SEO, ad creative |
| **Engage** | Hold attention and build conviction | Messaging, proof, UX clarity |
| **Convert** | Drive the target action | CTA, offer, friction reduction |
| **Confirm** | Reinforce the decision and set next steps | Thank-you page, onboarding, follow-up |

Most CRO work focuses on conversion mechanics. The most common failure is earlier — in engagement — where prospects don't find what they expected or don't believe the claim.

---

## Micro-Conversions and Leading Indicators

Define the full conversion path, not just the final event:

| Funnel Stage | Micro-Conversion | Measurement |
|---|---|---|
| Page arrival | Time on page > 30s | Session duration |
| Engagement | Scrolled 75% of page | Scroll depth tracking |
| Consideration | Clicked into pricing, case study, or demo | Click-through rate |
| Intent | Opened demo booking flow | Funnel initiation rate |
| Conversion | Submitted form / completed booking | Conversion rate |
| Confirmation | Attended demo / activated trial | Show rate / activation rate |

Tracking micro-conversions reveals where buyers stall before the main event.

---

## Process

### Step 1 — Map the Current Funnel State
Document the current flow from entry to conversion:
- All pages in the flow
- Current conversion rates at each step
- Traffic volume at each step
- Drop-off rates and where they are highest

Tools: Google Analytics 4 funnel exploration, Hotjar session recordings, heatmaps, CRM pipeline data.

### Step 2 — Diagnose Drop-Off Causes
For each high-friction stage, identify the root cause:

| Root Cause | Symptom | Fix |
|---|---|---|
| **Message mismatch** | High bounce rate; low scroll depth | Align page headline to traffic source intent |
| **Credibility gap** | Long time on page; no conversion | Add proof: case studies, reviews, logos, data |
| **Offer clarity** | High pricing page drop-off | Simplify pricing; improve tier differentiation |
| **Friction** | Form abandonment | Reduce form fields; progressive disclosure |
| **Trust deficit** | High exit rate on conversion page | Add guarantees, security signals, social proof |
| **Wrong audience** | Low engagement across all metrics | Fix targeting upstream |

### Step 3 — Design the Ideal Funnel
For the target conversion event, design:

**Landing Page Anatomy**
1. Hero — headline (outcome-led), subheadline (how), hero visual
2. Social proof bar — logos, review aggregate, key stat
3. Problem articulation — describe the pain in customer language
4. Solution overview — what you do and how it works
5. Proof section — case study, testimonial, or data
6. Offer and CTA — what they get; what they need to do
7. Objection handling — FAQ or trust signals
8. Final CTA — repeat the conversion action

Each section has a job. If a section doesn't move the visitor toward conversion, remove it.

**CTA Design Principles**
- Lead with the benefit, not the action ("Get your free trial" not "Submit")
- One primary CTA per page; secondary CTAs should be visually subordinate
- Reduce commitment perception: "Book a 30-minute demo" vs "Talk to sales"
- Test button copy, colour, and placement

**Form Design Principles**
- Only ask for what is absolutely necessary at this stage
- Multi-step forms reduce perceived friction (even if total fields are equal)
- Progressive disclosure: capture email first; ask qualifying questions later
- Inline validation and clear error states reduce abandonment

### Step 4 — Build the Test Roadmap
Prioritise tests using ICE scoring:

| Test | Impact (1–10) | Confidence (1–10) | Ease (1–10) | ICE Score |
|---|---|---|---|---|
| Change hero headline | 8 | 7 | 9 | 504 |
| Add customer logo bar | 6 | 8 | 9 | 432 |
| Reduce form fields | 7 | 6 | 7 | 294 |

Run highest-ICE tests first. Set clear success metrics before launching each test.

### Step 5 — Define Measurement and Reporting
Set up tracking for:
- Funnel step completion rates
- Conversion rate by traffic source, device, and segment
- Time to convert
- Cost per conversion by channel

Review weekly for active campaigns; monthly for ongoing optimisation.

---

## Output Formats

### Funnel Map
Visual showing:
- Entry points and traffic sources
- All pages and steps in the flow
- Conversion rates at each step
- Identified friction points and root causes

### Landing Page Brief
For each conversion page:
- Audience and intent
- Primary conversion goal
- Recommended page structure and section-by-section rationale
- CTA copy and placement
- Proof requirements (social proof, case studies, data)
- Objections to handle

### CRO Testing Roadmap
- Prioritised test backlog (ICE scored)
- Test design (control vs variant)
- Success metric and statistical threshold
- Timeline and owner

### Conversion Playbook
- Funnel architecture and rationale
- Page-level briefs
- CTA guidelines
- Form design standards
- Testing protocol

---

## Common Mistakes to Avoid
- **Optimising the wrong stage.** Fixing the form doesn't help if the problem is upstream in messaging.
- **Testing without a hypothesis.** "Let's see what happens" is not a test. Define what you expect and why.
- **Underpowered tests.** Small sample sizes produce false positives. Calculate minimum detectable effect before testing.
- **One CTA for all intent levels.** A buyer ready to purchase and a buyer just exploring need different CTAs.
- **Ignoring mobile.** If more than 40% of traffic is mobile, mobile UX must be designed first, not as an afterthought.

---

## Quality Check
Before submitting, ask:
- [ ] Is every funnel step mapped with a conversion rate (actual or estimated)?
- [ ] Are drop-off causes diagnosed by evidence, not assumption?
- [ ] Does every page have a single, clear primary conversion goal?
- [ ] Is the test roadmap ICE-scored and prioritised?
- [ ] Is there tracking in place to measure the impact of each change?
