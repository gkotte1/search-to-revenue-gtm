# Contributing to search-to-revenue-gtm

Thanks for your interest in making this resource better. This repo thrives on contributions from GTM practitioners who work at the intersection of search, AI, and growth every day.

## What We Accept

| Contribution type | Where it goes | How to submit |
|---|---|---|
| New tool | `data/tools-*.json` | Pull request |
| New framework | `docs/frameworks.md` | Pull request |
| New workflow | `docs/workflows.md` | Pull request |
| New playbook | `docs/playbooks.md` | Pull request |
| New example | `docs/examples.md` | Pull request |
| Correction or update | Any file | Pull request or issue |
| Idea or discussion | N/A | Issue |

## Adding a New Tool

All tools live in the `/data` directory as JSON arrays. Before submitting, check that:

1. **The tool is not already listed.** Search across all three JSON files.
2. **You use the correct file.** SEO tools go in `tools-seo.json`, AI/AIO tools in `tools-aio.json`, growth/GEO tools in `tools-geo.json`. If a tool spans categories, pick the primary one.
3. **Your entry follows the schema exactly:**

```json
{
  "name": "Tool Name",
  "website": "https://example.com",
  "category": "short-tag",
  "summary": "1-2 sentence practical description focused on GTM outcomes.",
  "gtm_use_cases": [
    "Specific GTM use case 1",
    "Specific GTM use case 2"
  ],
  "pricing_model": "free | freemium | paid",
  "best_for_stage": ["early", "growth", "enterprise"]
}
```

### Schema rules

- `name`: Official product name. No taglines.
- `website`: Primary marketing or docs URL. No affiliate links.
- `category`: A short, lowercase tag (e.g., `keyword-research`, `content-optimization`, `analytics`, `crm`, `experimentation`).
- `summary`: Describe what a GTM team actually gets from this tool. Avoid "powerful," "best-in-class," "revolutionary." Be specific.
- `gtm_use_cases`: 1-4 concrete use cases. Each should describe an action a GTM team would take (e.g., "Identify high-intent keywords for bottom-of-funnel landing pages").
- `pricing_model`: One of `free`, `freemium`, or `paid`.
- `best_for_stage`: Array containing one or more of `early`, `growth`, `enterprise`.

### Example of a good entry

```json
{
  "name": "Screaming Frog",
  "website": "https://www.screamingfrog.co.uk/seo-spider/",
  "category": "technical-seo",
  "summary": "Desktop-based site crawler that surfaces indexability issues, broken links, and redirect chains. The free tier crawls up to 500 URLs, making it practical for early-stage audits.",
  "gtm_use_cases": [
    "Audit technical SEO health before a site relaunch",
    "Identify crawl-budget waste on large content sites",
    "Generate XML sitemaps for programmatic page sets"
  ],
  "pricing_model": "freemium",
  "best_for_stage": ["early", "growth", "enterprise"]
}
```

### Example of a bad entry

```json
{
  "name": "CoolSEOTool",
  "website": "https://affiliate.link/coolseotool",
  "category": "seo",
  "summary": "The best SEO tool on the market. 10x your traffic!",
  "gtm_use_cases": ["SEO"],
  "pricing_model": "paid",
  "best_for_stage": ["early"]
}
```

Problems: affiliate link, hypey summary, vague use case, overly broad category.

## Adding Frameworks, Workflows, or Playbooks

1. Open a GitHub Issue first to discuss the idea. Describe the framework/workflow/playbook, the GTM problem it solves, and a rough outline.
2. Once there is maintainer agreement, submit a PR with the content added to the appropriate doc in `/docs`.
3. Follow the existing structure in each doc (headings, subsections, bullet points).

## Style Guidelines

- **Be specific.** "Increase MQL-to-SQL conversion by aligning landing page messaging with search intent" is better than "improve conversions."
- **Be practical.** Describe what a team does, not abstract theory.
- **No sales language.** This repo is a reference, not a pitch deck.
- **No affiliate links.** Ever.
- **No self-promotion without substance.** If you built a tool, you can add it, but the entry must meet the same quality bar as everything else.
- **Use plain English.** Avoid jargon that only makes sense inside one company's culture.

## Pull Request Process

1. Fork the repo and create a feature branch.
2. Make your changes.
3. Ensure JSON files are valid (the CI workflow will check automatically).
4. Submit a PR with a clear description of what you added or changed and why.
5. A maintainer will review your PR. We may suggest edits for clarity, tone, or accuracy. This is collaborative, not adversarial.

## Code of Conduct

All contributors are expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md). Be respectful, be constructive, and focus on making this resource genuinely useful.
