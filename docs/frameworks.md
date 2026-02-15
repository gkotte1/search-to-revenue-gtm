# Core Frameworks

This document expands on the four core frameworks referenced in the README. Each framework gives GTM teams a mental model for connecting search, AI, and growth into a unified system. The goal is to provide not just theoretical structure but practical, actionable guidance so that teams can immediately apply these models to their own businesses. Whether you are building a GTM engine from scratch or optimizing an existing one, these frameworks serve as the connective tissue between strategy and execution.

---

## 1. Search-to-Revenue Loop (S2R Loop)

### Overview

The S2R Loop is a five-stage model that maps how a potential customer moves from a search query to revenue, and how SEO, AIO, and GEO each contribute at every stage. Unlike traditional marketing funnels that stop at "lead," the S2R Loop runs all the way to expansion revenue and explicitly identifies where AI and growth engineering accelerate the loop. The fundamental insight behind the S2R Loop is that search behavior does not end at the top of the funnel. Buyers search at every stage of their journey, from initial problem awareness through vendor evaluation, onboarding questions, feature discovery, and renewal decision-making. By modeling the entire journey as a continuous loop rather than a linear funnel, teams can identify leverage points where small improvements create compounding returns across the full customer lifecycle.

### When to use it

- **Planning a new GTM motion from scratch.** When you are starting with a blank slate, the S2R Loop gives you a complete architecture to build against. Rather than optimizing individual channels in isolation, you can design every touchpoint to feed into the next stage. This prevents the common mistake of over-investing in top-of-funnel traffic without building the infrastructure to convert and retain that traffic.
- **Auditing an existing content or growth engine to find bottleneck stages.** If your GTM engine is underperforming, the S2R Loop helps you diagnose exactly where the breakdown is occurring. For example, you might discover that your Discover stage is strong (plenty of organic traffic) but your Capture stage is weak (low conversion to known leads). This stage-by-stage diagnosis prevents wasted effort on areas that are already performing well.
- **Aligning cross-functional teams (marketing, product, sales, RevOps) on a shared model.** One of the most common GTM failures is functional silos, where marketing optimizes for traffic, sales optimizes for pipeline, and product optimizes for engagement, all without a shared framework. The S2R Loop gives every team a common language and a shared understanding of how their work connects to revenue outcomes.

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

**Discover.** The buyer has a problem and searches for answers. This is the stage where awareness is created, and it encompasses everything from broad informational queries ("what is observability?") to narrowly scoped problem queries ("why does my Kubernetes pod keep crashing?"). The quality of your Discover stage determines the size and relevance of your addressable audience. Getting this wrong means either attracting the wrong visitors or missing high-intent buyers entirely.

- **SEO: Rank for high-intent queries with the right content type (informational, comparison, solution-aware).** This means going beyond simple keyword targeting. You need to match the search intent precisely, which requires analyzing the SERP for each target query to understand what format Google rewards (long-form guide, listicle, comparison table, video). Content that mismatches intent will not rank regardless of its quality. Build a keyword-to-content-type mapping as part of your editorial calendar so that writers and AI tools know exactly what format each piece should take.
- **AIO: Use AI to research keywords, generate briefs, and draft content at scale.** AI tools dramatically compress the time from keyword opportunity identification to published content. The key is establishing a repeatable workflow: AI performs the initial keyword clustering and competitive analysis, generates a structured brief with target headings and questions to answer, and then produces a first draft that a human editor refines. This workflow can reduce content production time from weeks to days while maintaining quality through human oversight at the editing stage.
- **GEO: Ensure analytics capture the discovery source and intent signal.** Every visitor who arrives through the Discover stage carries valuable data about their intent, their context, and the channel that brought them. Your analytics infrastructure must capture not just the traffic source (organic, paid, referral) but also the specific query or content that attracted them. This data feeds the feedback loop and informs downstream personalization. Without proper attribution at the Discover stage, you lose the ability to optimize the rest of the loop.

**Capture.** The visitor arrives. You need to capture identity or intent. This stage is where anonymous traffic transforms into known, actionable contacts. The capture mechanism must feel valuable to the visitor, not extractive. The best capture strategies offer something immediately useful (a free tool, a personalized assessment, a template) in exchange for identity information. A poorly designed Capture stage is the most common reason GTM engines leak, because even high volumes of quality traffic produce zero pipeline if you cannot identify the visitors.

- **SEO: On-page CTAs optimized for the search intent (demo, free tool, gated asset).** The CTA must match the intent behind the query that brought the visitor to the page. A visitor searching "how to calculate churn rate" is in learning mode, so a CTA for a free churn calculator is far more effective than a CTA for a sales demo. Map each content piece to the appropriate CTA type based on where the visitor is in their buying journey. Test CTA placement (inline vs. sidebar vs. end-of-post) and format (button vs. embedded tool vs. chatbot prompt) to find the highest-converting combinations.
- **GEO: Forms, chat, and enrichment tools convert anonymous visitors into known leads.** Growth engineering provides the technical infrastructure for capture. This includes progressive profiling forms that ask only one or two questions initially and gather more data over time, live chat or chatbot widgets that engage visitors at moments of high intent, and third-party enrichment tools (like Clearbit or ZoomInfo) that append firmographic data to captured email addresses. The goal is to build a rich contact record with minimal friction for the visitor.
- **AIO: AI-personalized CTAs or chat responses based on visitor signals.** AI enables dynamic personalization of the capture experience. Based on signals like the referring search query, the visitor's geographic location, the pages they have viewed, and their firmographic profile (if enriched), AI can customize the CTA copy, the chat greeting, or the recommended resource. This personalization meaningfully increases capture rates because the visitor sees an offer that feels tailored to their specific situation rather than a generic prompt.

