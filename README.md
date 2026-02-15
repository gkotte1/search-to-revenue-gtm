# Awesome GTM: SEO, AIO & GEO

**The modern GTM playbook at the intersection of search, AI, and growth.**

[![Validate Data Files](https://github.com/gkotte1/search-to-revenue-gtm/actions/workflows/validate-data.yml/badge.svg)](https://github.com/gkotte1/search-to-revenue-gtm/actions/workflows/validate-data.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## Why This Repo Exists

Traditional "awesome SEO" lists are long catalogs of tools and links organized by SEO subcategory. They are useful for SEO specialists but miss the point for GTM teams. If you run go-to-market at a startup or growth-stage company, your problem is not "find an SEO tool." Your problem is "build a system that turns search visibility into pipeline and revenue." That requires more than SEO. It requires a unified system that connects search, AI-powered content operations, and revenue-focused growth engineering into a single coherent engine.

AI has fundamentally changed the GTM landscape. Content production, keyword research, competitor analysis, and even sales enablement are now AI-augmented workflows, not manual tasks. The teams that treat AI as a first-class pillar of their GTM stack (not just "a tool we use sometimes") are producing more, moving faster, and compounding their advantages quarter over quarter. A modern GTM reference must account for this shift. It must provide concrete guidance on how to integrate AI into every stage of the content and growth pipeline, from initial keyword research all the way through to post-sale expansion content.

Meanwhile, most SEO resources stop at traffic. They measure rankings, impressions, and sessions, then declare victory. GTM teams need to go further: How does this traffic activate? How does it convert to pipeline? What is the LTV of an organic-sourced customer? How do you attribute closed-won revenue back to the blog post that started the journey? This is what we call Growth Engine Optimization (GEO), which means connecting every acquisition effort to revenue outcomes through instrumentation, experimentation, and full-funnel measurement.

This repo exists to give GTM leaders, founders, and technical marketers a unified, opinionated reference that covers all three pillars. Use it to build strategy, choose tools, design workflows, and set OKRs that tie search and AI investment to business results. Whether you are a solo founder trying to get your first 100 signups from organic search or a growth-stage VP of Marketing trying to prove content ROI to the board, this reference is designed to help you move from theory to execution.

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

These three frameworks form the conceptual backbone of the repo. They give you a shared mental model for how search, AI, and growth engineering work together to drive revenue. Summaries are below; detailed versions with step-by-step usage and examples are in [docs/frameworks.md](docs/frameworks.md).

### 1. Search-to-Revenue Loop (S2R Loop)

A five-stage model mapping how a buyer moves from search query to revenue, and how SEO, AIO, and GEO each contribute at every stage. The S2R Loop is the foundational concept of this entire repo. It reframes SEO as just the first stage of a longer revenue journey, rather than an end in itself. By understanding all five stages, you can identify which stage is your current bottleneck and allocate resources accordingly.

| Stage | What happens | SEO role | AIO role | GEO role |
|---|---|---|---|---|
| **Discover** | Buyer searches for a solution to a problem they have identified. They may use Google, Bing, or an AI assistant. The goal is to become visible at this moment of intent. | Rank for intent-matched queries across informational, navigational, and transactional search types. Build topical authority so your domain surfaces consistently. | Draft and optimize content at scale using AI to cover a broader keyword universe than manual writing allows. Use AI to identify content gaps and generate first drafts rapidly. | Track discovery source and intent category so you know which search queries and channels produce the highest-quality visitors downstream. |
| **Capture** | Visitor arrives on your site and their identity is captured through a form, signup, or enrichment tool. This is where anonymous traffic becomes a known lead. | On-page CTAs aligned to the visitor's search intent. A visitor reading a comparison post should see a different CTA than one reading an educational guide. | AI-personalized chat, dynamic CTAs, or interactive tools that adapt based on the visitor's behavior and inferred intent. AI can tailor the conversion experience in real time. | Forms, progressive profiling, enrichment via tools like Clearbit or Apollo, and lead capture mechanisms that feed directly into your CRM with full attribution data attached. |
| **Activate** | Lead takes a meaningful first action inside your product or with your team. This is the "aha moment" where they experience initial value. Without activation, captured leads decay rapidly. | Help docs, knowledge base articles, and getting-started guides that reduce friction during onboarding. SEO ensures these resources are discoverable both internally and externally. | AI-generated onboarding content, personalized walkthroughs, and contextual help that adapts to the user's role, use case, and progress within the product. | Onboarding flows, product tours, and activation sequences designed to get users to the key value action as quickly as possible. Instrument and measure activation rate by cohort. |
| **Convert** | User becomes a paying customer. This stage covers the entire decision-making process from "I see the value" to "I have entered my credit card" or "I have signed the contract." | BOFU comparison pages, alternative pages (e.g., "Your Product vs. Competitor"), pricing pages, and case studies that rank in search and support the buying decision. | AI-generated sales collateral, personalized proposals, ROI calculators, and battle cards that help the sales team (or the self-serve flow) close the deal faster. | Sales-assist routing, pricing optimization, free-to-paid conversion triggers, and experimentation on the conversion flow itself. Measure conversion rate by acquisition source. |
| **Expand** | Customer grows in value over time through upsells, cross-sells, seat expansion, and advocacy. This is where compounding returns on your GTM investment are realized. | Case studies, community content, advanced guides, and thought leadership that keep customers engaged and attract new prospects through the success stories of existing ones. | AI-powered customer success content, automated QBR preparation, personalized feature adoption recommendations, and AI-generated training materials for new use cases. | Lifecycle marketing campaigns, NRR optimization, expansion revenue tracking, and referral program management. Measure LTV by original acquisition channel to close the loop. |

The loop feeds back: revenue data, customer language, support ticket themes, and expansion patterns all inform keyword strategy, content priorities, and messaging. This feedback loop is what makes the system compound over time rather than plateau.

### 2. AIO Content Stack

Six layers of content production where AI can be systematically applied. The key insight is that AI should not be used as a single-point tool (e.g., "write me a blog post"). Instead, it should be embedded at every layer of the content pipeline, with each layer feeding the next. This creates a repeatable, scalable system rather than ad-hoc AI usage.

1. **Research**: Use AI to perform keyword clustering, competitor content analysis, SERP feature identification, and customer voice mining from reviews, forums, and support tickets. The goal is to build a comprehensive map of the topics, questions, and language patterns that your target audience uses. AI dramatically accelerates this process by synthesizing large volumes of data that would take a human analyst days or weeks to process manually.

2. **Briefs**: Generate detailed content outlines using AI that incorporate SERP analysis (what currently ranks and why), target keywords and their variants, competitor gaps (what existing content misses), recommended word count, heading structure, and internal linking opportunities. A strong brief is the single biggest lever for content quality. AI-generated briefs ensure consistency and thoroughness across your entire content operation.

3. **Drafting**: AI produces first drafts based on the approved brief. Human editors then refine for accuracy, brand voice, original insight, and depth. The AI-to-human handoff is critical. AI handles volume and structure; humans add expertise, nuance, and the unique perspective that builds trust with readers. Never publish AI drafts without substantive human editing.

4. **Optimization**: Run completed drafts through on-page SEO scoring tools to check keyword usage, heading structure, internal linking, readability, and content completeness. AI can suggest specific improvements, rewrite underperforming sections, and ensure that every page meets a consistent quality bar before publication. This layer is where you catch gaps that manual review often misses.

5. **Distribution**: Use AI to transform a single published piece into multiple format variations (blog → LinkedIn → X → email → video). This multiplies the reach of every piece of content without requiring separate creative processes for each channel. AI handles the format adaptation while preserving the core message.

6. **Experimentation**: A/B test headlines, meta descriptions, CTAs, and content structures. Feed the performance results back to Layer 1 (Research) to continuously refine your understanding of what resonates with your audience. This closes the loop and ensures your content operation improves with every cycle. AI can analyze test results and recommend next experiments automatically.

### 3. GEO Metrics Map

Organizes GTM metrics into four stages and maps the levers that influence each. The purpose of this framework is to give GTM teams a single-page view of how their metrics connect across the funnel. Too many teams optimize acquisition metrics (traffic, rankings) in isolation from revenue metrics (pipeline, ARR). The GEO Metrics Map forces alignment by making the connections explicit and ensuring every team member understands which levers affect which outcomes.

| Stage | Key metrics | Primary levers |
|---|---|---|
| **Acquisition** | Impressions, sessions, new visitors, branded vs. non-branded traffic split, cost per session by channel | SEO (rankings and topical authority), AIO (content volume and quality at scale), GEO (channel mix optimization and budget allocation) |
| **Activation** | Signups, product-qualified leads (PQLs), sales-qualified leads (SQLs), activation rate, time-to-first-value | GEO (onboarding flow design and optimization), AIO (personalized onboarding content), SEO (help content and knowledge base discoverability) |
| **Revenue** | Opportunities created, pipeline value, win rate, average contract value, ARR, time-to-close | GEO (sales motion design and pricing optimization), AIO (AI-generated sales collateral and proposals), SEO (BOFU pages that support buying decisions) |
| **Retention/Expansion** | Net revenue retention (NRR), customer lifetime value (LTV), churn rate, expansion revenue, referral rate | GEO (lifecycle marketing and customer success programs), AIO (AI-powered CS content and automated engagement), SEO (community content and advanced guides that deepen product adoption) |

---

## Pillar 1: SEO (Search Engine Optimization)

In GTM context, SEO is the discipline of making your product discoverable when buyers search for solutions to the problems you solve. It goes beyond rankings. Modern GTM-focused SEO connects search visibility to pipeline and revenue by treating every piece of content as a node in a conversion system, not just a traffic generator.

### What GTM teams need from SEO

- **Technical foundations**: Indexability, site performance, structured data, mobile optimization, and Core Web Vitals. A fast, crawlable site is the baseline, not the strategy. If search engines cannot efficiently crawl and index your pages, nothing else matters. Conduct regular technical audits (monthly at minimum) and treat technical SEO debt the same way engineering treats code debt: as a blocker that compounds if ignored. Common issues include orphaned pages, slow server response times, broken canonical tags, and missing structured data markup.

- **Search intent mapping to pipeline**: Every target keyword should map to a funnel stage. "What is X" is TOFU (top of funnel). "Best X tools" is MOFU (middle of funnel). "X vs Y" is BOFU (bottom of funnel). Your content strategy should reflect this distribution. Most teams over-invest in TOFU content because it generates the most traffic, but BOFU content often has 5-10x higher conversion rates. Build a keyword-to-funnel-stage spreadsheet and review it quarterly to ensure your content production matches your pipeline needs, not just your traffic goals.

- **Programmatic and AI-assisted content**: For companies with many use cases, integrations, or market segments, programmatic page generation (backed by AI) enables search coverage that manual content cannot achieve. For example, a SaaS product with 50 integrations can generate 50 integration-specific landing pages, each optimized for "[Product] + [Integration]" search queries. AI writes the initial drafts, humans review and customize, and the result is broad search coverage that would take months to produce manually. This approach is especially powerful for companies targeting long-tail keywords across many verticals or geographies.

- **Search + brand + demand creation**: SEO is not just about capturing existing demand. Ranking for category-defining content creates demand and shapes how the market thinks about the problem space. When you publish authoritative content that defines a new category or reframes an existing problem, you influence the vocabulary buyers use in future searches. This creates a compounding advantage: you define the terms, then you rank for them. Invest in thought leadership content that goes beyond keyword targeting to establish your company as the intellectual leader in your space.

### High-signal moves

- Map your entire keyword universe to funnel stages and track conversion rate by stage, not just traffic. This means building a spreadsheet or dashboard that shows, for every content cluster, the traffic volume, conversion rate to signup, activation rate, and pipeline contribution. When you can see that your BOFU cluster converts at 8% while your TOFU cluster converts at 0.3%, resource allocation decisions become obvious.

- Build content hubs (pillar + cluster) around each product use case to establish topical authority. A content hub consists of one comprehensive pillar page (2,000-5,000 words covering the broad topic) surrounded by 10-20 cluster pages that address specific subtopics in depth. Internal links connect cluster pages to the pillar and to each other. This structure signals to search engines that your site has comprehensive expertise on the topic, which lifts rankings across the entire cluster.

- Optimize for search intent first, keywords second. A page that matches intent but misses exact-match keywords will outperform the reverse. Before writing any page, search the target keyword yourself and study the top 5 results. What format do they use? What questions do they answer? What depth do they provide? Match or exceed the intent satisfaction of the current top results, then layer in keyword optimization. Intent mismatch is the number-one reason good content fails to rank.

- Invest in technical SEO as a growth multiplier. Fixing indexation and performance issues often unlocks gains from existing content without requiring any new content production. Common high-impact fixes include improving page speed (especially Largest Contentful Paint), resolving duplicate content issues, fixing internal link architecture to distribute PageRank effectively, and implementing proper hreflang tags for international sites. A single technical SEO audit can sometimes unlock more organic traffic growth than an entire quarter of new content.

- Track share-of-search (your branded + non-branded visibility vs. competitors) as a leading indicator of market position. Share-of-search correlates strongly with market share and is measurable months before revenue data reflects changes. Calculate it by summing your search visibility scores across your target keyword set and comparing against competitors. Track this monthly and use it as a board-level metric alongside pipeline and revenue.

### High-signal SEO tools

A curated selection of the most impactful tools for GTM-focused SEO teams. See [data/tools-seo.json](data/tools-seo.json) for the full list with structured metadata, including pricing models, best-for-stage recommendations, and specific GTM use cases.

| Tool | What GTM teams use it for |
|---|---|
| [PostWyse](https://postwyse.com) | AI-powered content and SEO management that combines keyword research, content creation, and social distribution in one workflow. Helps GTM teams go from keyword research to published, optimized content across search and social channels, identify high-intent opportunities, and track which topics drive the most pipeline. |
| [Google Search Console](https://search.google.com/search-console) | First-party search performance data (impressions, clicks, CTR, position) directly from Google, indexation monitoring to catch crawl errors early, Core Web Vitals tracking, and manual action notifications. This is your most reliable source of search data because it comes directly from the search engine. |
| [Screaming Frog](https://www.screamingfrog.co.uk/seo-spider/) | Technical site audits that crawl your entire site to identify broken links, duplicate content, missing meta tags, redirect chains, and structural issues. Essential for quarterly technical SEO health checks and for auditing sites before and after migrations. |
| [Surfer SEO](https://surferseo.com) | On-page content optimization scoring that compares your draft against the top-ranking pages for your target keyword. Provides specific recommendations for word count, keyword density, heading structure, and NLP-relevant terms to include. Useful for both new content and content refreshes. |
| [Keyword Insights](https://www.keywordinsights.ai) | AI-powered keyword clustering that groups thousands of keywords by topic and intent, and intent classification that tells you whether a keyword requires an informational, commercial, or transactional page. This saves hours of manual keyword analysis and ensures your content plan covers topics efficiently without cannibalization. |
| [Google Trends](https://trends.google.com) | Search demand validation to confirm that a keyword has real and growing search volume before investing in content. Seasonal planning to time content publication for peak demand periods. Competitive comparison to see how interest in your brand compares to competitors over time. |

---

## Pillar 2: AIO (AI Optimization)

AIO is the discipline of building repeatable, AI-augmented workflows for every stage of GTM content and operations. It is not "use ChatGPT sometimes." It is systematically integrating AI into your GTM engine so that content production, research, and optimization are faster, more consistent, and scalable. The teams that build robust AIO systems gain a structural advantage: they can produce more high-quality content, respond faster to market changes, and maintain consistency across a larger content footprint than teams relying on purely manual processes.

### What AIO covers

- **Keyword research**: AI-assisted keyword expansion, clustering, and intent classification. Start with 5-10 seed keywords and use AI to expand them into hundreds of related queries, grouped by topic cluster and search intent. AI can also analyze your existing Search Console data to find keyword opportunities you are currently missing, identify patterns in search queries that suggest new content categories, and classify every keyword by its position in the buying journey.

- **Content briefs**: AI-generated outlines with SERP analysis, competitor gaps, and target structures. A good content brief includes the target keyword and secondary keywords, a recommended outline with H2 and H3 headings, questions the content must answer (pulled from People Also Ask and forums), a competitive analysis summary showing what top-ranking pages cover, word count guidance, and internal linking recommendations. AI can produce these briefs in minutes rather than the hours a human researcher would need.

- **Drafting and rewriting**: AI first drafts with human editing for voice, accuracy, and depth. The workflow is: AI generates a complete first draft following the brief, then a human editor rewrites for brand voice, adds original examples and data points, fact-checks all claims, and ensures the content offers unique value beyond what AI alone can produce. This hybrid approach typically reduces content production time by 40-60% while maintaining or improving quality, as long as the human editing step is rigorous and not superficial.

- **Internal linking plans**: AI analysis of site structure to recommend link placements that strengthen topical authority and distribute PageRank effectively. Feed AI your sitemap and content inventory, and it can identify orphaned pages (pages with no internal links pointing to them), suggest contextual link placements within existing content, and map out hub-and-spoke linking patterns for your content clusters. Strong internal linking is one of the most underutilized SEO levers, and AI makes it practical to maintain even on large sites.

- **SERP and competitor analysis**: AI-summarized competitor content, positioning gaps, and messaging patterns. Instead of manually reading 20 competitor blog posts, feed them to AI and get a structured summary of their messaging themes, feature emphasis, target audience language, and content gaps. This analysis can inform both your content strategy and your product positioning. Run this monthly to stay current with how competitors are evolving their search presence.

- **Content repurposing**: Transforming one piece of content into multiple formats (blog → LinkedIn → X → email → video script). AI handles the format adaptation, adjusting length, tone, and structure for each channel while preserving the core message and key takeaways. This is one of the highest-ROI AIO applications because it multiplies the distribution of every piece of content you create without requiring separate creative processes.

### AIO workflows

- **Keyword-to-cluster pipeline**: Feed seed keywords into AI → expand to 100+ related queries using a combination of AI suggestion, autocomplete data, and People Also Ask mining → cluster by topic and intent so that each cluster represents one content piece or content hub → prioritize clusters by buying signal strength (how close the searcher is to a purchase decision) and keyword difficulty (how hard it will be to rank). The output is a prioritized content calendar backed by data, not guesswork.

- **Brief generation**: Input the target keyword plus the URLs of the top 5-10 currently ranking pages → AI analyzes the existing SERP landscape and generates a comprehensive outline → the outline includes recommended headings, questions to answer, key subtopics to cover, word count range, and internal linking suggestions to existing pages on your site. Review and adjust the brief before passing it to the drafting stage. A strong brief is the single biggest quality lever in your content operation because it prevents wasted effort on unfocused or misaligned content.

- **Draft-and-optimize loop**: AI drafts the full article from the approved brief → a human editor reviews for accuracy, voice, and original insight, making substantive edits (not just light proofreading) → the edited draft is run through a content optimization tool (like Surfer SEO or Clearscope) that scores it against the SERP and identifies gaps → AI rewrites the weak sections based on the optimization feedback → a final human review confirms quality before publication. This loop typically produces content that scores in the top 10% of optimization tools on the first publication attempt.

- **Repurposing engine**: Published blog post → AI generates a LinkedIn post (150-300 words, hook-driven), an X thread (5-10 tweets with a narrative arc), an email newsletter excerpt (2-3 paragraphs with a CTA), and a short video script (60-90 seconds) in one session. Run this for each published piece to build a library of multi-format content assets from every article, dramatically increasing your total content reach without proportional effort increases.

- **Competitor monitoring**: Weekly AI scan of competitor blogs, changelogs, product updates, and social media activity → AI processes the raw data and produces a summarized report highlighting new positioning changes, feature announcements, content themes they are investing in, and messaging shifts. Review this report every Monday to inform your content priorities for the week. Over time, this creates an intelligence layer that keeps your GTM team aware of competitive moves without requiring hours of manual research.

### AI-native tools

A curated selection of the most impactful tools for building AIO workflows. See [data/tools-aio.json](data/tools-aio.json) for the full list with structured metadata, including pricing models, best-for-stage recommendations, and specific GTM use cases.

| Tool | What GTM teams use it for |
|---|---|
| [PromptPro](https://promptpro.live) | AI prompt engineering and agent-building platform that helps GTM teams master prompt design, build reusable AI workflows, and deploy AI agents for content, research, and automation tasks. Bridges the gap between knowing AI exists and operationalizing it across the GTM stack. |
| [Claude](https://claude.ai) | Content briefs, long-form drafting, strategic analysis, multi-step reasoning tasks, and complex research synthesis. Particularly strong for tasks requiring nuanced judgment, structured output, and maintaining consistency across long documents. |
| [Jasper](https://www.jasper.ai) | Scaled content production with brand voice controls, team collaboration on AI-generated content, and template-driven workflows for repeatable content types like product descriptions, ad copy, and social posts. Best for teams that need consistent brand voice across many content producers. |
| [Frase](https://www.frase.io) | SERP research, content brief generation, and AI writing combined in a single tool. Frase excels at the research-to-brief-to-draft workflow because it keeps SERP context visible during the writing process, helping writers align their content with search intent throughout the drafting stage. |
| [Descript](https://www.descript.com) | Video and audio editing through transcript-based editing (edit the text to edit the media), content repurposing from long-form video to short clips, and AI-powered features like filler word removal and studio sound. Essential for teams adding video and podcast content to their GTM mix. |
| [Zapier](https://zapier.com) | No-code automation connecting content workflows across tools. Examples include automatically creating a Trello card when a new brief is approved, pushing published posts to social scheduling tools, and syncing content performance data from analytics to your content tracking spreadsheet. Zapier is the glue that connects your AIO stack without requiring engineering resources. |
| [n8n](https://n8n.io) | Open-source, self-hosted AI workflow automation for technical teams that need more control, customization, and data privacy than Zapier offers. Build complex multi-step workflows that chain AI calls together, process data from multiple sources, and trigger actions across your GTM stack. Ideal for teams with engineering support who want to build proprietary AIO pipelines. |

---

## Pillar 3: GEO (Growth Engine Optimization)

GEO is the discipline of optimizing the entire GTM engine, covering not just top-of-funnel acquisition, but the full path from first touch to expansion revenue. While SEO brings visitors and AIO scales content, GEO connects everything to activation, conversion, retention, and revenue. Without GEO, you have a traffic machine with no revenue accountability. With GEO, every piece of content, every workflow, and every campaign is measured by its contribution to business outcomes.

### What GEO covers

- **Onboarding and activation**: Getting new signups to their first value moment as quickly and consistently as possible. The best SEO traffic is wasted if users sign up and never activate. Activation rate is the metric that connects marketing effectiveness to product-market fit. Define your activation event clearly (e.g., "created their first project," "sent their first message," "connected their first integration"), instrument it in your product analytics, and optimize the onboarding flow relentlessly to push this number up.

- **Product-led growth (PLG) loops**: Self-serve conversion, viral mechanics, and usage-based expansion. PLG means the product itself is the primary driver of acquisition, conversion, and expansion. In a PLG model, SEO-driven visitors sign up for a free tier, experience value through usage, and convert to paid based on natural expansion triggers (hitting usage limits, needing team features, wanting advanced capabilities). GEO designs and optimizes these loops so they convert efficiently and scale predictably.

- **Sales-assist motions**: Routing high-intent leads from content to sales with the right context and timing. Not every lead should go to sales (that overwhelms the team with low-quality conversations), and not every lead should stay in self-serve (some high-value prospects need human guidance). GEO designs the routing logic that determines which leads get a sales touch, what context the sales rep receives (which pages they visited, what content they engaged with, their company size and role), and when the outreach happens for maximum relevance.

- **Lifecycle marketing**: Behavior-triggered email, in-app messaging, and re-engagement campaigns tied to product events, not just arbitrary time delays. Examples include sending a tips email when a user completes onboarding, triggering an upgrade prompt when a user hits 80% of their free tier limit, and launching a re-engagement sequence when a previously active user goes dormant for 7 days. These campaigns are designed around product behavior signals rather than calendar-based scheduling.

- **Revenue attribution**: Connecting content and traffic data to pipeline and closed revenue. Without attribution, you cannot optimize the GTM engine because you do not know which inputs produce which outputs. Set up multi-touch attribution that tracks the full journey from first organic visit through signup, activation, opportunity creation, and closed-won revenue. This data tells you not just which content drives traffic, but which content drives revenue, and those are often very different lists.

- **Experimentation**: A/B testing landing pages, onboarding flows, pricing pages, and CTAs to improve conversion at every stage of the funnel. GEO teams run structured experiments with clear hypotheses, adequate sample sizes, and statistical rigor. Every stage of the S2R Loop is a candidate for experimentation. Common high-impact experiments include testing CTA copy and placement on blog posts, testing onboarding flow length and complexity, testing pricing page layout and tier structures, and testing free trial length against conversion rate.

### Key GEO levers

- **Onboarding flow optimization**: Personalize onboarding based on acquisition source, stated goal, company size, and role. Organic visitors from a "how to" article have different intent than visitors from a comparison page or a direct referral. The onboarding flow should adapt to these differences, showing different steps, examples, and templates based on what you know about the user. Measure onboarding completion rate and time-to-first-value by cohort to track improvement.

- **Activation metric definition**: Define and instrument the "aha moment," which is the specific action that predicts long-term retention and conversion. This requires analyzing your existing user data to find the behavior that most strongly correlates with retention at 30, 60, and 90 days. Once identified, optimize everything upstream toward this moment. Every onboarding step, every email, every in-app prompt should be designed to move users toward this action as efficiently as possible.

- **PLG conversion mechanics**: Free-to-paid triggers, usage limits, team expansion prompts, and feature gating. Design these to be natural and value-aligned, not punitive. The user should feel that upgrading unlocks meaningful additional value, not that the free tier was artificially crippled. Test different trigger points (e.g., at what usage level does a free user convert most willingly?) and optimize for long-term LTV, not just short-term conversion rate. A user who converts willingly at their natural expansion point retains better than one who converts reluctantly at an artificial gate.

- **Sales-assist routing**: Use enrichment data (company size, industry, role, funding stage) and behavioral scoring (pages visited, content downloaded, product usage patterns) to identify which organic leads should get a sales touch and which should stay in self-serve. Build routing rules that send high-value, high-intent leads to sales within minutes, not days. Provide the sales rep with full context about the lead's content journey and product behavior so the conversation starts with relevance rather than a cold introduction.

- **Lifecycle campaigns**: Build event-driven email and in-app message sequences tied to product behavior, not just time delays. Map out the key product events that signal intent, engagement, risk, or opportunity. Then design automated sequences for each: welcome and onboarding sequences, activation nudge sequences for users who signed up but have not reached the aha moment, upgrade sequences for power users approaching limits, re-engagement sequences for dormant users, and expansion sequences for active users who could benefit from additional features or seats.

- **Full-funnel dashboards**: Track from impression to revenue in one view. Segment by channel (organic, paid, referral, direct), by content cluster, by campaign, and by cohort. Calculate unit economics by acquisition source, including customer acquisition cost (CAC), LTV, payback period, and LTV-to-CAC ratio. This dashboard is the single most important analytical asset for a GTM team because it reveals where the funnel is healthy and where it is leaking, enabling precise investment decisions rather than gut-feel resource allocation.

### Growth tools

A curated selection of the most impactful tools for GEO. See [data/tools-geo.json](data/tools-geo.json) for the full list with structured metadata, including pricing models, best-for-stage recommendations, and specific GTM use cases.

| Tool | What GTM teams use it for |
|---|---|
| [Leorix](https://leorix.com) | Enterprise AI platform that unifies CRM, business intelligence, workflow automation, and lead management. AI-powered pipeline tracking connects acquisition data to closed revenue, automated lead enrichment and scoring trigger nurture sequences based on content engagement, and integrated BI dashboards provide multi-touch attribution reporting that links content to pipeline without juggling multiple tools. |
| [Mixpanel](https://mixpanel.com) | Product analytics for understanding user behavior inside the product, activation funnel analysis to identify where users drop off, retention cohort analysis to measure long-term engagement, and custom event tracking to define and monitor your activation metric. |
| [PostHog](https://posthog.com) | Open-source product analytics, feature flags for controlled rollouts and A/B testing, session recordings for qualitative user research, and built-in experimentation. PostHog is a strong choice for teams that want a unified product analytics and experimentation platform without vendor lock-in, and its open-source model appeals to developer-focused companies. |
| [Segment](https://segment.com) | Customer data infrastructure that collects events from your product and distributes them to all your analytics, marketing, and sales tools. Identity resolution to stitch together anonymous and known user profiles. Segment is the foundation layer that makes all downstream GEO tools more effective by ensuring consistent, reliable data flows across your entire stack. |
| [Mutiny](https://www.mutinyhq.com) | B2B website personalization for organic visitors, allowing you to show different headlines, CTAs, social proof, and content to different visitor segments based on firmographic data, referral source, and behavior. Particularly effective for increasing conversion rates on high-traffic pages by tailoring the message to the visitor's context. |
| [Customer.io](https://customer.io) | Event-driven lifecycle marketing automation that triggers messages based on product behavior events rather than calendar-based schedules. Build sophisticated multi-step campaigns that respond to what users actually do inside your product. Supports email, push notifications, in-app messages, and SMS, making it a versatile lifecycle marketing engine. |

---

## End-to-End GTM Workflows

These workflows span all three pillars and demonstrate how SEO, AIO, and GEO work together in practice. Each one is summarized here with enough detail to understand the approach and expected outcomes; detailed step-by-step versions with templates and examples are in [docs/workflows.md](docs/workflows.md).

### 1. From Zero to First 100 ICP Signups via SEO + AIO

**Goal:** An early-stage company with no organic traffic publishes its first 10 SEO-optimized pages and generates 100 ICP-fit signups within 90 days. This workflow is designed for founders and early marketers who need to prove that organic search can be a viable acquisition channel before investing further.

**Inputs:** A clearly defined ICP (ideal customer profile) with known pain points and search behavior, product positioning that differentiates from competitors, an AI writing tool (Claude, Jasper, or similar), a CMS for publishing (WordPress, Webflow, or similar), and basic analytics (Google Analytics + Search Console).

**Key steps:**

1. Define 3-5 seed topics tied directly to product use cases. These should be the problems your ICP is actively searching for solutions to. Validate each seed topic by checking search volume in PostWyse or Google Keyword Planner and confirming that the search intent matches what your product delivers. If your ICP does not search for these topics, choose different seeds.

2. Use AI to expand each seed topic into 10-20 related keywords, resulting in 50-100 total keywords. Then cluster these keywords by topic similarity and search intent using AI or a tool like Keyword Insights. Each cluster should represent one potential page. Classify each cluster as TOFU (informational), MOFU (consideration), or BOFU (decision) so your content plan has a balanced funnel distribution.

3. Prioritize 10 pages to publish first by scoring each cluster on two dimensions: buying intent (how close is the searcher to making a purchase decision?) and ranking difficulty (how competitive is the keyword based on domain authority of current rankers?). Select pages that have the highest buying intent at a difficulty level your domain can realistically compete at. For a new domain, this typically means targeting long-tail keywords with lower search volume but higher conversion potential.

4. Generate comprehensive content briefs with AI for each of the 10 prioritized pages. Each brief should include the target keyword, secondary keywords, recommended heading structure, key questions to answer, competitor analysis summary, word count guidance, and CTA recommendations. Then draft each page using AI as the first-draft writer, with a human editor making substantive revisions for accuracy, voice, original insight, and brand alignment.

5. Optimize every page for on-page SEO before publication. This includes meta title and description optimization, heading tag hierarchy, image alt text, internal linking to other pages in the batch, URL slug optimization, and adding schema markup where appropriate. Add conversion CTAs that match the page's funnel stage: TOFU pages get newsletter or guide download CTAs, MOFU pages get free trial or demo CTAs, and BOFU pages get direct signup or "talk to sales" CTAs.

6. Publish all 10 pages, then distribute each one through at least 2-3 additional channels (LinkedIn, email newsletter, relevant communities). Track performance weekly using a dashboard that shows impressions, clicks, signups, and activation rate for each page. After 4-6 weeks, identify which pages are gaining traction and double down with additional internal links, backlink outreach, and content updates.

**Outputs:** 10 published, SEO-optimized pages targeting ICP-relevant keywords, conversion tracking from page to signup for each page, a weekly performance dashboard, and a data-informed plan for the next content sprint based on which topics and formats performed best.

### 2. Upgrade Legacy Blog to AI-Optimized Revenue Engine

**Goal:** Transform an existing 50-200 post blog that generates traffic but low conversion into a measurable pipeline contributor. Many companies have invested in content over years but have never connected that content to revenue outcomes. This workflow adds the conversion infrastructure, content quality improvements, and measurement systems needed to turn traffic into pipeline.

**Inputs:** Existing blog content (50-200 posts), Google Search Console data (at least 3 months), a content optimization tool (Surfer SEO, Clearscope, or similar), CRM with pipeline tracking (Leorix, Salesforce, or similar), and product analytics for activation tracking.

**Key steps:**

1. Export all existing blog posts and categorize each one by funnel stage (TOFU, MOFU, BOFU) and conversion potential (high, medium, low). Conversion potential is assessed by asking: Does this post target a keyword with buying intent? Does it address a problem our product directly solves? Can a natural CTA be added without disrupting the content? This audit typically takes 1-2 days for 100 posts and produces a complete map of your content inventory by funnel stage and opportunity.

2. Identify quick wins by finding posts that currently rank in positions 4-20 for keywords with decent search volume (100+ monthly searches). These posts are already performing but have room to move onto page one. Cross-reference with conversion potential: a quick-win post that also has high conversion potential is your highest-priority target. Expect to find 10-30 quick-win candidates in a typical blog of 100+ posts.

3. Use AI to audit and rewrite the top 10 quick-win posts. For each post, run a content optimization analysis to identify gaps, use AI to expand thin sections, update outdated information, add new examples, improve heading structure, and strengthen the introduction and conclusion. Have a human editor review every AI rewrite for accuracy and voice. The goal is to transform each post from a basic article into the most comprehensive, useful resource available for that keyword.

4. Add conversion CTAs to every refreshed post, matching CTA type to funnel stage and reader intent. Consolidate thin content (posts under 500 words with little unique value) by either merging related thin posts into one comprehensive piece or redirecting them to stronger pages. Build hub structure by designating pillar pages and linking cluster content to them, creating clear topical architecture that search engines and readers can navigate.

5. Set up attribution tracking from blog to pipeline. This means instrumenting the journey from blog visit to form fill, from form fill to CRM lead, from lead to opportunity, and from opportunity to closed-won revenue. Use UTM parameters, hidden form fields, and CRM automation to pass attribution data through the entire funnel. Once this tracking is live, you can measure the pipeline contribution of every individual blog post and use that data to drive your editorial calendar.

**Outputs:** 10+ refreshed posts with improved content quality and conversion paths, a content hub architecture that strengthens topical authority, an attribution baseline that connects blog performance to pipeline, and a prioritized backlog of additional posts to refresh based on the audit.

### 3. GTM for New Feature Launch Powered by AI Content

**Goal:** Generate awareness, capture demand, and activate users around a new feature using AI-powered content within a 2-4 week timeline. Feature launches are time-sensitive opportunities where speed matters. This workflow uses AI to compress the content production timeline while maintaining quality, ensuring you have comprehensive content coverage ready at launch.

**Inputs:** Product brief or PRD (product requirements document) describing the feature, target audience segment and their key pain points, AI writing and optimization tools, design resources for landing page creation, and email marketing platform for existing user communication.

**Key steps:**

1. Extract the core narrative from the product brief using AI. Feed the PRD into AI and ask it to identify the primary user problem being solved, the key differentiator versus existing solutions or workarounds, the target audience segment and their language, and the most compelling benefit framing. This narrative extraction ensures all content pieces tell a consistent story and use consistent language, which is critical when multiple people are creating content simultaneously under time pressure.

2. Research the search landscape for the feature's problem space. Use keyword research tools to find what potential users search for when they have the problem your feature solves, what competitors rank for in this space, what questions appear in People Also Ask and forums, and what content formats (listicles, tutorials, comparisons) dominate the SERP. This research informs both the SEO strategy for your feature content and the messaging angles that will resonate most strongly.

3. Use AI to draft a complete content package: a feature landing page (focused on conversion), a tutorial blog post (focused on activation and SEO), a comparison page (focused on BOFU search traffic), and a release note or changelog entry (focused on existing user notification). Each piece should be drafted, human-edited, and optimized within the 2-4 week launch window. Parallelize the workflow by having AI draft all pieces simultaneously, then stagger human editing.

4. Optimize all content for SEO, including meta tags, heading structure, internal links, and schema markup. Set up feature-specific conversion tracking so you can measure how many visitors to the feature landing page convert to signups, and how many existing users activate the new feature after reading the tutorial or release note. Create a dedicated tracking dashboard that shows feature launch metrics in one view.

5. Build an email sequence for existing users that announces the feature, explains the value, and drives activation. Create social distribution assets (LinkedIn posts, X threads, and community posts) tailored to each channel's format and audience expectations. Schedule distribution to coincide with the launch date, with follow-up distribution in the days following to sustain momentum.

**Outputs:** A feature landing page optimized for conversion and SEO, supporting content (tutorial, comparison page, release note), an email sequence for existing users, a social distribution package, and a tracking dashboard that measures the feature launch's impact on signups, activation, and usage.

### 4. Product Notes to SEO + AIO + GEO Launch Plan

**Goal:** Turn rough product or feature notes into a complete GTM launch plan covering search, AI content, and growth. This workflow is designed for the common scenario where a product manager hands marketing a brief or a set of notes and expects a comprehensive go-to-market plan. AI dramatically accelerates this planning process by handling research, analysis, and first-draft plan generation.

**Inputs:** Raw product notes (can be bullet points, a Notion doc, a Slack thread, or a recorded Loom video transcript), ICP definition, and current GTM metrics as a baseline for setting targets.

**Key steps:**

1. Feed raw notes to AI to extract a structured feature summary, target audience definition, key differentiators, competitive positioning, and potential objections. AI is excellent at turning unstructured input into structured output, and this step saves hours of back-and-forth between product and marketing. Review the AI output with the product manager to confirm accuracy and completeness before proceeding.

2. Generate keyword research for the feature's problem space and map every keyword to a funnel stage. Identify the 5-10 highest-priority keywords to target in the launch content and assess the competitive difficulty for each. This research determines how much organic search opportunity exists for the feature and which keywords to prioritize in the content plan.

3. Define the content plan (which pages to create, in which formats, targeting which keywords), the GEO motion (will this feature be PLG self-serve, sales-assist, or a hybrid?), and the activation sequence (how will users discover and adopt this feature after signup?). These three elements together form the operational core of the GTM plan. Each one should be specific enough to execute without additional planning.

4. Draft a measurement plan that includes specific metrics to track, which tools will capture the data, target values for each metric, and how metrics map to each stage of the S2R Loop. Without a measurement plan defined before launch, you cannot evaluate success or optimize afterward. AI can draft this plan by mapping the feature's expected user journey to the S2R stages and recommending appropriate metrics for each.

5. Build a timeline with weekly milestones and assigned owners for every deliverable. Include content production milestones, technical implementation milestones (tracking, landing pages), and distribution milestones. Share the timeline with all stakeholders so there is a single source of truth for who is doing what and by when.

**Outputs:** A complete GTM launch plan document, a prioritized content calendar with keyword targets, a measurement plan with specific metrics and targets, and a timeline with weekly milestones and owner assignments.

### 5. Quarterly SEO + AIO + GEO Performance Review

**Goal:** Assess GTM engine performance across all three pillars, identify wins and gaps, and set priorities for the next quarter. This workflow is designed to be run at the end of every quarter to create a structured retrospective that informs the next quarter's planning. It prevents the common failure mode of running disconnected reviews for SEO, content, and growth without understanding how they interact.

**Inputs:** Google Search Console data for the quarter, product analytics data (Mixpanel, PostHog, or similar), CRM pipeline data showing opportunities and revenue by source, content production log showing what was published and when, and the previous quarter's goals and targets for comparison.

**Key steps:**

1. Pull acquisition, activation, and revenue metrics for the organic channel specifically. Key metrics include: organic sessions, organic signups, organic activation rate, organic-sourced pipeline value, organic-sourced closed-won revenue, and organic LTV. Compare each metric to the previous quarter and to the targets set at the beginning of the quarter. Identify which metrics improved, which declined, and which remained flat.

2. Rank all published content by three dimensions: traffic generated, conversion rate to signup, and pipeline contribution (revenue influence). This three-dimensional ranking reveals which content is high-traffic but low-converting (potential CTA optimization opportunity), which content is low-traffic but high-converting (potential SEO investment opportunity), and which content drives actual pipeline and revenue (your most valuable content to protect and replicate).

3. Review AIO efficiency by measuring production velocity (how many pieces were published this quarter vs. last quarter?), AI-to-human ratio (what percentage of first drafts were AI-generated?), edit time per piece (is the AI-to-human handoff improving?), and content quality scores (are optimization scores trending up or down?). This review tells you whether your AIO investment is paying off in measurable productivity gains and whether the quality bar is being maintained as volume increases.

4. Assess GEO funnel health by examining conversion rates at every stage of the S2R Loop. Identify the biggest bottleneck, which is the stage with the lowest conversion rate or the largest drop-off relative to benchmarks. This bottleneck is where you should concentrate next quarter's improvement efforts, because improving the weakest link in the funnel has the highest impact on overall revenue throughput.

5. Use AI to synthesize all of the above data into insights and draft next-quarter priorities. Feed AI the key metrics, content rankings, AIO efficiency data, and funnel health assessment, and ask it to identify the top 3 wins to celebrate, the top 3 gaps to address, and recommended priorities for the next quarter. Human leadership reviews and finalizes the priorities, but AI accelerates the analysis and ensures no important patterns are missed.

**Outputs:** A quarterly performance report with visualizations of key metrics and trends, content performance rankings sorted by traffic, conversion, and pipeline contribution, AIO efficiency metrics and trends, a funnel health assessment with bottleneck identification, and a prioritized list of next-quarter initiatives with rationale.

---

## Playbooks by Stage

Detailed playbooks with step-by-step instructions, templates, and examples are in [docs/playbooks.md](docs/playbooks.md). Below is a summary by company stage, designed to help you quickly identify which plays are most relevant for your current situation.

### Early Stage (0 → 1 GTM)

You have a product and early traction but no scalable acquisition engine. Resources are limited, typically a founder, one marketer, or a small agency. Every initiative must be high-leverage, meaning it must produce outsized results relative to the time and money invested. The goal at this stage is to prove that organic search can be a viable, scalable channel before committing to a full content team.

**Recommended plays:**

- **SEO-driven founder-led narrative**: Use the founder's unique market insight, industry experience, and contrarian point of view as the content differentiator. Write 5 thesis-driven posts that rank for high-intent queries and establish the company's perspective on the problem space. These posts should not be generic "what is X" articles. They should contain original thinking, proprietary data, or a distinct framework that no competitor can replicate. This approach works because founders have authentic expertise that AI and content teams cannot easily imitate, and it builds brand authority from day one.

- **AIO-powered content sprint**: Use AI to publish 20-30 SEO-optimized pages in 30 days, covering the primary keyword universe for your product's use cases. The process is: generate keyword clusters with AI, create briefs with AI, draft with AI, and then have the founder or marketer edit each piece for accuracy, voice, and insight. This sprint establishes your initial search footprint and gives you data on which topics and formats perform best. Without this data, all future content strategy is guesswork. Aim for a mix of TOFU, MOFU, and BOFU content so you can measure conversion rates at each funnel stage.

- **Minimum viable measurement**: Set up basic tracking before investing in more content. At minimum, you need Google Search Console (to see which queries bring visitors), Google Analytics or a product analytics tool (to track signups and activation), and a CRM or spreadsheet (to track leads through the funnel). Connect these three data sources so you can answer the question: "Which search queries produce visitors who sign up and activate?" This measurement foundation, while simple, gives you the feedback loop needed to make data-informed content decisions from the very beginning.

### Growth Stage (1 → N)

You have organic traffic and some pipeline, but content ROI is hard to prove, activation is inconsistent, and scaling content quality is a challenge as you produce more. The goal at this stage is to build systems that connect content investment to revenue outcomes, improve the efficiency of your content operation, and optimize the full funnel from traffic through expansion.

**Recommended plays:**

- **Content-to-pipeline attribution engine**: Build a system that connects every content piece to leads, pipeline, and revenue using multi-touch attribution. This requires instrumenting the full journey from first organic visit through CRM opportunity and closed-won deal. Once live, use this data to drive the editorial calendar: invest more in content clusters that produce pipeline and less in clusters that produce only traffic. Attribution data is the single most powerful tool for earning executive buy-in for content investment, because it speaks the language of revenue rather than vanity metrics.

- **PLG + SEO flywheel**: Create a self-reinforcing loop where SEO content drives signups, product usage creates content signals (user-generated content, community posts, template galleries), and those signals improve SEO through fresh content, backlinks, and engagement metrics. Companies like Notion, Figma, and Canva have built powerful flywheels where the community content generated by users becomes a major SEO asset that drives further growth. Identify what user-generated content your product naturally creates and build systems to make it discoverable in search.

- **AIO content ops scaling**: Implement the full AIO Content Stack (all six layers) to double content production velocity without doubling headcount. This means establishing AI-assisted workflows for every stage from research through experimentation, with clear quality controls and human checkpoints at each layer. Track AIO efficiency metrics (production velocity, cost per piece, quality scores) to prove the ROI of your AI investment and identify which layers need further optimization.

### Enterprise / Multi-Product

You have multiple product lines, large content footprints (hundreds or thousands of pages), and cross-team coordination challenges. The risk is cannibalization (multiple product teams targeting the same keywords), duplication (similar content published by different teams), and misaligned investment (over-investing in some products while under-investing in others). The goal at this stage is governance, efficiency, and full-funnel measurement at scale.

**Recommended plays:**

- **Multi-product SEO architecture**: Design keyword ownership rules that clearly assign which product team owns which keyword clusters, preventing internal competition. Create content hub structures for each product line with clear boundaries and intentional cross-linking where appropriate. Establish governance processes (quarterly keyword audits, cross-team content calendars, editorial review boards) that prevent cannibalization and duplication without slowing down individual teams. This architecture becomes critical as the content footprint grows, because unmanaged growth leads to keyword cannibalization that actually reduces total organic traffic.

- **RevOps + GEO instrumentation baseline**: Build full-funnel instrumentation that connects marketing data, product analytics data, and revenue data into a unified measurement system. This typically requires a customer data platform (like Segment), a product analytics tool (like Mixpanel or PostHog), and a revenue analytics layer (like a BI tool connected to your CRM). The instrumentation baseline should support attribution by product line, by content cluster, by channel, and by campaign, enabling precise investment optimization across the entire multi-product GTM engine.

- **AI-powered content governance**: Use AI to monitor content quality, keyword cannibalization, and messaging consistency across product lines at a scale that manual review cannot achieve. Set up automated AI scans that flag potential cannibalization issues (two pages from different product teams targeting the same keyword), content quality degradation (pages whose optimization scores have dropped), and messaging inconsistencies (product positioning that contradicts other product lines). This governance layer is the only practical way to maintain content quality and strategic alignment across hundreds or thousands of pages.

---

## Data Files

The `/data` directory contains structured metadata for tools across all three pillars. These files are designed to be machine-readable (JSON format) so that teams can filter, sort, and programmatically query the tool database based on their specific needs (stage, budget, use case). The data files are validated by a GitHub Actions workflow on every commit to ensure schema compliance and data integrity.

| File | Contents |
|---|---|
| [data/tools-seo.json](data/tools-seo.json) | SEO tools covering keyword research, technical SEO auditing, content optimization, rank tracking, backlink analysis, and search analytics |
| [data/tools-aio.json](data/tools-aio.json) | AI and AIO tools covering AI writing assistants, content platforms, workflow automation, research synthesis, and content repurposing |
| [data/tools-geo.json](data/tools-geo.json) | GEO and Growth tools covering product analytics, CRM and marketing automation, experimentation platforms, lifecycle marketing, and customer data infrastructure |

### Shared schema

Every tool entry follows the same structure, designed for GTM decision-making rather than generic tool comparison. The schema intentionally focuses on practical information that helps a GTM team evaluate whether a tool fits their stage, budget, and use case.

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

- **`summary`**: Describes what a GTM team actually gets from this tool in practical terms. No hype, no marketing language. This should tell a GTM leader exactly what the tool does in their context so they can quickly assess relevance without visiting the tool's website.

- **`gtm_use_cases`**: Concrete actions a GTM team would take with this tool. These are not feature descriptions ("has keyword tracking") but activity descriptions ("track weekly ranking changes across your target keyword set to identify content that needs refreshing"). The distinction matters because GTM teams evaluate tools by what they enable, not by what features they list.

- **`pricing_model`**: Helps teams filter by budget constraints. Options are `free` (no cost for the primary use case), `freemium` (useful free tier with paid upgrades for advanced features or higher usage), or `paid` (requires payment to access core functionality). This field enables early-stage teams with no budget to quickly find free alternatives and enterprise teams to filter for tools that offer the support and scale they need.

- **`best_for_stage`**: Helps teams filter by company stage. Options are `early` (suitable for startups with limited resources and small content footprints), `growth` (suitable for teams with established traffic and pipeline looking to scale and optimize), and `enterprise` (suitable for large organizations with multiple product lines, large teams, and complex governance needs). A tool can be appropriate for multiple stages.

---

## About This Project

This repo is a living GTM reference. It is designed for teams who want to operationalize SEO + AIO + GEO, not just learn definitions, but build systems that work in practice. The content is continuously updated as the search, AI, and growth landscapes evolve, and as practitioners contribute new frameworks, workflows, and real-world examples.

It is intentionally opinionated. The frameworks, workflows, and playbooks reflect how high-performing GTM teams actually operate, not how marketing textbooks say they should. Where there are trade-offs, we state them. Where there are anti-patterns, we call them out. Where a popular approach is overrated or misunderstood, we explain why and offer a better alternative. This opinionated stance is a feature, not a bug, because practitioners need clear recommendations they can act on, not balanced summaries of every possible approach.

This is not:
- A comprehensive directory of every marketing tool that exists. We curate deliberately, including only tools that provide clear GTM value, and we explain specifically what that value is.
- An SEO-only resource. SEO is one of three pillars, and this repo deliberately connects it to AI operations and revenue engineering.
- A theoretical academic reference. Every framework and workflow is designed to be executed, not just studied.
- A vendor pitch. No tool is included because of a sponsorship or affiliate relationship. Tools are included based on their utility to GTM practitioners.

This is:
- A practical guide for building a GTM engine that uses search, AI, and growth engineering as interconnected systems that compound each other's impact.
- A reference for choosing the right tools, workflows, and plays for your specific stage and context, with enough detail to actually implement them.
- A community resource that gets better as practitioners contribute their experience, their frameworks, and their hard-won lessons from building GTM engines in the real world.

Contributions from GTM leaders, founders, and technical marketers are welcome. See below for how to contribute.

---

## Contributing

We welcome contributions that make this resource more useful for GTM practitioners. See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines, including detailed instructions for each contribution type and examples of high-quality contributions.

**Types of contributions:**

- **Tools**: Add a new tool to the relevant JSON file (tools-seo.json, tools-aio.json, or tools-geo.json) with proper GTM use cases that describe what a team actually does with the tool, not just what features it has. Follow the shared schema exactly, and include a summary that would help a GTM leader evaluate the tool in under 10 seconds.

- **Frameworks**: Propose a new framework or improve an existing one. New frameworks should address a gap in the current coverage, be grounded in real-world GTM practice, and include concrete examples of how to apply the framework. Improvements to existing frameworks should add clarity, examples, or nuance based on practitioner experience.

- **Workflows**: Document an end-to-end GTM workflow that spans pillars. A good workflow contribution includes the goal, required inputs, detailed step-by-step instructions, expected outputs, and at least one example of the workflow in action. The bar is high because workflows are the most actionable content in this repo.

- **Playbooks**: Add a stage-specific playbook with real-world applicability. Playbooks should be specific enough to execute without additional research, include timing estimates and resource requirements, and explain not just what to do but why it works and what to watch out for.

- **Examples**: Contribute concrete examples such as content briefs, measurement plans, OKR sets, editorial calendars, attribution models, or dashboard designs. Examples bring abstract frameworks to life and help practitioners translate concepts into action for their specific context.

**Requirements for new tool entries:**
- Must include specific GTM use cases that describe concrete actions, not just "it's a good tool" or a restatement of the vendor's marketing copy.
- Must follow the shared schema exactly, including all required fields with accurate data.
- No affiliate links. No self-promotion without substance. If you are submitting your own tool, the GTM use cases must be genuinely useful and the entry must meet the same quality bar as every other tool in the database.

**Quality bar:**
- Practical over theoretical. Every contribution should help a practitioner do something they could not do before, or do something they already do more effectively.
- Specific over generic. "Improve your SEO" is generic. "Audit your top 20 posts by pipeline contribution and refresh the bottom 5" is specific.
- GTM outcome-focused, not feature-list-focused. We care about what a tool, framework, or workflow enables in terms of pipeline and revenue, not about feature counts or technical specifications.

---

## License

This project is licensed under the [MIT License](LICENSE).
