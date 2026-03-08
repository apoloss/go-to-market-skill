# Go-To-Market Strategy Skill

A [Claude Code](https://claude.com/claude-code) skill that builds comprehensive, data-driven Go-To-Market strategies for any business type.

## What it does

This skill guides you through a structured conversation to produce a complete GTM strategy document with:

- **Revenue model** with full funnel math (TAM → installs → activation → conversion → MRR)
- **Paid channel plans** for Google Ads, Meta Ads, Apple Search Ads, TikTok Ads — each with CPI benchmarks, keyword/audience targeting, creative strategy, and budget projections
- **Ad account warm-up protocols** for new accounts on every major platform — budget ramp schedules, learning phase management, and pre-launch checklists
- **Organic channels** — social media content strategy, ASO, viral/referral loops, influencer playbook, SEO
- **Phased timeline** (typically 12 months in 3-4 phases) with specific milestones and budget allocation
- **KPI framework** — acquisition, retention, conversion, and revenue metrics by phase with tracking tool recommendations
- **Risk analysis** — 8-12 risks with probability, impact, and mitigation plans
- **Complete budget** — by channel, by phase, plus operational costs and payback period

## Install

```bash
npx skills add apoloss/go-to-market-skill
```

Or install globally (available across all projects):

```bash
npx skills add apoloss/go-to-market-skill -g
```

## Usage

Once installed, start a conversation with Claude Code and describe your business:

```
I'm building a SaaS for restaurant inventory management.
I want to reach $50K ARR in 12 months. Help me build a GTM strategy.
```

The skill will:

1. Ask you targeted questions about your product, market, competition, pricing, and resources
2. Build each section of the strategy with you, presenting it for feedback
3. Output the final document as `gtm-strategy.md` plus optional companion docs (`pricing-model.md`, `competitive-analysis.md`)

## Adapts to your business

The strategy adapts based on business type:

| Type | Focus areas |
|------|-------------|
| **Mobile app** | CPI, ASO, app install campaigns, retention metrics, viral loops |
| **SaaS / Web** | CAC, SEO, content marketing, trial-to-paid, sales pipeline |
| **Marketplace** | Supply/demand balance, liquidity, chicken-and-egg problem |
| **Physical product** | Distribution channels, margins, inventory, retail partnerships |
| **Services** | Lead generation, sales pipeline, capacity planning |

## Output example

The generated `gtm-strategy.md` includes sections like:

```markdown
## 1. Revenue Model for $100K ARR

### 1.1 Monthly Target: $8,333 MRR

### 1.2 Revenue Mix
| Source          | % of total | ARR Target | MRR Month 12 |
|-----------------|-----------|------------|--------------|
| Subscriptions   | 70%       | $70,000    | $5,833       |
| Affiliates      | 30%       | $30,000    | $2,500       |

### 1.5 Full Funnel
110,000 installs
  → 30% activation = 33,000 active users
  → 55% M1 retention = 18,150 MAU
  → 8.7% paid conversion = 1,575 subscribers
  → MRR: $8,333+
```

Every section contains specific numbers, calculations, and tables — not generic advice.

## License

MIT