**Activate.** The lead or signup takes a meaningful first action. Activation is the most critical and most overlooked stage in most GTM engines. It is the bridge between "someone who signed up" and "someone who experiences value." Without activation, leads decay, free trials expire unused, and the pipeline that marketing worked so hard to create evaporates. The definition of activation varies by product: for a developer tool, it might be "ran their first build"; for an analytics platform, it might be "connected a data source and viewed their first dashboard."

- **GEO: Onboarding flows, product tours, and activation emails.** Growth engineering builds the rails that guide new users toward their activation moment. This includes in-product onboarding checklists that highlight the three to five steps needed to experience core value, interactive product tours that walk users through key features, and time-triggered email sequences that re-engage users who signed up but have not yet activated. Each of these touchpoints should be instrumented with analytics so you can measure drop-off at every step and continuously optimize.
- **AIO: AI-generated onboarding content personalized to the user's stated goal or industry.** Generic onboarding content underperforms because different users need different paths to value. AI enables you to generate personalized onboarding content at scale. For example, if a user indicates during signup that they are in healthcare, the onboarding sequence can include healthcare-specific use cases, templates, and compliance considerations. This personalization requires collecting minimal data at signup (role, industry, primary goal) and using AI to dynamically generate or select the appropriate content for each segment.
- **SEO: Help docs and knowledge base content that ranks and supports activation.** Well-structured help documentation serves double duty. It supports activation by answering the questions that new users encounter during onboarding, and it ranks in search engines to capture users who are researching whether a product can solve their specific problem. Help docs should be written with both audiences in mind: the existing user trying to complete a task, and the prospective user evaluating whether the product can meet their needs.

**Convert.** The activated user becomes a paying customer. Conversion is where the GTM engine produces direct revenue, and it requires tight coordination between product, marketing, and sales. The conversion motion varies dramatically by business model. Product-led growth (PLG) companies convert through self-serve upgrade flows and pricing pages. Sales-led companies convert through demo calls, proposals, and procurement processes. Most modern B2B companies use a hybrid approach where PLG handles small accounts and sales handles enterprise deals.

- **GEO: Sales-assist motions, pricing optimization, trial-to-paid conversion flows.** Growth engineering at the Convert stage includes designing and testing pricing pages, building automated sales-assist triggers (for example, sending a personalized offer when a free user hits a usage limit), and creating self-serve upgrade flows that minimize friction. For sales-assisted deals, GEO includes CRM workflows that route qualified leads to the right rep, deal scoring models that prioritize high-probability opportunities, and conversion analytics that identify the most common objections and drop-off points.
- **AIO: AI-generated sales collateral and proposal content.** AI can dramatically accelerate the creation of sales materials that would otherwise require hours of manual work. This includes generating customized proposals based on the prospect's industry and stated needs, creating ROI calculators pre-populated with relevant benchmarks, drafting case study summaries that highlight similar customers, and producing competitive battle cards that address the specific alternatives the prospect is evaluating. The key is connecting AI to your CRM data so that generated content reflects the actual context of each deal.
- **SEO: Bottom-of-funnel comparison and alternative pages that influence the decision.** Buyers at the Convert stage frequently search for terms like "[your product] vs [competitor]," "[your product] pricing," and "[your product] reviews." These bottom-of-funnel queries represent high-intent traffic that directly influences purchasing decisions. Creating well-structured comparison pages, pricing FAQs, and customer story pages ensures that your brand controls the narrative during this critical evaluation phase rather than ceding it to third-party review sites or competitor content.

**Expand.** The customer grows in value through upsell, cross-sell, and advocacy. Expansion is where the S2R Loop diverges most significantly from traditional marketing funnels. Most funnels treat conversion as the endpoint, but in SaaS and subscription businesses, the majority of lifetime value comes after the initial purchase. The Expand stage encompasses everything from increasing per-account revenue (upsell and cross-sell) to reducing churn (retention) to turning customers into advocates who drive new Discover-stage traffic (referrals, case studies, community content).

