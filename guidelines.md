# SEO Knowledge Base — AEO / GEO / AI Search Guidelines

This file is updated weekly by an automated research agent. The most recent findings appear at the top.

---

## Update: 2026-05-10

### Sources Reviewed
- [Neil Patel — GEO vs AEO: What's the Difference?](https://neilpatel.com/blog/geo-vs-aeo/) — Breaks down AEO (direct answers / featured snippets) vs GEO (AI-generated citations), and why both matter in 2026
- [Neil Patel — AEO vs GEO vs LLMO: Are They All SEO?](https://neilpatel.com/blog/aeo-vs-geo-vs-llmo/) — Argues that structure and citations now outweigh thoroughness and backlink volume for AI visibility
- [HubSpot — AEO Best Practices Marketing Teams Can't Ignore](https://blog.hubspot.com/marketing/answer-engine-optimization-best-practices) — Covers content chunking, schema, entity consistency, and citation density benchmarks
- [HubSpot — Answer Engine Optimization Trends 2026](https://blog.hubspot.com/marketing/answer-engine-optimization-trends) — AI-surfaced URLs average 1,064 days old vs 1,432 for traditional search; freshness is a relative advantage
- [ALM Corp — AEO 2026 Playbook for Google AI Overviews, ChatGPT, Perplexity, Claude](https://almcorp.com/blog/answer-engine-optimization-2026/) — Platform-specific tactics across the four major AI answer engines
- [Search Engine Journal — Which Content Formats Earn AI Citations in 2026 (Webinar)](https://www.searchenginejournal.com/aeo-in-2026-which-content-formats-earn-ai-citations-how-to-produce-more-webinar/572870/) — Empirical breakdown of content types most frequently cited by LLMs
- [Search Engine Land — Mastering GEO in 2026: Full Guide](https://searchengineland.com/mastering-generative-engine-optimization-in-2026-full-guide-469142) — End-to-end GEO strategy including llms.txt, AI crawler access, and author credentialing
- [Frase.io — Complete AEO Guide 2026](https://www.frase.io/blog/what-is-answer-engine-optimization-the-complete-guide-to-getting-cited-by-ai) — Deep dive on FAQPage schema, inverted-pyramid writing, and section-length benchmarks
- [Elsner — GEO vs AEO vs SEO Comparison Guide 2026](https://www.elsner.com/geo-vs-aeo-vs-seo-comparison-guide/) — Strategic budget allocation framework (30–40% to GEO) and channel ROI data
- [Semrush — How to Optimize Content for AI Search Engines 2026](https://www.semrush.com/blog/how-to-optimize-content-for-ai-search-engines/) — Structured data, AI crawler permissions, and citation surface area tactics
- [Enrich Labs — GEO Complete Guide 2026](https://www.enrichlabs.ai/blog/generative-engine-optimization-geo-complete-guide-2026) — Named-author requirements, llms.txt implementation, and content freshness signals
- [TrySight — AI Model Citation Optimization: Complete 2026 Guide](https://www.trysight.ai/blog/ai-model-citation-optimization) — Data point density, extractable tables, and section-structure benchmarks for LLM citation

### Key AEO/GEO/AI Search Guidelines

#### Content Formatting for AI Citations
- Open every page with a direct two-sentence answer in the first 100 words — LLMs extract opening chunks first and use them as candidate answer snippets
- Keep body sections between 120–180 words between H2/H3 headings; empirically, pages in this range receive ~70% more ChatGPT citations than fragmented or wall-of-text pages
- Use an inverted-pyramid structure — answer first, supporting detail after — in every section, not just introductions
- Maintain a citation density of 2–3 data points (statistics, studies, specific claims with sources) per 300 words to signal factual credibility to AI retrievers
- Include at least one FAQ block, one comparison table, or one numbered how-to list per major content piece to expand citation surface area
- Use H2 and H3 subheadings that summarize the section's takeaway rather than vague labels (e.g. "FAQ Schema Boosts AI Pickup 23%" not "Schema Tips")
- Write in a conversational, natural tone that mirrors how real people phrase questions — avoid keyword-stuffed headings and dense jargon

#### Schema Markup for AEO/GEO
- Implement **FAQPage schema** on all FAQ sections — this is the single highest-impact AEO optimization because AI engines can directly extract structured Q&A pairs
- Add **HowTo schema** to all step-by-step guides; numbered steps with clear `name` and `text` fields are pulled verbatim into AI Overviews
- Use **Article / BlogPosting schema** with explicit `author`, `datePublished`, `dateModified`, and `about` fields on every article page
- Deploy **Organization schema** on the homepage/about page with consistent `name`, `url`, `logo`, and `sameAs` (social profiles) to build entity recognition
- Add **Speakable schema** to paragraphs specifically crafted for voice assistant retrieval
- Use **BreadcrumbList schema** to signal topical hierarchy and help AI engines understand site structure

#### Topical Authority and Internal Linking
- Build content clusters: one comprehensive pillar page per core topic, supported by 5–10 narrowly focused subtopic articles that all internally link back to the pillar
- Replace anonymous "Content Team" bylines with named, credentialed authors — anonymous authorship is treated as a GEO penalty by major LLMs
- Ensure each author has a verifiable external presence (LinkedIn, author profiles on authoritative sites, published bylines elsewhere) so AI models can resolve the entity
- Maintain consistent entity representation across the web — brand name, author names, and product names should appear identically on your site, Google Business Profile, Wikipedia, Wikidata, and major directories
- Prioritize earning citations and backlinks from high-authority domains; traditional link authority remains a prerequisite for AI inclusion, not a replacement concern

#### Google AI Overviews (AIO) Optimization
- Target AIO-eligible query types: "what is," "how to," and "X vs Y" comparison queries — these trigger AI Overviews in ~15–25% of all searches as of Q2 2026
- Structure content as comprehensive how-to guides with clear numbered steps, definition-first "what is" articles, and comparison sections with explicit pros/cons tables
- Apply EEAT signals rigorously: detailed author bios with credentials, external citations for factual claims, factual accuracy reviewed and dated, and backlinks from authoritative domains
- Keep content updated — add a visible `Last updated: [date]` to pages; AI Overviews weight recency when multiple sources cover the same topic

#### Perplexity / ChatGPT / Claude Optimization
- Audit `robots.txt` to ensure AI crawlers are **not** blocked: whitelist `GPTBot`, `ClaudeBot`, `PerplexityBot`, `Googlebot-Extended`, and `anthropic-ai`
- Create an `llms.txt` file in the site root to guide AI systems on how to interpret and prioritize site content (analogous to `robots.txt` for LLMs)
- Structure content around quotable data points, clear single-sentence definitions, and extractable tables — these are cited more often than higher-authority pages lacking that structure
- Use clear alt text on images and diagrams; AI parsers index alt text as structured content and include it in citation decisions

#### New Ranking Factors Identified This Week
- **llms.txt** — A new voluntary standard (analogous to robots.txt) that signals to AI engines which pages are authoritative and how to crawl them; early adopters are seeing measurably higher citation rates
- **Author entity authority** — Named authors with verifiable profiles now function as a standalone ranking signal in AI citation models, separate from domain authority
- **Sentiment and tone scoring** — At least one major LLM (reported via Patel's analysis) now weights positive, clear, and helpful tone as a ranking input, down-weighting overly promotional or hedge-heavy copy
- **Section-length calibration** — The 120–180 word "chunk size" between headings has emerged as a practical benchmark for LLM retrieval optimization, distinct from traditional SEO readability guidelines
- **AI crawler access parity** — Sites blocking any major AI crawler (GPTBot, ClaudeBot, PerplexityBot) are seeing citation share decline across all AI platforms, not just the blocked one

### Notable Insight This Week

The most important finding from this week's research is the emergence of **author entity authority** as a first-class ranking signal in AI citation models. Multiple sources — including Neil Patel's analysis, Search Engine Land's GEO guide, and Enrich Labs — independently confirm that LLMs are now using named author credentials as a content quality proxy. Pages with anonymous bylines ("Content Team," "Staff Writer," or no attribution) are being systematically down-ranked in AI-generated citations even when the underlying domain authority is strong. The practical implication is that publishing workflows need to change immediately: every piece of content targeting AI citation should carry a real author name, link to an author bio with verifiable credentials, and that author should have an external presence (LinkedIn, published bylines, etc.) that AI models can resolve to a known entity. This is a fundamentally different trust signal from traditional E-A-T and cannot be addressed by technical SEO alone — it requires editorial policy changes.

---
