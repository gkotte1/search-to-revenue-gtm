# Core Frameworks

This document expands on the three core frameworks referenced in the README. Each framework gives GTM teams a mental model for connecting search, AI, and growth into a unified system.

---

## 1. Search-to-Revenue Loop (S2R Loop)

### Overview

The S2R Loop is a five-stage model that maps how a potential customer moves from a search query to revenue, and how SEO, AIO, and GEO each contribute at every stage. Unlike traditional marketing funnels that stop at "lead," the S2R Loop runs all the way to expansion revenue and explicitly identifies where AI and growth engineering accelerate the loop.

### When to use it

- Planning a new GTM motion from scratch.
- Auditing an existing content or growth engine to find bottleneck stages.
- Aligning cross-functional teams (marketing, product, sales, RevOps) on a shared model.

### Diagram (text description)

```
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│ DISCOVER  │───▶│ CAPTURE  │───▶│ ACTIVATE │───▶│ CONVERT  │───▶│  EXPAND  │
│           │    │          │    │          │    │          │    │          │
│ SEO: rank │    │ SEO: CTA │    │ AIO: on- │    │ GEO: sales│    │ GEO: NRR │
│ AIO: draft│    │ GEO: form│    │ boarding  │    │ assist,  │    │ upsell,  │
│ content   │    │ enrich   │    │ sequences │    │ PLG conv │    │ expansion│
└──────────┘    └──────────┘    └──────────┘    └──────────┘    └──────────┘
       ▲                                                              │
       └──────────────────── feedback loop ───────────────────────────┘
```

### Stages

**Discover** — The buyer has a problem and searches for answers.
- SEO: Rank for high-intent queries with the right content type (informational, comparison, solution-aware).
- AIO: Use AI to research keywords, generate briefs, and draft content at scale.
- GEO: Ensure analytics capture the discovery source and intent signal.

**Capture** — The visitor arrives. You need to capture identity or intent.
- SEO: On-page CTAs optimized for the search intent (demo, free tool, gated asset).
- GEO: Forms, chat, and enrichment tools convert anonymous visitors into known leads.
- AIO: AI-personalized CTAs or chat responses based on visitor signals.

**Activate** — The lead or signup takes a meaningful first action.
- GEO: Onboarding flows, product tours, and activation emails.
- AIO: AI-generated onboarding content personalized to the user's stated goal or industry.
- SEO: Help docs and knowledge base content that ranks and supports activation.

**Convert** — The activated user becomes a paying customer.
- GEO: Sales-assist motions, pricing optimization, trial-to-paid conversion flows.
- AIO: AI-generated sales collateral and proposal content.
- SEO: Bottom-of-funnel comparison and alternative pages that influence the decision.

**Expand** — The customer grows in value (upsell, cross-sell, advocacy).
- GEO: Lifecycle marketing, usage-based expansion triggers, NRR optimization.
- AIO: AI-powered customer success content, renewal collateral.
- SEO: Customer-generated content, case study pages, community SEO.

### Feedback loop

Revenue outcomes and customer behavior data feed back into the Discover stage:
- High-converting topics inform keyword strategy.
- Customer language from sales calls shapes content messaging.
- Expansion patterns reveal new content opportunities.

### Example scenario: B2B SaaS (Developer Tools)

A developer tools company uses the S2R Loop:
1. **Discover**: Ranks for "how to debug [framework] in production" with an AI-drafted technical guide.
2. **Capture**: Offers a free debugging tool as a CTA within the guide.
3. **Activate**: Sends an onboarding sequence that walks the developer through their first debugging session.
4. **Convert**: After 3 debugging sessions, triggers a sales-assist motion for the team plan.
5. **Expand**: Monitors usage across the organization and triggers expansion outreach when new team members onboard.

---

## 2. AIO Content Stack

### Overview

The AIO Content Stack describes the six layers of content production where AI can be systematically applied. It replaces the old "writer → editor → publish" model with an AI-augmented pipeline that is faster, more consistent, and measurable.

### When to use it

- Building or restructuring a content operations team.
- Evaluating where to introduce AI tools into existing workflows.
- Diagnosing content pipeline bottlenecks (e.g., "we generate briefs fast but drafts take weeks").