- **GEO: Lifecycle marketing, usage-based expansion triggers, NRR optimization.** Growth engineering at the Expand stage focuses on identifying and acting on signals that indicate expansion opportunity or churn risk. Usage-based triggers (for example, a team approaching their seat limit, or a customer using 90% of their API quota) should automatically initiate expansion outreach. Churn risk signals (declining login frequency, support ticket spikes, failure to adopt key features) should trigger retention campaigns. NRR (Net Revenue Retention) is the north star metric for this stage, and it should be decomposed into its component parts (gross retention, expansion rate, contraction rate) for precise optimization.
- **AIO: AI-powered customer success content, renewal collateral.** AI enables customer success teams to operate at scale by automating the creation of personalized usage reports, renewal proposals, and feature adoption recommendations. For example, AI can analyze a customer's product usage data and generate a quarterly business review deck that highlights the value they have received, the features they have not yet adopted, and the ROI case for upgrading. This kind of personalized outreach, which would be prohibitively time-consuming to create manually for every account, becomes feasible with AI.
- **SEO: Customer-generated content, case study pages, community SEO.** Happy customers produce content that fuels the Discover stage for new prospects. Case study pages that rank for industry-specific queries, community forums where customers discuss use cases and best practices, and user-generated templates or integrations all create organic discovery paths. The key is making it easy for customers to create and share this content, and then ensuring it is properly optimized to rank in search engines.

### Feedback loop

Revenue outcomes and customer behavior data feed back into the Discover stage, creating a self-reinforcing cycle that compounds over time. This feedback loop is what makes the S2R Loop a loop rather than a linear funnel. Without it, each stage operates in isolation and the GTM engine never learns from its own results.

- **High-converting topics inform keyword strategy.** When you know which content topics produce the highest conversion rates (not just the most traffic), you can shift your editorial calendar toward those topics. This requires end-to-end attribution from the initial search query through to revenue, which is a non-trivial analytics challenge but one that pays enormous dividends. A topic that generates 1,000 monthly visits and a 5% conversion rate is far more valuable than one that generates 10,000 visits with a 0.1% conversion rate.
- **Customer language from sales calls shapes content messaging.** The words and phrases that customers use to describe their problems, their goals, and the value they receive are the most authentic and resonant copy you can use in Discover-stage content. Mining sales call transcripts, onboarding interviews, and customer reviews for this language (often called "voice of customer" research) ensures that your content speaks the same language as your audience. AI can automate this mining process by analyzing transcripts and extracting recurring themes and phrases.
- **Expansion patterns reveal new content opportunities.** When you observe that customers frequently expand into a particular use case or feature area, that pattern signals a content opportunity at the Discover stage. For example, if many customers who initially adopt your product for use case A eventually expand into use case B, creating Discover-stage content about use case B will attract prospects who are already predisposed to become high-value, multi-use-case customers.

### Example scenario: B2B SaaS (Developer Tools)

A developer tools company uses the S2R Loop to build an integrated GTM engine that spans from organic search all the way through expansion revenue.

1. **Discover**: The team identifies that "how to debug [framework] in production" is a high-volume, high-intent query cluster. Using the AIO Content Stack, they research the keyword cluster, generate structured briefs, and produce an AI-drafted technical guide that a senior engineer reviews for accuracy. The guide includes real code examples, common pitfalls, and a step-by-step debugging methodology. It ranks on page one within eight weeks due to its depth, technical accuracy, and strong on-page optimization.
2. **Capture**: Within the guide, the team embeds an interactive free debugging tool that allows readers to paste a stack trace and receive an AI-powered analysis of probable root causes. Accessing the tool requires only an email address. This CTA converts at 12% because it is directly relevant to the task the reader is trying to accomplish, unlike a generic "request a demo" button that would convert at under 1% for this audience.
3. **Activate**: After signup, the developer receives a three-email onboarding sequence. The first email walks them through their first debugging session using the free tool. The second email introduces advanced features like team-shared debugging sessions. The third email highlights integrations with popular CI/CD platforms. Each email is personalized based on the framework the developer was searching for when they discovered the product.
4. **Convert**: The system monitors product usage, and after three debugging sessions, it triggers a sales-assist motion. A product specialist reaches out with a personalized message referencing the bugs the developer has debugged, and offers a team plan trial. For smaller teams, a self-serve upgrade flow triggers when the developer invites a colleague, since the free plan supports only one user.
5. **Expand**: Once the team plan is active, the system monitors usage across the organization. When new team members onboard, it triggers a welcome sequence. When usage approaches the plan limit, it triggers an expansion conversation. When a team achieves a significant milestone (for example, reducing mean time to resolution by 40%), it triggers a case study request that, if completed, feeds back into Discover-stage content.

---

## 2. AIO Content Stack

### Overview

The AIO Content Stack describes the six layers of content production where AI can be systematically applied. It replaces the old "writer → editor → publish" model with an AI-augmented pipeline that is faster, more consistent, and measurable. The core principle of the AIO Content Stack is that AI should be applied at every layer of content production, not just at the drafting stage where most teams first experiment with it. Research, briefing, optimization, distribution, and experimentation all benefit from AI augmentation, and the compound effect of applying AI across all six layers is far greater than the sum of applying it at any single layer. The Stack is designed to be adopted incrementally: teams can start by introducing AI at whichever layer is their current bottleneck and expand from there.

### When to use it

