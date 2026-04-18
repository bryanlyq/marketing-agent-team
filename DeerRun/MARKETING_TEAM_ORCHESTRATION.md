# Marketing Agent Team Orchestration Framework

**Version:** 1.0
**Date:** 2026-03-24
**Status:** Active

---

## Table of Contents

1. [Overview](#overview)
2. [Team Structure](#team-structure)
3. [Role Definitions](#role-definitions)
4. [Skill Inventory](#skill-inventory)
5. [Orchestration Patterns](#orchestration-patterns)
6. [Workflow Examples](#workflow-examples)
7. [Data Flow & Dependencies](#data-flow--dependencies)
8. [Agent Communication Protocol](#agent-communication-protocol)

---

## Overview

This document defines how the Marketing Agent Team operates as a coordinated system. Seven specialized agents work under the direction of a Marketing Director to execute integrated marketing strategies.

### Key Principles

- **Specialization**: Each agent has deep expertise in their domain
- **Coordination**: Director routes work and manages dependencies
- **Handoff Protocol**: Clear inputs/outputs between agents
- **Feedback Loops**: Results inform strategy adjustments
- **Scalability**: New skills add capability without breaking workflows

---

## Team Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                  MARKETING DIRECTOR AGENT                       │
│              (Strategic Coordination & Routing)                  │
└────────────────┬────────────────────────────────────────────────┘
                 │
    ┌────────────┼────────────┬──────────────┬──────────┬──────────┬──────────┐
    │            │            │              │          │          │          │
    ▼            ▼            ▼              ▼          ▼          ▼          ▼
┌────────────┐ ┌──────────┐ ┌─────────┐ ┌──────────┐ ┌────────┐ ┌───────┐ ┌────────┐
│  RESEARCH  │ │ SOCIAL   │ │ GROWTH  │ │ANALYTICS │ │ CONTENT│ │ PAID  │ │PRODUCT │
│   INTEL    │ │  MEDIA   │ │    &    │ │ REPORTER │ │CREATOR │ │MARKET.│ │MARKETER│
│   AGENT    │ │  AGENT   │ │EXPERIMENT│ │  AGENT   │ │ AGENT  │ │ AGENT │ │ AGENT  │
└────────────┘ └──────────┘ └─────────┘ └──────────┘ └────────┘ └───────┘ └────────┘
    │            │            │              │          │          │          │
    │            │            │              │          │          │          │
Competitive    Social media   A/B tests    Dashboards  Copywriting Ad spend  Feature
analysis       monitoring     Landing page  Metrics    Blog posts  ROI       messaging
Market trends  Sentiment      CRO testing   Attribution Email       Budget    Launches
Positioning    Competitor ads Multivariate  Reporting  Social copy  Optimize  Sales
Audience       Performance    Testing       Attribution SEO content Platform   enablement
```

---

## Role Definitions

### 1. RESEARCH INTEL AGENT 🔍

**Purpose**: Provide strategic insights and competitive context for all marketing initiatives

**Primary Responsibilities**:
- Competitive landscape analysis
- Market trend identification
- Audience segmentation & insights
- Positioning framework development
- Industry benchmarking

**Key Skills**:
- `competitor-analysis` - Deep analysis of competitor strategies, messaging, positioning
- `market-research` - Trend identification, market opportunity assessment
- `audience-segmentation` - Behavioral, demographic, psychographic segmentation
- `positioning-framework` - Value prop refinement, messaging architecture

**Outputs**:
- Competitive intelligence reports
- Audience personas & segments
- Positioning recommendations
- Market opportunity assessments

**Triggers**: Research requests, quarterly competitive reviews, new campaign planning, product launches

**Handoff Recipients**: Director, Product Marketer, Social Media Agent, Content Creator

---

### 2. SOCIAL MEDIA AGENT 📱 ⭐ **NEW ROLE**

**Purpose**: Master social media strategy, competitor analysis, and social advertising landscape

**Primary Responsibilities**:
- Social media platform monitoring (TikTok, Instagram, LinkedIn, X/Twitter, YouTube)
- Competitor social media strategy analysis
- Competitor ad library monitoring (Meta, Google, LinkedIn)
- Social sentiment & engagement analysis
- Trend identification & viral potential assessment
- Influencer & community analysis
- Social media content calendar recommendations
- Paid social ad copy & creative analysis

**Key Skills**:
- `social-media-monitoring` - Real-time platform tracking, engagement analysis, community health
- `competitor-social-analysis` - Competitor posting patterns, audience size, engagement rates, content strategy
- `competitor-ads-analysis` - Ad copy variations, targeting, creative assets, ad spend estimation
- `social-trends-analysis` - Viral potential, hashtag research, trend adoption
- `social-sentiment-analysis` - Brand mentions, sentiment tracking, crisis detection
- `influencer-analysis` - Audience quality, engagement authenticity, partnership fit
- `paid-social-audit` - Facebook/Instagram/TikTok/LinkedIn ad strategy analysis
- `social-content-strategy` - Platform-specific content recommendations, posting schedules, growth tactics

**Outputs**:
- Competitor social strategy reports
- Competitive ad analysis (creative, copy, targeting variations)
- Trend & opportunity reports
- Social listening dashboards
- Content calendar recommendations
- Influencer partnership assessments
- Paid social competitive benchmarking

**Triggers**:
- New product launch
- Paid social campaign planning
- Content strategy development
- Competitor monitoring (continuous)
- Crisis management
- Trend analysis requests

**Handoff Recipients**: Director, Content Creator, Paid Marketing Agent, Growth Agent

**Data Sources**:
- Native platform APIs (where available)
- Ad library access (Meta, Google, LinkedIn, TikTok)
- Social listening tools
- Competitor websites & social profiles
- Influencer databases

---

### 3. GROWTH & EXPERIMENTATION AGENT 🧪

**Purpose**: Drive revenue through testing, optimization, and data-driven experimentation

**Primary Responsibilities**:
- A/B and multivariate test design
- Landing page conversion rate optimization (CRO)
- Funnel analysis & bottleneck identification
- Hypothesis generation & validation
- Test prioritization & roadmapping

**Key Skills**:
- `ab-test-setup` ✓ **EXISTING** - Hypothesis design, sample size calculation, test methodology
- `page-cro` - Conversion optimization principles, layout testing, CTA optimization
- `funnel-analysis` - Bottleneck identification, drop-off analysis, micro-conversion tracking
- `hypothesis-generation` - Data-driven idea generation, experimentation roadmap

**Outputs**:
- Test specifications & designs
- CRO recommendations
- Funnel reports with improvement priorities
- Experimentation roadmaps

**Triggers**: Conversion improvement requests, new landing pages, campaign optimization, quarterly reviews

**Handoff Recipients**: Content Creator, Analytics Agent, Director

---

### 4. ANALYTICS REPORTER AGENT 📊

**Purpose**: Measure, track, and report on marketing performance across all channels

**Primary Responsibilities**:
- Analytics platform setup & configuration
- Metrics framework definition
- Performance dashboard creation
- Attribution modeling
- Data validation & integrity
- Regular performance reporting

**Key Skills**:
- `analytics-setup` - GA4/analytics implementation, event tracking, data warehouse setup
- `analytics-tracking` ✓ **REFERENCED** - A/B test measurement, event specification
- `performance-reporting` - Dashboard design, automated reporting, insights generation
- `attribution-modeling` - Multi-touch attribution, conversion path analysis
- `data-validation` - Quality assurance, anomaly detection, data health checks

**Outputs**:
- Performance dashboards (real-time & scheduled)
- Attribution reports
- Analytics implementation specs
- Data quality reports

**Triggers**: New campaigns, test launches, monthly reviews, stakeholder reporting

**Handoff Recipients**: All agents (provides measurement for all), Director

---

### 5. CONTENT CREATOR AGENT ✍️

**Purpose**: Produce compelling, optimized content across channels

**Primary Responsibilities**:
- Blog & SEO content creation
- Email marketing copy & campaigns
- Social media content (posts, captions, hashtags)
- Landing page copywriting
- Ad copy variation development
- Content strategy & calendar

**Key Skills**:
- `copywriting` - Persuasive writing, positioning expression, audience adaptation
- `seo-content` - Keyword research, optimization, content structure, link strategy
- `email-marketing` - Campaign design, subject lines, segmentation, automation
- `social-content-creation` - Platform-native content, hashtag strategy, engagement tactics
- `content-strategy` - Editorial calendar, content pillars, SEO roadmap

**Outputs**:
- Blog posts & content pieces
- Email campaign sequences
- Social media content calendar
- Landing page copy
- Ad copy variations
- Content performance briefs

**Triggers**: Campaign launches, blog calendar, product announcements, seasonal campaigns

**Handoff Recipients**: Paid Marketing Agent, Social Media Agent, Analytics Agent

---

### 6. PAID MARKETING AGENT 💰

**Purpose**: Optimize customer acquisition and conversion through paid channels

**Primary Responsibilities**:
- Campaign strategy & planning (Google, Meta, LinkedIn, TikTok, etc.)
- Ad copy & creative testing
- Budget allocation & optimization
- Bid strategy development
- Platform-specific tactics & automation
- ROAS monitoring & improvement

**Key Skills**:
- `ad-strategy` - Campaign structure, audience targeting, channel selection
- `paid-optimization` - Bid management, conversion tracking, audience optimization
- `budget-allocation` - Channel prioritization, spending curves, ROI optimization
- `platform-specific-tactics` - Google Ads, Facebook Ads, LinkedIn Ads, TikTok Ads expertise
- `creative-testing` - Ad variation design, creative best practices, performance prediction

**Outputs**:
- Campaign specifications
- Ad copy & creative variations
- Budget allocation recommendations
- Platform setup & configuration
- Performance optimization reports

**Triggers**: Campaign launches, quarterly budget planning, ROAS targets, new platforms

**Handoff Recipients**: Content Creator (copy/creative), Analytics Agent (measurement), Director

---

### 7. PRODUCT MARKETER AGENT 🎯

**Purpose**: Align product strategy with market needs and drive product launches

**Primary Responsibilities**:
- Product positioning & messaging
- Feature prioritization & communication
- Launch planning & go-to-market strategy
- Competitive feature analysis
- Sales enablement
- Product-market fit validation

**Key Skills**:
- `launch-planning` - GTM strategy, timeline, cross-functional coordination
- `feature-positioning` - Benefit messaging, competitive advantages, value articulation
- `competitive-messaging` - Differentiation, competitive analysis, positioning strategy
- `sales-enablement` - Materials creation, training, competitive battle cards
- `product-market-fit` - Validation, feedback integration, positioning iteration

**Outputs**:
- Launch plans & GTM strategy
- Positioning & messaging documents
- Feature comparison matrices
- Sales materials
- Launch communication plans

**Triggers**: New product/feature, competitive threats, positioning reviews, launch planning

**Handoff Recipients**: Content Creator, Research Intel Agent, Director, Paid Marketing Agent

---

### 8. MARKETING DIRECTOR AGENT 🎬

**Purpose**: Strategic coordination, priority management, and workflow orchestration

**Primary Responsibilities**:
- Request routing to appropriate agent(s)
- Dependency management across workflows
- Priority & resource allocation
- Cross-agent communication facilitation
- Strategy alignment
- Bottleneck resolution

**Key Skills**:
- `orchestration` - Workflow coordination, dependency mapping
- `strategic-planning` - Goal setting, metric definition, roadmap creation
- `prioritization` - Impact/effort assessment, resource allocation

**Decision Criteria**:

| Request Type | Primary Agent | Supporting Agents |
|---|---|---|
| "Increase homepage conversion" | Growth & Experimentation | Content, Analytics, Research |
| "Launch new product" | Product Marketer | Research, Content, Paid, Analytics |
| "Improve organic reach" | Content Creator | Research, Analytics, Social Media |
| "Optimize ad spend" | Paid Marketing | Analytics, Growth, Research |
| "Monitor competitors" | Social Media + Research | All (context-dependent) |
| "Analyze social opportunity" | Social Media | Research, Content, Paid |
| "Competitor ads benchmarking" | Social Media | Paid Marketing, Research |
| "Create content calendar" | Content Creator | Social Media, Research, Analytics |

---

## Skill Inventory

### Existing Skills ✓
- `ab-test-setup` - A/B testing & experimentation framework (v1.1.0)
- `analytics-tracking` - Referenced in ab-test-setup

### Planned Skills 🔄

#### High Priority (Enable core workflows)
- `page-cro` - Conversion rate optimization principles
- `copywriting` - Core marketing copy creation
- `competitor-analysis` - Competitive intelligence
- `social-media-monitoring` - Platform monitoring & engagement
- `competitor-social-analysis` - Social strategy & performance analysis
- `competitor-ads-analysis` - Ad library monitoring & analysis

#### Medium Priority (Enhance specialization)
- `seo-content` - SEO content creation & optimization
- `email-marketing` - Email campaign strategy & execution
- `analytics-setup` - Analytics implementation
- `performance-reporting` - Dashboard & reporting
- `ad-strategy` - Paid advertising strategy
- `paid-social-audit` - Paid social benchmarking

#### Lower Priority (Advanced features)
- `funnel-analysis` - Conversion funnel optimization
- `audience-segmentation` - Advanced targeting & segmentation
- `influencer-analysis` - Influencer partnership evaluation
- `launch-planning` - Product launch orchestration
- `social-trends-analysis` - Trend identification & virality assessment

---

## Orchestration Patterns

### Pattern 1: Linear Workflow (Sequential)

Used when output of one agent feeds directly into the next.

```
[Research Intel]
    ↓ (competitive insights)
[Growth Agent]
    ↓ (test ideas)
[Content Creator]
    ↓ (copy variants)
[Paid Marketing]
    ↓ (campaign)
[Analytics]
    ↓ (results)
[Director] → Report back to user
```

**Example**: Competitor ad analysis → Create test variants → Write copy → Launch paid test → Measure results

---

### Pattern 2: Parallel Workflow (Concurrent)

Used when agents work independently but results are later combined.

```
                    [Research Intel]
                           ↓
        ┌────────────────────┼────────────────────┐
        ↓                    ↓                    ↓
    [Content]          [Social Media]       [Product Marketer]
    Blog posts         Content calendar     Feature messaging
        │                    │                    │
        └────────────────────┼────────────────────┘
                             ↓
                    [Director Coordinates]
                    Combined launch plan
```

**Example**: Launch campaign with blog, social content, and product messaging

---

### Pattern 3: Feedback Loop Workflow

Used for iterative optimization and learning.

```
[Research] → [Test Design] → [Execution] → [Analytics]
    ↑                                           ↓
    └───────────────────────────────────────────┘
              Learnings inform next test
```

**Example**: Hypothesis generation → A/B test → Results analysis → Refined hypothesis

---

### Pattern 4: Competitive Monitoring (Continuous)

Social Media and Research agents run continuously, surfacing alerts.

```
[Social Media Agent] (continuous monitoring)
        ↓
    [Alert Triggers]
        ↓
    Competitor launches new campaign
    New trend emerging
    Sentiment shift detected
        ↓
[Director] → Routes to appropriate agents
```

---

## Workflow Examples

### Example 1: Landing Page Optimization Campaign

**Goal**: Improve pricing page conversion rate by 20%

```
1. RESEARCH INTEL AGENT
   ├─ Analyze competitor pricing pages
   ├─ Study audience pain points (from social listening)
   └─ Output: 3 core improvement hypotheses
        ↓
2. SOCIAL MEDIA AGENT (parallel)
   ├─ Monitor competitor pricing page social mentions
   ├─ Analyze competitor social ads (pricing-focused)
   └─ Output: Social proof opportunities, messaging trends
        ↓
3. GROWTH & EXPERIMENTATION AGENT
   ├─ Receive: hypotheses + social insights
   ├─ Design 3 A/B tests with variants:
   │  ├─ Variant A: Enhanced social proof
   │  ├─ Variant B: Different value prop framing
   │  └─ Variant C: Risk reversal messaging
   └─ Calculate sample size for 20% lift detection
        ↓
4. CONTENT CREATOR AGENT (parallel with step 3)
   ├─ Write copy for each variant
   ├─ Create social proof elements
   └─ Output: Copy docs with variants
        ↓
5. ANALYTICS AGENT
   ├─ Set up A/B test tracking
   ├─ Define metrics:
   │  ├─ Primary: Conversion rate
   │  ├─ Secondary: Time on page, CTR
   │  └─ Guardrails: Bounce rate
   └─ Output: Measurement spec
        ↓
6. PAID MARKETING AGENT (optional)
   ├─ Create paid campaigns to drive test traffic
   ├─ Test ad variations promoting pricing page
   └─ Output: Campaign specs + budget
        ↓
7. DIRECTOR
   ├─ Coordinates test launch
   ├─ Monitors for issues
   └─ Output: "Test live, monitoring in place"
        ↓
8. ANALYTICS AGENT (ongoing)
   ├─ Daily health checks
   ├─ Alert if: anomalies, guardrail violations
   └─ Weekly: Preliminary performance reports
        ↓
9. GROWTH AGENT (end of test)
   ├─ Analyze results
   ├─ Determine winner
   ├─ If significant win: rollout recommendation
   ├─ If unclear: next test recommendations
   └─ Output: Test report + next steps
        ↓
10. DIRECTOR → User
    ├─ Results summary
    ├─ Implementation recommendation
    └─ Learning captured for future tests
```

**Timeline**: 2-3 weeks (research + setup) + test duration (depends on traffic)

**Success Metric**: 20% lift achieved, learnings documented

---

### Example 2: New Product Launch Campaign

**Goal**: Launch new product with coordinated marketing

```
PARALLEL WORKSTREAMS:

Workstream A: Strategy & Positioning
├─ RESEARCH INTEL
│  ├─ Competitive feature analysis
│  ├─ Positioning vs. competitors
│  └─ Audience opportunity assessment
│       ↓
├─ PRODUCT MARKETER
│  ├─ Define feature benefits & messaging
│  ├─ Create launch narrative
│  └─ Competitive battle cards
│       ↓
└─ DIRECTOR (orchestrates, manages timeline)

Workstream B: Content & Social
├─ CONTENT CREATOR
│  ├─ Launch announcement blog post
│  ├─ Email campaign sequence
│  ├─ Sales materials & fact sheets
│  └─ Landing page copy
│       ↓
├─ SOCIAL MEDIA AGENT
│  ├─ Social content calendar (2 weeks pre + launch)
│  ├─ Influencer outreach strategy
│  ├─ Competitor response monitoring plan
│  └─ Sentiment tracking setup
│       ↓
└─ DIRECTOR (coordinates timing)

Workstream C: Paid Acquisition
├─ PAID MARKETING AGENT
│  ├─ Paid campaign structure
│  ├─ Audience targeting definition
│  ├─ Budget allocation across channels
│  └─ Creative briefs
│       ↓
├─ CONTENT CREATOR (supplies ad copy/creative)
│  └─ Ad copy variations
│       ↓
└─ DIRECTOR (launch coordination)

Workstream D: Measurement
├─ ANALYTICS AGENT
│  ├─ Launch tracking implementation
│  ├─ Dashboard creation
│  ├─ Attribution setup
│  └─ Success metrics definition
│       ↓
└─ All other agents (report results)

CONVERGENCE:
Day 1 (Launch):
├─ Blog published + social push
├─ Email campaigns deployed
├─ Paid campaigns go live
├─ Sales team enabled
├─ Influencer posts scheduled
└─ Monitoring active

Week 1-2:
├─ Social media monitoring
├─ Paid campaign optimization
├─ Email performance tracking
└─ Sentiment analysis

Result:
└─ Director gets daily brief, weekly impact report
```

**Timeline**: 4-6 weeks (planning) + ongoing (monitoring)

**Success Metric**: Launch goals (signups, revenue, awareness) achieved

---

### Example 3: Competitor Response Campaign

**Goal**: Respond to competitor's new campaign/feature announcement

```
TRIGGER: Social Media Agent detects competitor announcement

T+0 (Minutes)
└─ Social Media Agent
   ├─ Flags opportunity/threat
   ├─ Provides initial competitive analysis
   │  ├─ Ad copy
   │  ├─ Landing page content
   │  ├─ Social messaging
   │  └─ Target audience
   └─ → Director receives alert

T+30 minutes
└─ Director routes for parallel analysis:

├─ Research Intel Agent
│  ├─ Competitive positioning analysis
│  ├─ Market impact assessment
│  └─ Our response options (3 scenarios)
│
├─ Product Marketer Agent
│  ├─ Feature comparison
│  ├─ Competitive advantage articulation
│  └─ Messaging recommendations
│
├─ Content Creator Agent
│  ├─ Social response content (if aggressive response)
│  └─ Blog counter-argument (if thought leadership response)
│
└─ Social Media Agent (continued)
   ├─ Monitor sentiment & conversation
   ├─ Track competitor ad spend & targeting
   └─ Identify response opportunities/risks

T+2 hours
└─ Director synthesis:
   ├─ Recommended response strategy
   ├─ Channel priorities
   ├─ Timeline
   └─ Resource requirements

Response Options:
A) Thought leadership (Blog + own social)
B) Direct competitive counter (Ad campaign)
C) Monitor and wait (Gather more data)
D) Feature announcement (If applicable)

Implementation:
├─ If A: Content Creator publishes, Paid Marketing amplifies
├─ If B: Paid Marketing launches competitive campaign
├─ If C: Social Media continues monitoring, brief daily
└─ If D: Full launch workflow (see Example 2)
```

**Timeline**: 2-4 hours (alert to decision) + execution time

**Success Metric**: Competitive threat neutralized or market position strengthened

---

### Example 4: Continuous Social Media Competitive Monitoring

**Goal**: Stay ahead of competitor moves and market trends

```
CONTINUOUS CYCLE (Daily/Weekly):

SOCIAL MEDIA AGENT
├─ Daily Monitoring Tasks:
│  ├─ Competitor social media updates (all platforms)
│  ├─ Ad library changes (new ads, variations)
│  ├─ Engagement metrics tracking
│  ├─ Sentiment analysis (brand mentions)
│  ├─ Trending topic relevance check
│  └─ Influencer activity related to category
│
├─ Weekly Summary (every Monday):
│  ├─ Competitor social strategy shift analysis
│  ├─ Emerging trends in category
│  ├─ Audience sentiment trends
│  ├─ Ad spend estimation for competitors
│  └─ Opportunities/threats for coming week
│
└─ Alert Triggers (immediate escalation):
   ├─ Major competitor campaign launch
   ├─ Negative sentiment surge
   ├─ Viral trend emergence (our category)
   ├─ Influencer partnerships
   └─ Product announcements

DIRECTOR
├─ Receives: Weekly summary + daily alerts
├─ Decision points:
│  ├─ Does this require immediate response?
│  ├─ Which agents should be engaged?
│  └─ New initiative needed?
└─ Routes to: Relevant agents for deeper analysis

RESEARCH INTEL AGENT (weekly)
├─ Receives: Social media findings
├─ Provides: Strategic context
│  ├─ What does this mean for positioning?
│  ├─ Market implications?
│  └─ Our recommended response?

CONTENT CREATOR AGENT (triggered)
├─ Receives: Trend alerts
├─ Decisions: Can we leverage this trend?
│  ├─ Blog post opportunity?
│  ├─ Social content angle?
│  └─ Campaign idea?

Outputs:
├─ Weekly competitive intelligence report
├─ Monthly trend analysis
├─ Quarterly strategic assessment
└─ Real-time alerts for urgent issues
```

---

## Data Flow & Dependencies

### Information Flow Map

```
INPUTS (External)
├─ Competitor websites & social profiles
├─ Ad libraries (Meta, Google, LinkedIn, TikTok)
├─ Social media APIs
├─ Analytics platforms
├─ Customer feedback/surveys
└─ Market data sources

        ↓

[RESEARCH INTEL]  ←→  [SOCIAL MEDIA]  ←→  [PRODUCT MARKETER]
        ↓                   ↓                       ↓
        └───────────────────┼───────────────────────┘
                            ↓
                  [GROWTH & EXPERIMENTATION]
                    ↓              ↓
            [CONTENT CREATOR] ← [PAID MARKETING]
                    │                │
                    └────────┬───────┘
                             ↓
                    [ANALYTICS REPORTER]
                             ↓
                   [DIRECTOR - Aggregates]
                             ↓
OUTPUT (to User)
├─ Reports & insights
├─ Recommendations
├─ Campaign implementations
└─ Performance tracking
```

### Critical Dependencies

| Agent | Depends On | For |
|---|---|---|
| Growth & Experimentation | Research Intel, Content | Test hypotheses, copy variants |
| Content Creator | Research Intel, Social Media | Audience insights, trend angles |
| Paid Marketing | Content Creator, Growth Agent | Ad copy, landing page validation |
| Product Marketer | Research Intel, Social Media | Market positioning, competitor moves |
| Analytics | All agents | Measurement specs, metrics definition |
| Social Media | Research Intel | Competitive context, positioning |
| Director | All agents | Results aggregation, orchestration |

### Data Handoff Format

**Standard Handoff Package** (Agent A → Agent B):

```markdown
## Handoff: [Agent A] → [Agent B]

**Context**: What problem are we solving?
**Key Findings**: Top 3-5 insights from Agent A
**Data Provided**:
- [Specific data files/results]
- [Metrics/numbers]
- [References/sources]

**Question for Agent B**: What specific question should Agent B answer?
**Timeline**: When is this needed?
**Acceptance Criteria**: How do we know Agent B succeeded?

---
## Response from Agent B
[Analysis/deliverable]
```

---

## Agent Communication Protocol

### Request Routing Rules

**Rule 1: Single Clear Owner**
- Each request has ONE primary responsible agent
- Other agents play supporting roles
- Director assigns and tracks ownership

**Rule 2: Dependency Declaration**
- Agent explicitly states needs from other agents
- Director identifies and schedules dependencies
- Sequential vs. parallel work determined by Director

**Rule 3: Escalation Path**
- Agent → Director (conflicts, resource issues)
- Director → User (strategic decisions, budget, timeline)

### Response Standards

**All agent responses include**:
1. **Summary** (1-2 sentences): What we did
2. **Key Findings** (3-5 bullets): Main insights
3. **Data/Deliverables** (links/files): What you can use
4. **Next Steps** (recommended actions): Where to go from here
5. **Handoff** (if applicable): Who needs this next?

**Example Response Structure**:
```markdown
## [Agent Name] Analysis: [Topic]

**Summary**: We analyzed [X] and found [Y].

**Key Findings**:
- Finding 1 with data point
- Finding 2 with data point
- Finding 3 with data point

**Deliverables**:
- [File/report name]
- [Dashboard/visualization]
- [Data sheet]

**Recommended Next Steps**:
1. Action A (owner: [Agent])
2. Action B (owner: [Agent])

**Questions for Director**:
- Any strategic decisions needed?
```

### Cross-Agent Communication

**When Agent A needs input from Agent B**:

1. Agent A sends structured request to Director
2. Director prioritizes and routes to Agent B
3. Agent B provides response with acceptance criteria met
4. Agent A proceeds with integration
5. Director tracks completion

**Exception**: High-frequency coordination (e.g., Analytics + Growth Agent during test) may happen directly with Director oversight.

---

## Workflow Decision Tree

```
REQUEST COMES TO DIRECTOR

├─ Is it research/competitive analysis?
│  └─ → RESEARCH INTEL + SOCIAL MEDIA (if ad/social related)
│
├─ Is it social media analysis?
│  └─ → SOCIAL MEDIA (primary) + RESEARCH (supporting)
│
├─ Is it conversion/testing related?
│  └─ → GROWTH AGENT (primary) + CONTENT + ANALYTICS
│
├─ Is it content creation?
│  └─ → CONTENT CREATOR (primary) + RESEARCH + SOCIAL MEDIA
│
├─ Is it paid advertising?
│  └─ → PAID MARKETING (primary) + CONTENT + ANALYTICS
│
├─ Is it analytics/measurement?
│  └─ → ANALYTICS (primary) + requesting agent
│
├─ Is it product related?
│  └─ → PRODUCT MARKETER (primary) + RESEARCH + CONTENT + PAID
│
├─ Is it a multi-faceted initiative?
│  └─ → Determine workstreams, parallelize, set coordination points
│
└─ Is it urgent/competitive threat?
   └─ → Alert SOCIAL MEDIA + RESEARCH, brief DIRECTOR, execute response
```

---

## Implementation Roadmap

### Phase 1: Core Skills (Weeks 1-4)
- [ ] `social-media-monitoring` - Enable continuous competitive watch
- [ ] `competitor-ads-analysis` - Competitor ad intelligence
- [ ] `competitor-social-analysis` - Social strategy analysis
- [ ] `copywriting` - Foundational content creation

### Phase 2: Optimization (Weeks 5-8)
- [ ] `page-cro` - Landing page optimization
- [ ] `seo-content` - Organic search content
- [ ] `analytics-setup` - Measurement infrastructure

### Phase 3: Advanced (Weeks 9+)
- [ ] `funnel-analysis` - Conversion funnel optimization
- [ ] `audience-segmentation` - Advanced targeting
- [ ] `social-trends-analysis` - Trend forecasting

---

## Success Metrics & KPIs

### Orchestration Health

| Metric | Target | Cadence |
|---|---|---|
| Request → Delivery Time | <24h for standard requests | Daily |
| Agent Utilization | 80%+ productive time | Weekly |
| Cross-Agent Handoff Success | 95%+ first-time | Weekly |
| Stakeholder Satisfaction | 4.5+/5.0 | Monthly |

### Marketing Impact

| Metric | Target | Cadence |
|---|---|---|
| Experiment Win Rate | >60% statistically significant | Per test |
| Content Performance | 50% increase in engagement | Monthly |
| Conversion Rate Growth | +15% YoY | Quarterly |
| Competitive Position | Market leader in category | Quarterly |

---

## Document Management

**Version**: 1.0
**Last Updated**: 2026-03-24
**Next Review**: 2026-06-24

**Change Log**:
- 2026-03-24: Initial framework document created with 7 agent roles, including new Social Media Manager
