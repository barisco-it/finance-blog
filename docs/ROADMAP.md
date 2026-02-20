# Finance Blog – Product Roadmap

This is a structured passion project.

Goals:
- Build a clean, SEO-first personal finance blog
- Maintain professional engineering discipline
- Avoid unnecessary complexity
- Ship small, stable increments
- Focus on long-term consistency over speed

---

## Guiding Principles

- Keep architecture simple
- No premature optimization
- No unnecessary dependencies
- One feature at a time
- Discovery before implementation
- Build must always pass
- Publish consistently

---

## Phase 0 – Discovery & Positioning

Objective: Define direction before writing code.

### 0.1 Benchmark Analysis
- Analyze 5 finance blogs (TR + Global)
- Compare layout, structure, tone
- Identify differentiation opportunities

Deliverable:
- `/docs/benchmark.md`

### 0.2 Positioning Definition
- Target reader
- Tone (analytical / educational / opinionated)
- Depth level (beginner / intermediate / advanced)
- Core themes (max 5 pillars)

Deliverable:
- `/docs/positioning.md`

### 0.3 Taxonomy Design
- Define tag system (max 10–15 tags)
- URL structure for tags
- Slug conventions

Deliverable:
- `/docs/taxonomy.md`

Exit Criteria:
- Clear blog identity
- Clear topic boundaries
- Defined content structure

---

## Phase 1 – Foundation (MVP)

Objective: Launch a stable, SEO-ready blog.

### 1.1 Core Setup
- Initialize Next.js
- Configure MDX content system
- Add Tailwind (optional)
- Base layout (header + footer)

### 1.2 Blog System
- `/blog` listing page
- `/blog/[slug]` post page
- Posts sorted by date (desc)
- MDX frontmatter support

### 1.3 Tags
- Tag pages (`/tags/[tag]`)
- Posts linked to tags

### 1.4 Legal & Trust
- Disclaimer page
- About page
- Footer links

### 1.5 SEO Baseline
- Meta titles + descriptions
- OpenGraph tags
- robots.txt
- sitemap.xml

Exit Criteria:
- Deployed to Vercel
- Clean production build
- Mobile responsive
- 3 published posts

---

## Phase 2 – Credibility & Distribution

Objective: Improve discoverability and authority.

- RSS feed
- Google Search Console setup
- Lightweight analytics (privacy-friendly)
- Performance optimization (images, fonts)

Exit Criteria:
- Indexed on Google
- Analytics active
- Core Web Vitals acceptable

---

## Phase 3 – Value Add Features (Optional)

Objective: Add small tools after the blog is stable.

- Compound interest calculator
- Inflation-adjusted returns calculator
- ETF comparison tables (lightweight)

Exit Criteria:
- Tools add clear reader value
- No architecture complexity spiral

---

## Content Strategy

Initial 5 article targets:
- Long-term investing basics
- Inflation-adjusted returns explained
- ETF basics
- Risk vs return (practical)
- Turkey vs global diversification

Cadence:
- Target 1 post/week (quality over quantity)

---

## Technical Governance Rules

- No new npm package without justification
- No architecture refactors during feature implementation
- Always pass:
  - lint
  - build
- Small changes only (reviewable diffs)
- One feature in progress at a time