- **Building or restructuring a content operations team.** The AIO Content Stack provides a blueprint for content team structure and workflows. Each layer suggests specific roles (researcher, brief writer, drafter, editor, distribution specialist, experimentation analyst) and shows where AI can augment or partially automate each role. When restructuring a content team, this framework helps you identify which roles can be made more efficient with AI and where human expertise remains essential, particularly in areas like subject-matter accuracy, brand voice, and strategic prioritization.
- **Evaluating where to introduce AI tools into existing workflows.** If your team is already producing content but wants to adopt AI, the Stack helps you diagnose which layer will benefit most from AI augmentation. A common mistake is jumping straight to AI drafting (Layer 3) when the real bottleneck is upstream at research (Layer 1) or downstream at distribution (Layer 5). By mapping your current workflow to the six layers and measuring throughput at each stage, you can identify where AI will have the highest impact and avoid wasting budget on tools that address the wrong problem.
- **Diagnosing content pipeline bottlenecks (for example, "we generate briefs fast but drafts take weeks").** The layered architecture makes it easy to measure cycle time at each stage and identify exactly where content gets stuck. If briefs are produced quickly but drafts lag, the bottleneck is at Layer 3 (Drafting), and the solution is either AI-assisted first drafts or additional writer capacity. If drafts move fast but published content does not perform well, the bottleneck might be at Layer 4 (Optimization) or Layer 2 (Briefs), where inadequate SEO targeting leads to content that never ranks.

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

- **Input**: Product positioning, ICP (Ideal Customer Profile) definition, seed keywords, and existing customer data. You need a clear understanding of who you are targeting, what problems they face, and what language they use to describe those problems. Without solid inputs at the research layer, every downstream layer will produce misaligned content.
- **AI role**: Cluster keywords into topic groups based on semantic similarity and search intent. Classify each cluster by intent type (informational, navigational, commercial, transactional). Scrape and summarize the top-ranking competitor content for each cluster to identify content gaps and opportunities. Extract recurring themes from customer call transcripts, support tickets, and product reviews to surface the exact language your audience uses. AI is particularly powerful here because research is time-intensive and repetitive, making it an ideal candidate for automation. The goal is to compress what would normally take a content strategist several weeks into a few hours.
- **Output**: A prioritized topic list ranked by a composite score of search volume, intent alignment with your product, competitive difficulty, and estimated traffic potential. Each topic in the list should include the primary keyword, secondary keywords, intent classification, a brief summary of what top-ranking competitors cover, and a gap analysis showing what they miss. This output becomes the master editorial backlog that drives all downstream content production.

**Layer 2: Briefs**

- **Input**: A prioritized topic from Layer 1, including all associated keyword and competitive data. The brief writer (human or AI) also needs access to your brand guidelines, tone-of-voice documentation, and any product-specific messaging frameworks.
- **AI role**: Generate a comprehensive content brief that includes the target keyword and secondary keywords, a recommended title (with alternatives for testing), an outline of recommended headings (H2s and H3s), specific questions the content should answer (derived from "People Also Ask" data and competitor analysis), a target word count range based on what currently ranks, a summary of the top three to five competitor articles with notes on what they cover well and what they miss, and internal linking suggestions to existing content on your site. The brief should be detailed enough that any competent writer (human or AI) can produce a high-quality draft without additional research.
- **Output**: A complete content brief document that is ready to hand off to a writer. The brief should serve as both a creative guide and a quality checklist. After the draft is complete, the brief can be used to verify that all requirements were met. Teams that skip or shortcut the briefing layer consistently produce content that underperforms, because writers lack the strategic context to make good decisions about structure, depth, and emphasis.

**Layer 3: Drafting**

- **Input**: The completed content brief from Layer 2. The drafter (human or AI) should also have access to any relevant product documentation, case studies, or subject-matter expert interviews that are referenced in the brief.
- **AI role**: Generate a complete first draft based on the brief's specifications. The AI draft should follow the recommended outline, incorporate target keywords naturally, answer all specified questions, and match the target word count range. The critical human role at this layer is editing the AI draft for accuracy, voice, and subject-matter depth. AI is excellent at producing structurally sound, well-organized content, but it can hallucinate facts, miss nuance, and fail to capture the authentic voice that distinguishes great content from generic content. Human editors should focus their energy on these areas rather than on structural or grammatical issues, which AI handles well.
- **Output**: A polished draft that is ready for SEO optimization. The draft should read as though it was written by a knowledgeable human in your brand's voice, with AI having handled the structural heavy lifting. Establish a clear quality bar: the draft should be factually accurate, well-structured, engaging to read, and aligned with the brief's specifications. Any draft that does not meet this bar goes back for revision rather than forward to optimization.

**Layer 4: Optimization**

- **Input**: The polished draft from Layer 3. The optimizer also needs access to your SEO tooling (content scoring tools like Surfer, Clearscope, or MarketMuse), your site's internal linking map, and your content hub architecture plan.
- **AI role**: Score the draft against SEO optimization targets, including keyword density, NLP entity coverage, heading structure, and content depth relative to competing pages. Suggest specific internal links to other pages on your site, ensuring that the new content strengthens your overall site architecture. Check that the heading structure follows a logical hierarchy and that all target questions from the brief are answered. Identify any thin sections that might benefit from additional depth or supporting data. AI optimization tools are most effective when used as a checklist rather than a replacement for editorial judgment. A high optimization score does not guarantee good content, but a low score almost always indicates missed opportunities.
- **Output**: An SEO-optimized draft that is ready for publication. The output should include a clear optimization score, a list of any remaining issues to address, and confirmed internal links. The content should be structured for both human readability and search engine comprehension, with clear headings, concise paragraphs, relevant images or diagrams, and proper meta tags (title, description, canonical URL).