### Diagram (text description)

```
┌─────────────────────────────────────────────────────────────────────┐
│                        AIO CONTENT STACK                            │
│                                                                     │
│  Layer 6: EXPERIMENTATION                                           │
│  ├── A/B test headlines, CTAs, page layouts                         │
│  └── Feed results back into Layer 1                                 │
│                                                                     │
│  Layer 5: DISTRIBUTION                                              │
│  ├── Repurpose: blog → LinkedIn → X → email → video                │
│  └── AI-generated format variations per channel                     │
│                                                                     │
│  Layer 4: OPTIMIZATION                                              │
│  ├── On-page SEO scoring (NLP terms, structure, intent match)       │
│  └── Internal linking and content hub architecture                  │
│                                                                     │
│  Layer 3: DRAFTING                                                  │
│  ├── AI-generated first drafts from briefs                          │
│  └── Human editing for voice, accuracy, and depth                   │
│                                                                     │
│  Layer 2: BRIEFS                                                    │
│  ├── AI-generated outlines with SERP analysis                       │
│  └── Target keywords, questions to answer, competitor gaps           │
│                                                                     │
│  Layer 1: RESEARCH                                                  │
│  ├── Keyword research and clustering                                │
│  ├── Competitor content analysis                                    │
│  └── Customer voice mining (calls, reviews, forums)                 │
└─────────────────────────────────────────────────────────────────────┘
```

### Layer-by-layer usage

**Layer 1: Research**
- Input: Product positioning, ICP definition, seed keywords.
- AI role: Cluster keywords, classify intent, scrape and summarize competitor content, extract themes from customer call transcripts.
- Output: Prioritized topic list with intent classification and estimated traffic potential.

**Layer 2: Briefs**
- Input: Prioritized topic from Layer 1.
- AI role: Generate content brief with target keyword, secondary keywords, recommended headings, questions to answer, word count range, and competitor content summary.
- Output: Content brief ready for a writer (human or AI).

**Layer 3: Drafting**
- Input: Content brief from Layer 2.
- AI role: Generate a complete first draft. Human reviews for accuracy, voice, and subject-matter depth.
- Output: Draft ready for optimization.

**Layer 4: Optimization**
- Input: Draft from Layer 3.
- AI role: Score against SEO optimization targets. Suggest internal links. Check heading structure and keyword coverage.
- Output: Optimized draft ready for publication.

**Layer 5: Distribution**
- Input: Published content from Layer 4.
- AI role: Generate derivative formats — LinkedIn post, Twitter thread, email newsletter excerpt, short-form video script.
- Output: Multi-channel content package.

**Layer 6: Experimentation**
- Input: Performance data from distributed content.
- AI role: Generate headline and CTA variations for A/B testing. Analyze experiment results.
- Output: Winning variations and insights that feed back to Layer 1.

### Example scenario: Healthcare SaaS

A healthcare compliance SaaS company:
1. **Research**: AI clusters 2,000 keywords around "HIPAA compliance" into 30 topic groups.
2. **Briefs**: Generates briefs for the top 10 topics by traffic potential and buying intent.
3. **Drafting**: AI produces first drafts; a compliance SME reviews for regulatory accuracy.
4. **Optimization**: Surfer SEO scores each draft; AI suggests internal links to the product's compliance checklist tool.
5. **Distribution**: Each blog post is repurposed into a LinkedIn carousel and a short email for the newsletter.
6. **Experimentation**: A/B tests on blog CTAs reveal that "Get your free compliance audit" converts 3x better than "Learn more."

---

## 3. GEO Metrics Map

### Overview

The GEO Metrics Map organizes GTM metrics into four stages — Acquisition, Activation, Revenue, and Retention/Expansion — and clarifies which metrics matter at each stage, how to measure them, and which levers (SEO, AIO, GEO) influence each.

### When to use it

- Setting quarterly OKRs for the GTM team.
- Building dashboards and reporting infrastructure.
- Diagnosing where the GTM engine is leaking (e.g., "we get traffic but no signups").

### The map

