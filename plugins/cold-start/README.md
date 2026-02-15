# Cold-Start Toolkit

A Claude Code plugin that takes a business idea from zero to validated online presence in ~2 weeks. Five specialized AI agents coordinate to automate ~75% of the work — market research, brand generation, code scaffolding, content creation, and deployment — while guiding the founder through the remaining 25% with structured handoff protocols.

## Quick Start

```
/cold-start A newsletter about AI tools
```

Or just:

```
/cold-start
```

The toolkit will ask you to describe your idea.

## What It Does

1. **Intake Interview** — 10 questions to understand your idea, audience, budget, and goals
2. **Market Research** — Competitor analysis, keyword research, Reddit sentiment mining, Google Trends, market sizing (all automated)
3. **Brand Generation** — Name candidates with domain/social availability, color palettes with WCAG validation, typography, complete design system
4. **Code Generation** — Full Next.js application from 7 templates, deployed to Vercel
5. **Content Creation** — 30-day content calendar, 5-email welcome sequence, SEO blog posts, social media bios, ad copy
6. **Human Handoffs** — Step-by-step guides for tasks only humans can do (account creation, identity verification), batched to minimize time
7. **Validation Report** — Scorecard across 6 dimensions with a data-driven Persevere/Pivot/Kill recommendation

## Agents

| Agent | Model | Role |
|-------|-------|------|
| **Orchestrator** | Opus | Conducts intake, classifies business, coordinates all agents, generates validation report |
| **Researcher** | Opus | Market research (5 parallel tracks), brand name generation, design system creation |
| **Builder** | Sonnet | Code generation from 7 templates, database setup, auth/payments/email/analytics configuration |
| **Marketer** | Sonnet | Content calendar, email sequences, blog posts, social media content, ad copy, validation tracking |
| **Guide** | Haiku | Human handoff instructions, credential validation, progress dashboard, troubleshooting |

## Business Categories Supported

| Category | Automation Level | Best For |
|----------|-----------------|----------|
| Newsletter/Content | 90% | Fastest validation, $0 to start |
| Personal Tools & Utilities | 85% | Quick build, easy to test |
| Digital Products | 80% | Pre-sell before you build |
| SaaS Micro-Tools | 75% | Full-stack app with freemium |
| Community/Membership | 60% | Waitlist + Discord setup |
| Service Businesses | 55% | Portfolio + booking site |
| E-commerce/Dropshipping | 50% | Product showcase + checkout |
| B2B SaaS | 40% | Landing page + demo booking |
| Marketplace | 35% | Waitlist validation first |
| Mobile Apps | 30% | Web prototype validation |
| Hardware/Physical | 15% | Crowdfunding landing page |

## Templates

1. **Waitlist Landing Page** — Email capture with referral system
2. **Product Showcase** — Features, pricing tiers, Stripe Checkout
3. **Newsletter / Content Hub** — Subscribe form + issue archive
4. **SaaS Micro-Tool** — Auth, dashboard, freemium with Stripe
5. **Digital Product Store** — Product grid, checkout, secure downloads
6. **Service Business** — Portfolio, services, booking, contact form
7. **Community Landing** — Join form, benefits, Discord integration

## Default Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Next.js 15 + TypeScript |
| Styling | Tailwind CSS + shadcn/ui |
| Hosting | Vercel |
| Database | Supabase |
| Auth | Supabase Auth |
| Payments | Stripe |
| Email | Resend + React Email |
| Analytics | PostHog |

All free tier. $0/month to start.

## Output Structure

```
cold-start-output/{project-name}/
├── research/              # Market research reports
├── brand/                 # Name, design system, Tailwind config
├── src/                   # Complete deployable Next.js app
├── content/               # Calendar, emails, blog posts, social
│   ├── emails/
│   └── blog/
└── reports/               # Progress dashboard, handoff guides, validation report
```

## Human Time Required

| Phase | Time | When |
|-------|------|------|
| Intake interview | 10 min | Start |
| Brand selection | 15 min | After research |
| Account signups (Batch 1) | 28 min | During build |
| Service setup (Batch 2) | 45 min | Mid-build |
| Content review | 15 min | Pre-launch |
| Social media setup (Batch 3) | 30 min | Pre-launch |
| **Total** | **~2.5 hours** | **Spread over 2 weeks** |

## Example Use Cases

### Example 1: "AI Tool Digest" — Newsletter/Content

**Command:**
```
/cold-start A weekly newsletter curating the best new AI tools with reviews
```

**What gets generated:**
- **Research:** 15 competitor newsletters analyzed, keyword clusters (AI tools, no-code, productivity), Reddit sentiment from r/artificial and r/SideProject, TAM estimate for AI newsletter market
- **Brand:** 5 name candidates with .com availability check, tech-forward color palette (electric blue + slate), Inter/JetBrains Mono typography, minimal logo concepts
- **Code:** Newsletter Hub template — subscribe form with double opt-in, issue archive page, referral tracking, RSS feed, deployed to Vercel
- **Content:** 30-day content calendar, 5-email welcome sequence, 3 SEO blog posts ("Best AI Tools This Week" format), Twitter/LinkedIn bios, first issue draft
- **Handoffs:** Create Beehiiv account, connect custom domain, set up Resend API key, claim social handles

**Expected validation (Day 14):**
250+ subscribers, 45% open rate, 12% click rate, 3 referral signups. PKP recommendation: **Persevere** — strong engagement signals with $0 operating cost.

---

### Example 2: "StatusPing" — SaaS Micro-Tool

**Command:**
```
/cold-start A simple uptime monitor that pings URLs and sends alerts
```

