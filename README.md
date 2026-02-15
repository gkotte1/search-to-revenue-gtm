# Awesome GTM: SEO, AIO & GEO

**The modern GTM playbook at the intersection of search, AI, and growth.**

[![Validate Data Files](https://github.com/search-to-revenue-gtm/search-to-revenue-gtm/actions/workflows/validate-data.yml/badge.svg)](https://github.com/search-to-revenue-gtm/search-to-revenue-gtm/actions/workflows/validate-data.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## Why This Repo Exists

Traditional "awesome SEO" lists are long catalogs of tools and links organized by SEO subcategory. They are useful for SEO specialists but miss the point for GTM teams. If you run go-to-market at a startup or growth-stage company, your problem is not "find an SEO tool." Your problem is "build a system that turns search visibility into pipeline and revenue." That requires more than SEO.

AI has fundamentally changed the GTM landscape. Content production, keyword research, competitor analysis, and even sales enablement are now AI-augmented workflows, not manual tasks. The teams that treat AI as a first-class pillar of their GTM stack — not just "a tool we use sometimes" — are producing more, moving faster, and compounding their advantages. A modern GTM reference must account for this.

Meanwhile, most SEO resources stop at traffic. They measure rankings, impressions, and sessions, then declare victory. GTM teams need to go further: How does this traffic activate? How does it convert to pipeline? What is the LTV of an organic-sourced customer? This is what we call Growth Engine Optimization (GEO) — connecting every acquisition effort to revenue outcomes.

This repo exists to give GTM leaders, founders, and technical marketers a unified, opinionated reference that covers all three pillars. Use it to build strategy, choose tools, design workflows, and set OKRs that tie search and AI investment to business results.

---

## Table of Contents

- [Core Frameworks](#core-frameworks)
- [Pillar 1: SEO (Search Engine Optimization)](#pillar-1-seo-search-engine-optimization)
- [Pillar 2: AIO (AI Optimization)](#pillar-2-aio-ai-optimization)
- [Pillar 3: GEO (Growth Engine Optimization)](#pillar-3-geo-growth-engine-optimization)
- [End-to-End GTM Workflows](#end-to-end-gtm-workflows)
- [Playbooks by Stage](#playbooks-by-stage)
- [Data Files (Tools and Resources)](#data-files)
- [About This Project](#about-this-project)
- [Contributing](#contributing)
- [License](#license)

---

## Core Frameworks

These three frameworks form the conceptual backbone of the repo. Summaries are below; detailed versions with step-by-step usage and examples are in [docs/frameworks.md](docs/frameworks.md).

### 1. Search-to-Revenue Loop (S2R Loop)

A five-stage model mapping how a buyer moves from search query to revenue — and how SEO, AIO, and GEO each contribute at every stage.

| Stage | What happens | SEO role | AIO role | GEO role |
|---|---|---|---|---|
| **Discover** | Buyer searches for a solution | Rank for intent-matched queries | Draft and optimize content at scale | Track discovery source and intent |
| **Capture** | Visitor arrives, identity is captured | On-page CTAs aligned to intent | AI-personalized chat or CTAs | Forms, enrichment, lead capture |
| **Activate** | Lead takes a meaningful first action | Help docs and knowledge base | AI-generated onboarding content | Onboarding flows and product tours |
| **Convert** | User becomes a paying customer | BOFU comparison and alternative pages | AI-generated sales collateral | Sales-assist, pricing optimization |
| **Expand** | Customer grows in value | Case studies, community content | AI-powered CS content | Lifecycle marketing, NRR optimization |

The loop feeds back: revenue data and customer language inform keyword strategy and content.

### 2. AIO Content Stack

Six layers of content production where AI can be systematically applied:

1. **Research** — Keyword clustering, competitor analysis, customer voice mining.
2. **Briefs** — AI-generated outlines with SERP analysis, target keywords, and competitor gaps.
3. **Drafting** — AI first drafts, human editing for accuracy and voice.
4. **Optimization** — On-page SEO scoring, internal linking, heading structure.
5. **Distribution** — AI-generated format variations (blog → LinkedIn → X → email → video).
6. **Experimentation** — A/B test headlines and CTAs, feed results back to Layer 1.

### 3. GEO Metrics Map

Organizes GTM metrics into four stages and maps the levers that influence each:

| Stage | Key metrics | Primary levers |
|---|---|---|
| **Acquisition** | Impressions, sessions, leads | SEO (rankings), AIO (content volume), GEO (channel mix) |
| **Activation** | Signups, PQLs, SQLs | GEO (onboarding), AIO (personalization), SEO (help content) |
| **Revenue** | Opportunities, pipeline, ARR | GEO (sales motion), AIO (sales content), SEO (BOFU pages) |
| **Retention/Expansion** | NRR, LTV, churn rate | GEO (lifecycle marketing), AIO (CS content), SEO (community) |

---

## Pillar 1: SEO (Search Engine Optimization)

In GTM context, SEO is the discipline of making your product discoverable when buyers search for solutions to the problems you solve. It goes beyond rankings — modern GTM-focused SEO connects search visibility to pipeline and revenue.

### What GTM teams need from SEO

- **Technical foundations**: Indexability, site performance, structured data. A fast, crawlable site is the baseline, not the strategy.
- **Search intent mapping to pipeline**: Every target keyword should map to a funnel stage. "What is X" is TOFU. "Best X tools" is MOFU. "X vs Y" is BOFU. Your content strategy should reflect this.
- **Programmatic and AI-assisted content**: For companies with many use cases, integrations, or market segments, programmatic page generation (backed by AI) enables search coverage that manual content cannot achieve.
- **Search + brand + demand creation**: SEO is not just about capturing existing demand. Ranking for category-defining content creates demand and shapes how the market thinks about the problem space.

### High-signal moves

- Map your entire keyword universe to funnel stages and track conversion rate by stage, not just traffic.
- Build content hubs (pillar + cluster) around each product use case to establish topical authority.
- Optimize for search intent first, keywords second. A page that matches intent but misses exact-match keywords will outperform the reverse.
- Invest in technical SEO as a growth multiplier — fixing indexation and performance issues often unlocks gains from existing content.
- Track share-of-search (your branded + non-branded visibility vs. competitors) as a leading indicator of market position.

### High-signal SEO tools

A curated selection — see [data/tools-seo.json](data/tools-seo.json) for the full list with structured metadata.

| Tool | What GTM teams use it for |
|---|---|
| [Ahrefs](https://ahrefs.com) | Keyword research, competitor gap analysis, backlink monitoring |
| [Google Search Console](https://search.google.com/search-console) | First-party search performance data, indexation monitoring |
| [Screaming Frog](https://www.screamingfrog.co.uk/seo-spider/) | Technical site audits, crawl analysis |
| [Surfer SEO](https://surferseo.com) | On-page content optimization scoring |
| [Keyword Insights](https://www.keywordinsights.ai) | AI-powered keyword clustering and intent classification |
| [Google Trends](https://trends.google.com) | Search demand validation and seasonal planning |

---

## Pillar 2: AIO (AI Optimization)

AIO is the discipline of building repeatable, AI-augmented workflows for every stage of GTM content and operations. It is not "use ChatGPT sometimes." It is systematically integrating AI into your GTM engine so that content production, research, and optimization are faster, more consistent, and scalable.

### What AIO covers

- **Keyword research**: AI-assisted keyword expansion, clustering, and intent classification.
- **Content briefs**: AI-generated outlines with SERP analysis, competitor gaps, and target structures.
- **Drafting and rewriting**: AI first drafts with human editing for voice, accuracy, and depth.
- **Internal linking plans**: AI analysis of site structure to recommend link placements.
- **SERP and competitor analysis**: AI-summarized competitor content, positioning gaps, and messaging patterns.
- **Content repurposing**: Transforming one piece of content into multiple formats (blog → LinkedIn → X → email → video script).

### AIO workflows

- **Keyword-to-cluster pipeline**: Feed seed keywords into AI → expand to 100+ queries → cluster by topic and intent → prioritize by buying signal and difficulty.
- **Brief generation**: Input target keyword + competitor URLs → AI generates outline, questions to answer, word count range, and internal linking suggestions.
- **Draft-and-optimize loop**: AI drafts from brief → human edits for accuracy → content optimization tool scores → AI rewrites weak sections → final human review.
- **Repurposing engine**: Published blog post → AI generates LinkedIn post, X thread, email excerpt, and short video script in one session.
- **Competitor monitoring**: Weekly AI scan of competitor blogs and changelogs → summarized report of new positioning, features, and content themes.

### AI-native tools

A curated selection — see [data/tools-aio.json](data/tools-aio.json) for the full list with structured metadata.

| Tool | What GTM teams use it for |
|---|---|
| [Claude](https://claude.ai) | Content briefs, drafting, analysis, and multi-step reasoning |
| [Jasper](https://www.jasper.ai) | Scaled content production with brand voice controls |
| [Frase](https://www.frase.io) | SERP research + content brief + AI writing in one tool |
| [Descript](https://www.descript.com) | Video/audio editing and content repurposing |
| [Zapier](https://zapier.com) | No-code automation connecting content workflows |
| [n8n](https://n8n.io) | Open-source AI workflow automation for technical teams |

---

## Pillar 3: GEO (Growth Engine Optimization)

GEO is the discipline of optimizing the entire GTM engine — not just top-of-funnel acquisition, but the full path from first touch to expansion revenue. While SEO brings visitors and AIO scales content, GEO connects everything to activation, conversion, retention, and revenue.

### What GEO covers

- **Onboarding and activation**: Getting new signups to their first value moment. The best SEO traffic is wasted if users sign up and never activate.
- **Product-led growth (PLG) loops**: Self-serve conversion, viral mechanics, and usage-based expansion.
- **Sales-assist motions**: Routing high-intent leads from content to sales, with the right context and timing.
- **Lifecycle marketing**: Behavior-triggered email, in-app messaging, and re-engagement campaigns tied to product events.
- **Revenue attribution**: Connecting content and traffic data to pipeline and closed revenue. Without this, you cannot optimize the GTM engine.
- **Experimentation**: A/B testing landing pages, onboarding flows, pricing pages, and CTAs to improve conversion at every stage.

### Key GEO levers

- **Onboarding flow optimization**: Personalize onboarding based on acquisition source and stated goal. Organic visitors have different intent than paid or referral users.
- **Activation metric definition**: Define and instrument the "aha moment" — the action that predicts retention and conversion. Optimize everything upstream toward this moment.
- **PLG conversion mechanics**: Free-to-paid triggers, usage limits, team expansion prompts. Design these to be natural, not punitive.
- **Sales-assist routing**: Use enrichment and scoring to identify which organic leads should get a sales touch and which should stay in self-serve.
- **Lifecycle campaigns**: Build event-driven email and in-app message sequences tied to product behavior, not just time delays.
- **Full-funnel dashboards**: Track from impression to revenue in one view. Segment by channel. Calculate unit economics by acquisition source.

### Growth tools

A curated selection — see [data/tools-geo.json](data/tools-geo.json) for the full list with structured metadata.

| Tool | What GTM teams use it for |
|---|---|
| [HubSpot](https://www.hubspot.com) | CRM, marketing automation, lead nurturing, attribution |
| [Mixpanel](https://mixpanel.com) | Product analytics, activation funnels, retention analysis |
| [PostHog](https://posthog.com) | Product analytics, feature flags, session recordings, experiments |
| [Segment](https://segment.com) | Customer data infrastructure, identity resolution |
| [Mutiny](https://www.mutinyhq.com) | B2B website personalization for organic visitors |
| [Customer.io](https://customer.io) | Event-driven lifecycle marketing automation |

---

## End-to-End GTM Workflows

These workflows span all three pillars. Each one is summarized here; detailed step-by-step versions are in [docs/workflows.md](docs/workflows.md).

### 1. From Zero to First 100 ICP Signups via SEO + AIO

**Goal:** An early-stage company with no organic traffic publishes its first 10 SEO-optimized pages and generates 100 ICP-fit signups within 90 days.

**Inputs:** ICP definition, product positioning, AI writing tool, CMS, analytics.

**Key steps:**
1. Define 3-5 seed topics tied to product use cases.
2. Use AI to expand into 50-100 keywords, cluster by intent.
3. Prioritize 10 pages by buying intent and difficulty.
4. Generate briefs with AI, draft with AI, edit with human judgment.
5. Optimize for on-page SEO, add conversion CTAs.
6. Publish, distribute, and track impressions → signups weekly.

**Outputs:** 10 published pages, conversion tracking, a data-informed plan for the next sprint.

### 2. Upgrade Legacy Blog to AI-Optimized Revenue Engine

**Goal:** Transform an existing 50-200 post blog with low conversion into a measurable pipeline contributor.

**Inputs:** Existing blog content, Search Console data, content optimization tool, CRM.

**Key steps:**
1. Export and categorize all existing posts by funnel stage and conversion potential.
2. Identify quick wins: posts ranking positions 4-20 with decent impressions.
3. Use AI to audit and rewrite the top 10 quick-win posts.
4. Add conversion CTAs, consolidate thin content, build hub structure.
5. Set up attribution tracking from blog to pipeline.

**Outputs:** 10+ refreshed posts with conversion paths, content hub architecture, attribution baseline.

### 3. GTM for New Feature Launch Powered by AI Content

**Goal:** Generate awareness, capture demand, and activate users around a new feature using AI-powered content within a 2-4 week timeline.

**Inputs:** Product brief/PRD, target audience segment, AI tools.

**Key steps:**
1. Extract core narrative from the product brief using AI.
2. Research the search landscape for the feature's problem space.
3. Use AI to draft a landing page, tutorial blog post, comparison page, and release note.
4. Optimize for SEO, set up feature-specific conversion tracking.
5. Build email sequence for existing users, create social distribution assets.

**Outputs:** Feature landing page, supporting content, email sequence, distribution package, tracking dashboard.

### 4. Product Notes to SEO + AIO + GEO Launch Plan

**Goal:** Turn rough product/feature notes into a complete GTM launch plan covering search, AI content, and growth.

**Inputs:** Raw product notes, ICP definition, current GTM metrics.

**Key steps:**
1. Feed raw notes to AI to extract feature summary, audience, and differentiation.
2. Generate keyword research and map to funnel stages.
3. Define content plan, GEO motion (PLG vs. sales-assist), and activation sequence.
4. Draft measurement plan with metrics, tools, and targets per S2R stage.
5. Build timeline with weekly milestones and assigned owners.

**Outputs:** Complete GTM launch plan document, content calendar, measurement plan, timeline.

### 5. Quarterly SEO + AIO + GEO Performance Review

**Goal:** Assess GTM engine performance across all three pillars, identify wins and gaps, and set priorities for the next quarter.

**Inputs:** Search Console data, product analytics, CRM pipeline data, content production log.

**Key steps:**
1. Pull acquisition, activation, and revenue metrics for organic channel.
2. Rank all content by traffic, conversion rate, and pipeline contribution.
3. Review AIO efficiency (production velocity, AI-to-human ratio).
4. Assess GEO funnel health and identify the biggest bottleneck.
5. Use AI to generate insights and draft next-quarter priorities.

**Outputs:** Quarterly performance report, content performance rankings, next-quarter priorities.

---

## Playbooks by Stage

Detailed playbooks are in [docs/playbooks.md](docs/playbooks.md). Below is a summary by stage.

### Early Stage (0 → 1 GTM)

You have a product and early traction but no scalable acquisition engine. Resources are limited. Every initiative must be high-leverage.

**Recommended plays:**

- **SEO-driven founder-led narrative**: Use the founder's unique market insight as the content differentiator. Write 5 thesis-driven posts that rank for high-intent queries and establish the company's point of view.
- **AIO-powered content sprint**: Use AI to publish 20-30 SEO-optimized pages in 30 days, covering the primary keyword universe for your product's use cases.
- **Minimum viable measurement**: Set up basic tracking (Search Console + analytics + CRM) to measure organic → signup → activation before investing in more content.

### Growth Stage (1 → N)

You have organic traffic and some pipeline, but content ROI is hard to prove, activation is inconsistent, and scaling content quality is a challenge.

**Recommended plays:**

- **Content-to-pipeline attribution engine**: Build a system that connects every content piece to leads, pipeline, and revenue. Use this data to drive the editorial calendar.
- **PLG + SEO flywheel**: Create a self-reinforcing loop where SEO content drives signups, product usage creates content signals, and those signals improve SEO.
- **AIO content ops scaling**: Implement the AIO Content Stack to double content production velocity without doubling headcount.

### Enterprise / Multi-Product

You have multiple product lines, large content footprints, and cross-team coordination challenges. The risk is cannibalization, duplication, and misaligned investment.

**Recommended plays:**

- **Multi-product SEO architecture**: Design keyword ownership rules, content hub structures, and governance processes that prevent internal competition for search visibility.
- **RevOps + GEO instrumentation baseline**: Build full-funnel instrumentation connecting marketing, product, and revenue data into a unified measurement system.
- **AI-powered content governance**: Use AI to monitor content quality, keyword cannibalization, and messaging consistency across product lines.

---

## Data Files

The `/data` directory contains structured metadata for tools across all three pillars:

| File | Contents |
|---|---|
| [data/tools-seo.json](data/tools-seo.json) | SEO tools (keyword research, technical SEO, content optimization, analytics) |
| [data/tools-aio.json](data/tools-aio.json) | AI/AIO tools (AI assistants, content platforms, automation, research) |
| [data/tools-geo.json](data/tools-geo.json) | GEO/Growth tools (analytics, CRM, experimentation, lifecycle marketing) |

### Shared schema

Every tool entry follows the same structure, designed for GTM decision-making:

```json
{
  "name": "Tool Name",
  "website": "https://example.com",
  "category": "short-tag",
  "summary": "1-2 sentence practical description for GTM teams.",
  "gtm_use_cases": [
    "Primary GTM use case 1",
    "Primary GTM use case 2"
  ],
  "pricing_model": "free | freemium | paid",
  "best_for_stage": [
    "early",
    "growth",
    "enterprise"
  ]
}
```

- **`summary`**: Describes what a GTM team actually gets from this tool. No hype.
- **`gtm_use_cases`**: Concrete actions a GTM team would take with this tool.
- **`pricing_model`**: Helps teams filter by budget constraints (`free`, `freemium`, `paid`).
- **`best_for_stage`**: Helps teams filter by company stage (`early`, `growth`, `enterprise`).

---

## About This Project

This repo is a living GTM reference. It is designed for teams who want to operationalize SEO + AIO + GEO — not just learn definitions, but build systems that work.

It is intentionally opinionated. The frameworks, workflows, and playbooks reflect how high-performing GTM teams actually operate, not how marketing textbooks say they should. Where there are trade-offs, we state them. Where there are anti-patterns, we call them out.

This is not:
- A comprehensive directory of every marketing tool that exists.
- An SEO-only resource.
- A theoretical academic reference.
- A vendor pitch.

This is:
- A practical guide for building a GTM engine that uses search, AI, and growth engineering as interconnected systems.
- A reference for choosing the right tools, workflows, and plays for your stage and context.
- A community resource that gets better as practitioners contribute their experience.

Contributions from GTM leaders, founders, and technical marketers are welcome. See below.

---

## Contributing

We welcome contributions that make this resource more useful for GTM practitioners. See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines.

**Types of contributions:**

- **Tools**: Add a new tool to the relevant JSON file with proper GTM use cases.
- **Frameworks**: Propose a new framework or improve an existing one.
- **Workflows**: Document an end-to-end GTM workflow that spans pillars.
- **Playbooks**: Add a stage-specific playbook with real-world applicability.
- **Examples**: Contribute concrete examples (content briefs, measurement plans, OKR sets).

**Requirements for new tool entries:**
- Must include specific GTM use cases (not just "it's a good tool").
- Must follow the shared schema.
- No affiliate links. No self-promotion without substance.

**Quality bar:**
- Practical over theoretical.
- Specific over generic.
- GTM outcome-focused, not feature-list-focused.

---

## License

This project is licensed under the [MIT License](LICENSE).
