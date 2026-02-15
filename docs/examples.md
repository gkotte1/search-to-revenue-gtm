# Concrete Examples

These examples are generic (no proprietary data) but realistic. Adapt them to your product, market, and stage.

---

## Example 1: AIO-Generated Content Brief for a Bottom-of-Funnel SEO Page

This is the kind of brief an AI assistant would produce when prompted with a target keyword and product context. A human editor would review and refine before handing to a writer.

### Content Brief: "Best project management tools for remote teams"

**Target keyword:** best project management tools for remote teams

**Secondary keywords:** remote project management software, project management for distributed teams, async project management tools

**Search intent:** Commercial investigation. The searcher has decided they need a tool and is evaluating options. They expect a curated list with honest assessments.

**Content type:** Listicle / comparison page

**Target word count:** 2,000 - 2,500 words

**Recommended structure:**

```
H1: Best Project Management Tools for Remote Teams in 2026
  - Introduction (150 words): Why remote teams have different PM needs (async
    communication, timezone handling, integration with remote-first tools).

H2: How We Evaluated These Tools
  - Criteria: async features, integrations, pricing for distributed teams,
    learning curve, mobile experience.

H2: The Top 8 Tools
  H3: [Tool 1] — Best for [specific use case]
    - What it does well (2-3 bullets)
    - Limitations (1-2 bullets)
    - Pricing summary
    - Best for: [team size / type]
  H3: [Tool 2] — Best for [specific use case]
    ... (repeat for each tool)

H2: Comparison Table
  - Side-by-side: features, pricing, best for

H2: How to Choose the Right Tool for Your Team
  - Decision framework based on team size, budget, and work style

H2: FAQ
  - 3-5 questions from People Also Ask data
```

**Questions to answer (from PAA and related searches):**
- What is the best free project management tool for remote teams?
- How do you manage projects across time zones?
- What features should remote project management software have?
- Is Asana or Monday better for remote teams?

**Competitor content notes:**
- Top 3 ranking pages are generic listicles with 10-15 tools, light on evaluation criteria.
- Gap: None of the top pages discuss async-specific features in depth. This is our angle.
- Gap: No page includes a practical decision framework. Most just list tools without helping the reader choose.

**Internal linking opportunities:**
- Link to our "Remote Work Productivity Guide" (TOFU).
- Link to our product's remote features page (conversion page).
- Link to our "How [Product] Compares to [Competitor]" page.