```
ACQUISITION                 ACTIVATION                  REVENUE                    RETENTION / EXPANSION
─────────────               ──────────                  ───────                    ─────────────────────
Impressions                 Signups                     Opportunities              NRR (Net Revenue Retention)
Sessions                    PQLs (Product-Qualified)    Pipeline value             LTV (Lifetime Value)
Leads (MQLs)                SQLs (Sales-Qualified)      Win rate                   Expansion revenue
                                                        ARR / MRR                  Churn rate
                                                        CAC payback                NPS / CSAT

Primary levers:             Primary levers:             Primary levers:            Primary levers:
├── SEO (rankings, CTR)     ├── GEO (onboarding)        ├── GEO (sales motion)     ├── GEO (lifecycle mktg)
├── AIO (content volume)    ├── AIO (personalization)    ├── AIO (sales content)    ├── AIO (CS content)
└── GEO (channel mix)       └── SEO (help/docs)         └── SEO (BOFU content)     └── SEO (community)
```

### How this repo helps at each stage

**Acquisition**
- SEO pillar: Tools and practices for ranking and earning traffic.
- AIO pillar: Workflows for producing content that ranks at scale.
- Workflows: "From Zero to First 100 ICP Signups via SEO + AIO."

**Activation**
- GEO pillar: Onboarding and product-led growth tools.
- AIO pillar: AI-personalized onboarding content.
- Playbooks: Early-stage and growth-stage activation plays.

**Revenue**
- GEO pillar: CRM, sales enablement, and conversion optimization tools.
- AIO pillar: AI-generated sales collateral and proposal content.
- Frameworks: S2R Loop's Convert stage.

**Retention / Expansion**
- GEO pillar: Lifecycle marketing, customer success, and analytics tools.
- AIO pillar: AI-powered customer communication and renewal content.
- Frameworks: S2R Loop's Expand stage and feedback loop.

### Example scenario: Developer tools startup

A Series A developer tools company sets quarterly OKRs:

| Stage | Metric | Target | Lever |
|---|---|---|---|
| Acquisition | Organic sessions | 50K/mo → 80K/mo | SEO content + AIO drafting |
| Activation | Signup → first project | 30% → 40% | GEO onboarding flow redesign |
| Revenue | Free-to-paid conversion | 5% → 7% | GEO pricing page experiment |
| Retention | Monthly active usage | 60% → 70% | AIO in-product help content |

---

## 4. Signals > Channels > Plays (Optional Model)

### Overview

A lightweight planning model for GTM teams that prefer to think in terms of market signals rather than funnel stages. Start with the signals you observe, choose the channels where those signals are actionable, and run specific plays.

### When to use it

- When the S2R Loop feels too linear for your business.
- When your GTM motion is event-driven or signal-driven (e.g., product-led growth).
- When planning short-term sprints rather than long-term strategy.

### Structure

```
SIGNALS (what you observe)
├── Rising search volume for a category term
├── Competitor launches a new feature
├── Customer churn spike in a segment
├── Product usage milestone reached
└── Seasonal demand pattern

        ▼

CHANNELS (where you act)
├── Organic search (SEO)
├── AI-generated content (AIO)
├── Email / lifecycle (GEO)
├── In-product messaging (GEO)
├── Sales outreach (GEO)
└── Community / social (AIO + SEO)

        ▼

PLAYS (what you do)
├── Publish a SERP-optimized guide on the trending topic
├── Launch a comparison page against the competitor's new feature
├── Trigger a re-engagement campaign for the churning segment
├── Send an expansion email when a usage milestone is hit
└── Publish a seasonal content hub before the demand spike
```

### Example: Signal-driven sprint

**Signal**: Google Trends shows "AI compliance tools" queries up 200% this quarter.

**Channels selected**: Organic search, AI-generated content, email.

**Plays executed**:
1. Use AIO stack to research, brief, draft, and publish 5 articles targeting "AI compliance" keyword cluster.
2. Build a gated "AI Compliance Checklist" as a lead capture asset.
3. Launch an email nurture sequence for leads captured from the checklist.
4. Enrich leads with firmographic data and route enterprise prospects to sales.
5. Measure: impressions → sessions → leads → SQLs → pipeline.