**What gets generated:**
- **Research:** 20 competitors mapped (UptimeRobot, Better Stack, Pingdom), pricing gap analysis, keyword research for "free uptime monitor", Indie Hacker sentiment analysis, market sizing ($2.1B monitoring market)
- **Brand:** 5 name candidates with domain check, status-green color palette with red/amber alerts, system-font stack for dashboard clarity, monitoring-themed design system
- **Code:** SaaS Micro-Tool template — Supabase Auth (magic link + GitHub OAuth), dashboard with URL list and status history, cron-based ping worker, Stripe freemium (5 free URLs / 50 paid), PostHog analytics, deployed to Vercel
- **Content:** 30-day launch calendar, 5-email onboarding sequence, 3 SEO posts ("UptimeRobot Alternative" angle), Product Hunt draft, changelog page
- **Handoffs:** Create Supabase project, configure Stripe products and pricing, set up PostHog project, register for Vercel cron

**Expected validation (Day 14):**
40 signups, 15 active monitors, 2 paid conversions ($9.99/mo each). PKP recommendation: **Persevere** — early paid conversion validates willingness to pay.

---

### Example 3: "The Notion Startup Kit" — Digital Products

**Command:**
```
/cold-start A Notion template pack for startup founders doing fundraising
```

**What gets generated:**
- **Research:** Top 30 Notion templates on Gumroad/Lemon Squeezy analyzed, pricing benchmarks ($19-$49 range), keyword research for "startup Notion template", founder community sentiment, TAM for digital productivity tools
- **Brand:** 5 name candidates, warm-professional palette (amber + charcoal), clean typography, product mockup guidelines for marketplace listings
- **Code:** Digital Product Store template — product grid with preview images, Lemon Squeezy checkout integration, secure download delivery, lead magnet landing page (free "Pitch Deck Tracker" template), email capture funnel, deployed to Vercel
- **Content:** 30-day content calendar focused on founder Twitter, 5-email nurture sequence, 3 SEO posts ("Fundraising Tracker" tutorials), Lemon Squeezy product descriptions, social proof section template
- **Handoffs:** Create Lemon Squeezy account, upload Notion templates as products, set up lead magnet delivery, post in r/Notion and Indie Hackers

**Expected validation (Day 14):**
200 email signups from lead magnet, 15 paid sales ($29 avg), 85% delivery rate. PKP recommendation: **Persevere** — pre-sell revenue proves demand before building full pack.

---

### Example 4: "BrandForge" — Service Business

**Command:**
```
/cold-start A freelance brand design agency for early-stage startups
```

**What gets generated:**
- **Research:** 25 freelance design agencies analyzed, pricing benchmarks ($500-$5K per project), keyword research for "startup branding agency", Dribbble/Behance trend analysis, ICP definition (funded pre-seed founders)
- **Brand:** 5 name candidates, creative-bold palette (violet + gold accents), display + body font pairing, portfolio-optimized design system
- **Code:** Service Business template — portfolio grid with case study pages, services/pricing page, Cal.com booking integration, contact form with Resend notifications, testimonial carousel, deployed to Vercel
- **Content:** 30-day content calendar (before/after portfolio posts), 5-email inquiry sequence, 3 SEO posts ("Brand Identity Checklist for Startups"), LinkedIn outreach templates, proposal template
- **Handoffs:** Create Cal.com account and set availability, set up CRM (Notion or HubSpot free), join startup Slack communities, create Dribbble profile

**Expected validation (Day 14):**
8 discovery calls booked, 2 proposals sent, 1 signed client ($1,500 project). PKP recommendation: **Persevere** — single client covers months of operating cost, refine positioning.

---

### Example 5: "DevChat" — Community/Membership

**Command:**
```
/cold-start A paid community for developers learning AI agent development
```

**What gets generated:**
- **Research:** 15 dev communities analyzed (Key Values, Indie Hackers, Lenny's), pricing benchmarks ($20-$50/mo), keyword research for "AI agents community", Twitter/Reddit sentiment for "learn AI agents", market timing analysis
- **Brand:** 5 name candidates with domain check, dev-dark palette (deep navy + neon green accents), monospace-forward typography, community badge/avatar system concepts
- **Code:** Community Landing template — benefits showcase, member count/social proof, Discord OAuth join flow, waitlist with referral tracking, Stripe subscription ($29/mo), FAQ section, deployed to Vercel
- **Content:** 30-day content calendar (Twitter threads on AI agents), 5-email waitlist nurture sequence, 3 SEO posts ("How to Build AI Agents" tutorials), Discord channel structure plan, welcome guide draft
- **Handoffs:** Create Discord server with role structure, configure Stripe subscription product, set up Discord bot for role assignment on payment, seed initial content in 3 channels

**Expected validation (Day 14):**
150 waitlist signups, 35% email open rate, 12 founding members ($29/mo = $348 MRR). PKP recommendation: **Persevere** — founding member cohort validates pricing, focus on retention and content cadence.

## Installation

This plugin is located at `/Users/crow/Documents/claude/cold-start/`. To use it, ensure Claude Code can discover plugins in this directory.

## Research Foundation

This toolkit was designed based on comprehensive research documented in:

- `cold-start-research/01-platform-catalog.md` — Platform scores, free tiers, MCP availability
- `cold-start-research/02-validation-strategies.md` — Category rankings, validation playbooks
- `cold-start-research/03-automation-boundaries.md` — 5-tier automation map, handoff protocols
- `cold-start-research/04-system-architecture.md` — Full architecture, templates, user journey
