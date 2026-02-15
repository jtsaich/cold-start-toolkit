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

## Installation

This plugin is located at `/Users/crow/Documents/claude/cold-start/`. To use it, ensure Claude Code can discover plugins in this directory.

## Research Foundation

This toolkit was designed based on comprehensive research documented in:

- `cold-start-research/01-platform-catalog.md` — Platform scores, free tiers, MCP availability
- `cold-start-research/02-validation-strategies.md` — Category rankings, validation playbooks
- `cold-start-research/03-automation-boundaries.md` — 5-tier automation map, handoff protocols
- `cold-start-research/04-system-architecture.md` — Full architecture, templates, user journey