**Layer 5: Distribution**

- **Input**: The published content from Layer 4, along with your channel strategy (which platforms you publish to) and each channel's format requirements and audience characteristics.
- **AI role**: Generate derivative formats tailored to each distribution channel. This includes LinkedIn posts that summarize the key insight from the article in a format optimized for the LinkedIn feed algorithm, Twitter/X threads that break the article into a series of concise, engaging points, email newsletter excerpts that highlight the most relevant section for your subscriber audience, short-form video scripts that present the core idea visually, and carousel or infographic formats for platforms that favor visual content. The key insight here is that each channel has its own content format, audience behavior, and algorithmic preference. Simply sharing a link to your blog post on LinkedIn is not distribution. Effective distribution means creating native content for each channel that stands on its own while driving traffic back to the original piece.
- **Output**: A multi-channel content package containing all derivative formats, each tailored to its destination platform. The package should include posting schedules, suggested hashtags or tags, and engagement prompts. This output transforms a single content investment into multiple touchpoints across your audience's preferred channels, dramatically increasing the content's reach and ROI.

**Layer 6: Experimentation**

- **Input**: Performance data from published and distributed content, including organic traffic, engagement metrics (time on page, scroll depth, bounce rate), conversion metrics (CTA clicks, form submissions, signups), and social engagement metrics (likes, shares, comments).
- **AI role**: Generate headline variations and CTA copy variations for A/B testing. Analyze experiment results to identify statistically significant winners and generate hypotheses for why certain variations outperform others. Recommend new experiments based on observed patterns. AI is particularly effective at generating a high volume of creative variations for testing, which is a task that humans find tedious and where cognitive biases often limit the range of ideas explored. AI can also analyze experiment results faster and with less statistical error than manual analysis.
- **Output**: Winning headline and CTA variations that replace the originals, along with documented insights about what resonates with your audience. These insights feed back to Layer 1 (Research) by informing future content prioritization and messaging strategy. For example, if experiments reveal that your audience responds strongly to "ROI calculator" CTAs but weakly to "download the guide" CTAs, that insight should shape both the content types you prioritize and the capture mechanisms you design for future content.

### Example scenario: Healthcare SaaS

A healthcare compliance SaaS company applies the AIO Content Stack to build a scalable content engine that drives qualified leads.

1. **Research**: AI ingests 2,000 keywords related to "HIPAA compliance" and clusters them into 30 topic groups based on semantic similarity and intent type. The analysis reveals that clusters around "HIPAA compliance checklist," "HIPAA training requirements," and "HIPAA violation penalties" have the highest combination of search volume and buying intent. Customer call transcript analysis reveals that compliance officers consistently describe their primary pain as "keeping up with regulatory changes," which becomes a key messaging theme.
2. **Briefs**: The team generates detailed briefs for the top 10 topics, prioritized by a composite score of traffic potential, buying intent alignment, and competitive difficulty. Each brief includes a competitive analysis showing what the top three ranking articles cover, a gap analysis identifying what they miss (for example, none of the top-ranking "HIPAA compliance checklist" articles include a downloadable, editable checklist template), and specific internal linking targets.
3. **Drafting**: AI produces first drafts for all 10 briefs in under a day. A compliance subject-matter expert reviews each draft for regulatory accuracy, correcting any inaccurate or outdated regulatory references and adding specific citations to the relevant Code of Federal Regulations sections. This expert review is critical in healthcare content, where inaccurate information can expose both the reader and the publisher to legal risk.
4. **Optimization**: Each draft is scored using an SEO content optimization tool. AI suggests internal links to the company's compliance checklist tool, its training course pages, and related blog posts. The optimizer ensures that each article uses the correct regulatory terminology and covers the NLP entities that search engines associate with authoritative HIPAA content.
5. **Distribution**: Each blog post is repurposed into a LinkedIn carousel summarizing the key compliance steps, a short email for the company's weekly compliance newsletter, and a Twitter/X thread highlighting the most surprising statistics about HIPAA violations. The LinkedIn carousels perform particularly well, generating significant engagement from the company's target audience of compliance officers and healthcare administrators.
6. **Experimentation**: A/B tests on blog CTAs reveal that "Get your free compliance audit" converts at 8.4%, which is 3x better than the original "Learn more" CTA at 2.8%. The team rolls out the winning CTA across all HIPAA-related content and applies the insight (specificity and value in CTA copy outperform generic language) to CTAs across the entire blog.

---

## 3. GEO Metrics Map

### Overview

The GEO Metrics Map organizes GTM metrics into four stages (Acquisition, Activation, Revenue, and Retention/Expansion) and clarifies which metrics matter at each stage, how to measure them, and which levers (SEO, AIO, GEO) influence each. The purpose of this framework is to eliminate the common problem of tracking too many metrics without understanding how they relate to each other or to revenue. By organizing metrics into stages that mirror the customer journey, the GEO Metrics Map helps teams focus on the metrics that matter most at their current growth stage and understand the causal relationships between leading indicators and lagging outcomes.