**CTA strategy:**
- Primary CTA: "Try [Product] free for 14 days" (inline after the tool's section, if our product is in the list).
- Secondary CTA: "Download our Remote PM Toolkit" (gated asset at bottom of page).

---

## Example 2: Internal Linking Plan for a Small SaaS Site

This example shows how to structure internal links for a site with ~30 pages to maximize topical authority and link equity flow.

### Site structure

**Pillar page:** /project-management-guide (comprehensive guide, targets the broadest keyword)

**Cluster pages (link TO and FROM the pillar):**

| Page | Target keyword | Link to pillar? | Pillar links to it? |
|---|---|---|---|
| /blog/remote-pm-tools | best remote PM tools | Yes (in intro) | Yes (in "Tools" section) |
| /blog/agile-vs-waterfall | agile vs waterfall | Yes (in context) | Yes (in "Methodologies" section) |
| /blog/project-timeline-template | project timeline template | Yes (in closing) | Yes (in "Planning" section) |
| /blog/team-collaboration-tips | team collaboration tips | Yes (in intro) | Yes (in "Collaboration" section) |
| /blog/sprint-planning-guide | sprint planning guide | Yes (in context) | Yes (in "Agile" section) |

**Conversion pages (link TO these from cluster pages):**

| Conversion page | Linked from |
|---|---|
| /pricing | All BOFU blog posts (comparison, tool lists) |
| /features/remote | Remote-focused blog posts |
| /features/agile | Agile-focused blog posts |
| /demo | All MOFU and BOFU pages |
| /free-trial | All pages (header CTA, not in-content) |

**Cross-linking rules:**

1. Every cluster page links to the pillar page at least once (naturally in context, not forced).
2. The pillar page links to every cluster page in the relevant section.
3. Cluster pages link to each other when topically relevant (e.g., the sprint planning guide links to the agile vs. waterfall post).
4. Every BOFU page links to at least one conversion page (/pricing, /demo, or /free-trial).
5. No page should have more than 3-5 internal links in the body content (beyond navigation).

**Link equity flow:**

```
                    ┌──────────────────────┐
                    │   Pillar Page         │
                    │   /pm-guide           │
                    │   (highest authority) │
                    └──────┬───────────────┘
                           │
           ┌───────────────┼───────────────┐
           │               │               │
    ┌──────▼──────┐ ┌──────▼──────┐ ┌──────▼──────┐
    │ Cluster 1   │ │ Cluster 2   │ │ Cluster 3   │
    │ /remote-pm  │ │ /agile-wf   │ │ /timeline   │
    └──────┬──────┘ └──────┬──────┘ └──────┬──────┘
           │               │               │
           └───────────────┼───────────────┘
                           │
                    ┌──────▼──────┐
                    │ Conversion  │
                    │ /pricing    │
                    │ /demo       │
                    └─────────────┘
```

---

## Example 3: GEO Measurement Plan

This measurement plan covers what to track, where to track it, and what targets to set for a GEO initiative.

### Context

A B2B SaaS company is launching a new GEO initiative to improve the organic-to-revenue pipeline. The goal is to increase marketing-sourced pipeline from organic search by 40% in one quarter.

### Measurement plan

| Stage | Metric | Definition | Tool | Current baseline | Target |
|---|---|---|---|---|---|
| **Acquisition** | Organic sessions | Unique sessions from Google organic | GA4 | 45,000/mo | 60,000/mo |
| **Acquisition** | Organic leads | Form fills from organic sessions | HubSpot | 450/mo | 650/mo |
| **Acquisition** | Organic lead rate | Leads / Sessions | Calculated | 1.0% | 1.1% |
| **Activation** | Signups from organic | Account creations attributed to organic | Product analytics + Segment | 180/mo | 280/mo |
| **Activation** | Activation rate | Users reaching aha moment / Signups | Product analytics | 35% | 42% |
| **Activation** | PQLs from organic | Product-qualified leads from organic signups | Product analytics + CRM | 63/mo | 118/mo |
| **Revenue** | SQLs from organic | Sales-qualified leads sourced from organic | CRM | 25/mo | 40/mo |
| **Revenue** | Pipeline from organic | Dollar value of opportunities from organic | CRM | $250K/mo | $350K/mo |
| **Revenue** | Closed revenue from organic | Closed-won revenue from organic-sourced opps | CRM | $75K/mo | $105K/mo |
| **Retention** | Organic cohort retention | 90-day retention for organic-sourced users | Product analytics | 45% | 50% |

### Tracking implementation checklist

- [ ] GA4 organic source segmentation configured and validated.
- [ ] UTM parameters standardized for all organic landing pages.
- [ ] First-touch attribution field populated in CRM for all new leads.
- [ ] Product signup event fires with `utm_source` and `landing_page` properties.
- [ ] Activation event ("aha moment") defined and instrumented in product analytics.
- [ ] PQL scoring model includes organic source as an input.
- [ ] CRM opportunity object has "original source" and "original landing page" fields.
- [ ] Monthly reporting dashboard built in BI tool (Looker, Metabase, or equivalent).
- [ ] Weekly review cadence established with marketing, sales, and product stakeholders.

### Reporting cadence

| Report | Frequency | Audience | Key metrics |
|---|---|---|---|
| Organic traffic & leads | Weekly | Content team | Sessions, leads, top pages |
| Activation funnel | Weekly | Growth team | Signups, activation rate, PQLs |
| Pipeline & revenue | Monthly | GTM leadership | Pipeline, closed revenue, CAC |
| Full GEO review | Quarterly | Exec team | All metrics, QoQ trends, next-Q plan |

---

## Example 4: Quarterly GTM OKR Set Using SEO + AIO + GEO

This example shows how to structure quarterly OKRs that span all three pillars. Each objective connects to business outcomes, not vanity metrics.

### Q2 2026 GTM OKRs

---

**Objective 1: Increase organic search as a pipeline source**

| Key Result | Metric | Baseline | Target | Owner | Pillar |
|---|---|---|---|---|---|
| KR1: Grow organic sessions to money pages | Sessions to /pricing, /features, /demo | 8,000/mo | 12,000/mo | SEO Lead | SEO |
| KR2: Improve organic lead conversion rate | Leads / organic sessions | 1.0% | 1.3% | Growth Lead | GEO |
| KR3: Increase organic-sourced pipeline | Pipeline $ attributed to organic | $250K/mo | $350K/mo | RevOps | GEO |

**Objective 2: Scale content production with AI-assisted workflows**

| Key Result | Metric | Baseline | Target | Owner | Pillar |
|---|---|---|---|---|---|
| KR1: Publish optimized content pieces | Published pages scoring 80+ on Surfer/Clearscope | 8/mo | 16/mo | Content Lead | AIO |
| KR2: Reduce time from brief to publish | Average calendar days | 14 days | 7 days | Content Lead | AIO |
| KR3: Maintain content quality score | Average optimization score across all new content | 72 | 80 | Content Lead | AIO + SEO |

**Objective 3: Improve post-signup activation for organic users**

| Key Result | Metric | Baseline | Target | Owner | Pillar |
|---|---|---|---|---|---|
| KR1: Increase organic signup-to-activation rate | % of organic signups reaching aha moment | 35% | 42% | Product/Growth | GEO |
| KR2: Launch personalized onboarding for top 5 organic landing pages | Onboarding variants live | 0 | 5 | Growth Lead | GEO + AIO |
| KR3: Improve 30-day retention for organic cohort | 30-day retention rate | 40% | 48% | Product | GEO |

---

### How these OKRs connect

```
Objective 1 (SEO + GEO)          Objective 2 (AIO)              Objective 3 (GEO)
More traffic to money pages  ◄──  More optimized content    ──►  Better activation
Higher lead conversion            Faster production              Higher retention
More pipeline                     Consistent quality             Stronger LTV
         │                               │                              │
         └───────────────────────────────┼──────────────────────────────┘
                                         │
                                  Business outcome:
                            +40% organic-sourced pipeline
                            +20% organic cohort retention
```

### Quarterly review questions

At the end of the quarter, answer these questions to assess the GTM engine:

1. **SEO health:** Did we gain or lose keyword positions for our most important terms? Did organic traffic grow or shrink?
2. **AIO efficiency:** Did AI-assisted workflows increase output without sacrificing quality? Where did humans add the most value?
3. **GEO effectiveness:** Did more organic traffic translate to more pipeline and revenue? Where is the funnel leaking?
4. **Cross-pillar alignment:** Are SEO, AIO, and GEO working as a system, or are they still siloed? What integration opportunities exist for next quarter?