### When to use it

- **Setting quarterly OKRs for the GTM team.** The GEO Metrics Map provides a structured way to set goals that span the entire customer journey rather than focusing narrowly on a single stage. It ensures that OKRs are balanced: you are not setting aggressive acquisition targets without corresponding activation and retention targets. Each OKR can be tied to a specific lever (SEO, AIO, or GEO), making it clear which team owns the outcome and what actions they need to take. This prevents the common anti-pattern where an entire GTM team is accountable for a revenue target but nobody is specifically accountable for the intermediate metrics that drive it.
- **Building dashboards and reporting infrastructure.** The four-stage structure of the GEO Metrics Map translates directly into a dashboard layout. Each stage becomes a section of the dashboard, with the key metrics for that stage displayed alongside the primary levers that influence them. This structure makes it immediately clear where the GTM engine is performing well and where it needs attention. It also prevents the "dashboard sprawl" problem where teams track dozens of metrics without understanding which ones are actionable.
- **Diagnosing where the GTM engine is leaking (for example, "we get traffic but no signups").** The staged structure makes it easy to identify exactly where prospects are dropping off. By measuring the conversion rate between each stage (Acquisition → Activation → Revenue → Retention), you can pinpoint which transition is underperforming. Once you identify the leaky stage, the "primary levers" section tells you which tools and tactics to deploy to fix it. This diagnostic approach prevents the shotgun approach of trying to improve everything simultaneously, which typically improves nothing.

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

- **SEO pillar: Tools and practices for ranking and earning traffic.** The SEO pillar provides actionable guidance on technical SEO foundations (site speed, crawlability, structured data), on-page optimization (title tags, meta descriptions, heading structure, content depth), and off-page authority building (link earning strategies, digital PR, content partnerships). These tools and practices directly influence the Acquisition-stage metrics of impressions, sessions, and MQLs. Without strong SEO fundamentals, even excellent content will struggle to generate organic traffic at scale.
- **AIO pillar: Workflows for producing content that ranks at scale.** The AIO pillar addresses the content velocity challenge that most teams face. Using the AIO Content Stack (Framework 2), teams can produce high-quality, SEO-optimized content at a pace that would be impossible with purely manual processes. This directly drives the volume of ranking pages and, consequently, the volume of organic sessions and leads. The key insight is that content volume and content quality are not trade-offs when AI is applied correctly, because AI handles the volume while human editors ensure the quality.
- **Workflows: "From Zero to First 100 ICP Signups via SEO + AIO."** This specific workflow provides a step-by-step playbook for early-stage companies that are building their organic acquisition engine from scratch. It covers everything from initial keyword research and content calendar planning through content production, publication, and optimization. The workflow is designed to produce measurable results (100 ICP-qualified signups) within a defined timeframe, giving early-stage teams a concrete target and a clear path to achieving it.

**Activation**

- **GEO pillar: Onboarding and product-led growth tools.** The GEO pillar provides guidance on designing and implementing onboarding flows that drive users toward their activation moment. This includes in-product checklists, interactive tours, progress indicators, and contextual help. It also covers PLG-specific tools like usage tracking, feature adoption analytics, and automated activation triggers. These tools directly influence the Activation-stage metrics of signups, PQLs (Product-Qualified Leads), and SQLs (Sales-Qualified Leads) by ensuring that more users experience enough value to become qualified.
- **AIO pillar: AI-personalized onboarding content.** Personalized onboarding content increases activation rates by making the onboarding experience relevant to each user's specific context. The AIO pillar describes how to use AI to generate segment-specific onboarding sequences, personalized feature recommendations, and contextual help content. The expected outcome is a measurable increase in the percentage of signups who reach the activation milestone.
- **Playbooks: Early-stage and growth-stage activation plays.** These playbooks provide specific, tactical plays for improving activation rates. Early-stage plays focus on manual, high-touch approaches (for example, personal onboarding calls for the first 50 users), while growth-stage plays focus on scalable, automated approaches (for example, AI-personalized email sequences triggered by usage data). Each play includes a description of when to use it, how to implement it, and how to measure its impact.

**Revenue**

- **GEO pillar: CRM, sales enablement, and conversion optimization tools.** The GEO pillar covers the tools and workflows that directly drive Revenue-stage metrics. This includes CRM configuration and deal pipeline management, sales enablement content (battle cards, objection handlers, ROI calculators), pricing page optimization, and trial-to-paid conversion flows. Each tool is evaluated for its impact on win rate, pipeline velocity, and CAC payback period.
- **AIO pillar: AI-generated sales collateral and proposal content.** AI can dramatically accelerate the creation of customized sales materials. The AIO pillar describes workflows for generating personalized proposals, custom ROI analyses, competitive comparisons tailored to specific deals, and case study summaries matched to the prospect's industry. These materials directly influence win rate by giving sales teams better ammunition for every deal.
- **Frameworks: S2R Loop's Convert stage.** The Convert stage of the S2R Loop (Framework 1) provides the strategic context for Revenue-stage optimization. It clarifies how SEO, AIO, and GEO work together to move activated users toward a purchasing decision, and it identifies the specific tactics that are most effective at each point in the conversion process.

**Retention / Expansion**

- **GEO pillar: Lifecycle marketing, customer success, and analytics tools.** The GEO pillar addresses Retention and Expansion through lifecycle marketing automation (renewal reminders, usage milestone celebrations, expansion triggers), customer success tooling (health scores, QBR automation, risk alerts), and analytics (cohort analysis, NRR decomposition, churn prediction models). These tools directly influence NRR, LTV, churn rate, and expansion revenue by ensuring that the GTM team can proactively manage the existing customer base rather than reacting to churn after it happens.
- **AIO pillar: AI-powered customer communication and renewal content.** AI enables personalized customer communication at scale. The AIO pillar describes how to use AI to generate customized QBR decks, renewal proposals that highlight specific value delivered, usage reports that demonstrate ROI, and feature adoption recommendations based on the customer's usage patterns. This content directly supports retention and expansion by continually reinforcing the value the customer receives.
- **Frameworks: S2R Loop's Expand stage and feedback loop.** The Expand stage and feedback loop of the S2R Loop provide the strategic context for Retention and Expansion optimization. The feedback loop is particularly important here, as it shows how expansion patterns and customer behavior data should flow back into the Discover stage to attract more customers with similar high-expansion-potential profiles.

### Example scenario: Developer tools startup

A Series A developer tools company uses the GEO Metrics Map to set balanced quarterly OKRs that span the entire customer journey. Each OKR is tied to a specific lever, making accountability clear and ensuring that the team invests in all four stages rather than over-indexing on acquisition at the expense of activation and retention.

| Stage | Metric | Target | Lever |
|---|---|---|---|
| Acquisition | Organic sessions | 50K/mo → 80K/mo | SEO content + AIO drafting |
| Activation | Signup → first project | 30% → 40% | GEO onboarding flow redesign |
| Revenue | Free-to-paid conversion | 5% → 7% | GEO pricing page experiment |
| Retention | Monthly active usage | 60% → 70% | AIO in-product help content |

Each target is chosen based on benchmarking against comparable developer tools companies at a similar stage. The Acquisition target of 80K organic sessions per month requires approximately 50 new ranking pages, which the team plans to produce using the AIO Content Stack at a rate of 12 to 15 pieces per month. The Activation target of 40% signup-to-first-project conversion requires a redesign of the onboarding flow, specifically reducing the number of steps between signup and first project creation from seven to three. The Revenue target of 7% free-to-paid conversion requires A/B testing the pricing page, including testing a lower-priced entry tier and adding social proof from existing customers. The Retention target of 70% monthly active usage requires building an in-product help system powered by AI that surfaces contextual tips and documentation when users appear stuck.

---

## 4. Signals > Channels > Plays (Optional Model)

### Overview

A lightweight planning model for GTM teams that prefer to think in terms of market signals rather than funnel stages. The Signals > Channels > Plays model starts with what you observe in the market, identifies the channels where those signals are actionable, and prescribes specific plays to execute. This model is particularly effective for teams that operate in fast-moving markets where conditions change frequently, because it is inherently reactive and adaptive. Rather than committing to a long-term funnel strategy and executing it regardless of market conditions, this model encourages continuous scanning for signals and rapid response. It complements the S2R Loop rather than replacing it: the S2R Loop provides the long-term architecture, while Signals > Channels > Plays provides the short-term agility.

### When to use it

- **When the S2R Loop feels too linear for your business.** Some businesses, particularly those with multiple products, diverse buyer personas, or complex buying committees, find that a linear stage model does not adequately capture how their customers actually buy. The Signals > Channels > Plays model removes the requirement for linearity and instead focuses on responding to whatever signals are most important right now. This makes it a better fit for businesses where the buyer journey is non-linear, where multiple stakeholders enter the journey at different stages, or where external events (competitive moves, regulatory changes, seasonal trends) drive GTM activity more than internal funnel metrics.
- **When your GTM motion is event-driven or signal-driven (for example, product-led growth).** PLG companies often find that their most effective GTM motions are triggered by product usage signals rather than marketing funnel stages. For example, a user hitting a usage limit, inviting a teammate, or achieving a milestone are all signals that should trigger specific plays. The Signals > Channels > Plays model provides a natural framework for organizing these event-driven motions. It is also well-suited for companies that rely heavily on competitive intelligence, where a competitor's product launch or pricing change triggers a rapid content response.
- **When planning short-term sprints rather than long-term strategy.** The model is ideal for two-week or monthly GTM sprints. At the start of each sprint, the team scans for the strongest current signals, selects the channels best suited to act on those signals, and commits to a set of plays that can be executed within the sprint. This cadence ensures that GTM activity is always responsive to current conditions rather than following a plan that was set months ago and may no longer be relevant. The sprint format also creates natural checkpoints for evaluating what worked and adjusting strategy accordingly.

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

### Signal types in detail

Understanding the types of signals you should monitor is essential for making this model work effectively. Each signal type has different characteristics, different data sources, and different response timeframes.

- **Rising search volume for a category term.** Monitor tools like Google Trends, Ahrefs, and SEMrush for increases in search volume around keywords relevant to your category. A sustained volume increase (not just a spike) indicates growing market interest and an opportunity to capture traffic before competitors respond. The response timeframe for this signal is typically two to eight weeks, since content needs to be produced and indexed before the traffic opportunity fully materializes.
- **Competitor launches a new feature.** Monitor competitor blogs, product changelogs, press releases, and social media for feature announcements. A competitor feature launch creates an immediate opportunity to publish comparison content, update your positioning, and proactively address the competitive narrative before your prospects encounter it during their evaluation process. The response timeframe is typically one to three days for initial messaging (social posts, email to pipeline prospects) and one to two weeks for deeper content (comparison pages, competitive battle cards).
- **Customer churn spike in a segment.** Monitor your churn data by segment (industry, company size, use case, cohort) for unusual increases. A churn spike in a specific segment signals a systemic problem that needs to be addressed both reactively (re-engage the churning customers) and proactively (prevent similar customers from churning). The response timeframe is immediate for the re-engagement campaign and one to four weeks for root cause analysis and structural fixes.
- **Product usage milestone reached.** Monitor your product analytics for users or accounts reaching significant milestones (first project created, tenth active user added, 100th API call made). These milestones are opportunities to reinforce the user's positive momentum with congratulatory messaging, feature recommendations, and expansion offers. The response timeframe should be automated and real-time, since the impact of milestone messaging decreases rapidly if delayed.
- **Seasonal demand pattern.** Monitor your historical traffic and pipeline data for seasonal patterns (for example, Q1 budget planning cycles, annual compliance renewal periods, back-to-school demand). Seasonal patterns are the most predictable signal type and should be addressed proactively by publishing relevant content and launching campaigns well before the demand spike begins. The response timeframe is four to eight weeks before the anticipated demand increase.

### Channel selection criteria

Not every signal warrants action on every channel. Choosing the right channels for each signal is critical for efficient resource allocation. Consider the following criteria when selecting channels.

- **Audience alignment.** Choose channels where the audience affected by the signal is most active. If the signal is rising search volume, organic search (SEO) is the natural channel. If the signal is a churn spike, email and in-product messaging are more appropriate.
- **Speed-to-market.** Some channels are faster to activate than others. Social media and email can be activated within hours. Organic search content takes weeks to produce and rank. Match the channel's speed to the urgency of the signal.
- **Measurability.** Choose channels where you can clearly measure the impact of your play. If you cannot measure whether the play worked, you cannot learn from it and improve your signal-response process over time.

### Example: Signal-driven sprint

**Signal**: Google Trends shows "AI compliance tools" queries up 200% this quarter. Keyword research confirms that monthly search volume for the cluster has grown from 2,400 to 7,200 searches per month, with the majority of queries being informational ("what are AI compliance requirements") and commercial ("best AI compliance tools"). Competitive analysis reveals that only two of the top ten ranking pages have been updated in the past six months, indicating an opportunity to capture rankings with fresh, comprehensive content.

**Channels selected**: Organic search (to capture the growing search volume), AI-generated content (to produce articles quickly enough to capitalize on the trend), and email (to nurture the leads generated from the content).

**Plays executed**:

1. **Content production.** Use the AIO Content Stack (Layers 1 through 4) to research the "AI compliance" keyword cluster, generate briefs for the top five topics by volume and intent, produce AI-drafted articles with human expert review for regulatory accuracy, and optimize each article for on-page SEO. Target turnaround: 10 business days from signal detection to publication.
2. **Lead capture asset.** Build a gated "AI Compliance Checklist" as a lead capture asset. The checklist should be genuinely useful (covering the specific regulatory requirements, technical controls, and documentation needed for AI compliance) so that it provides immediate value in exchange for an email address. Embed the checklist CTA within each of the five published articles and on a dedicated landing page.
3. **Email nurture sequence.** Launch a five-email nurture sequence for leads captured from the checklist. The sequence should educate the lead about AI compliance requirements (emails one and two), demonstrate how your product addresses those requirements (emails three and four), and offer a personalized demo or consultation (email five). Each email should be segmented by the lead's industry if that data is available from form fields or enrichment.
4. **Lead enrichment and routing.** Enrich captured leads with firmographic data (company size, industry, technology stack) using tools like Clearbit or ZoomInfo. Apply lead scoring criteria to identify enterprise prospects (more than 500 employees, regulated industries, existing compliance budgets) and route them to sales for immediate outreach. Smaller accounts remain in the automated nurture sequence.
5. **Measurement and feedback.** Track the full funnel from signal to revenue: impressions → sessions → checklist downloads → email engagement → SQLs → pipeline → closed revenue. Set specific targets for each metric (for example, 5,000 sessions in month one, 250 checklist downloads, 50 MQLs, 10 SQLs, 3 opportunities). Review results at the end of the sprint and feed learnings back into the next sprint's signal scanning and play selection.
