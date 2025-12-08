# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a **holiday marketing campaign planning repository** for EcoComfort, an e-commerce business selling natural bedding products (bamboo duvets, pillows). The repository contains comprehensive execution plans, operational guides, and tracking templates for a 6-week holiday sales campaign targeting $45,000 in revenue.

**Campaign Timeline:** December 9, 2024 - January 14, 2025
**Target Revenue:** $45,000
**Target Orders:** 157
**Ad Spend Budget:** $10,500

## Repository Structure

```
/Plan/
├── ECOCOMFORT_HOLIDAY_EXECUTION_PLAN.md  # Master campaign execution plan (83KB)
├── DAILY_ACTION_GUIDE.md                 # Day-by-day task checklist
├── FUNNEL_OPTIMIZATION_GUIDE.md          # Conversion funnel analysis and optimization
└── KPI_DASHBOARD_TEMPLATE.md             # Daily/weekly tracking templates
```

## Document Purpose & Usage

### ECOCOMFORT_HOLIDAY_EXECUTION_PLAN.md
The master tactical playbook containing:
- Pre-launch setup (Shopify, Meta Ads, Google Ads, Email)
- Week-by-week strategy breakdown
- Platform-specific setup instructions
- Landing page templates
- Creative briefs and ad copy examples
- Tracking systems and KPI definitions

**Use this for:** Understanding overall campaign strategy, setup instructions, and reference material.

### DAILY_ACTION_GUIDE.md
Time-blocked daily task lists for the entire 6-week campaign, including:
- Hourly schedules for critical launch days
- Daily monitoring routines
- Decision checkpoints with ROAS thresholds
- Emergency troubleshooting procedures
- Week-by-week success metrics

**Use this for:** Day-to-day operations, time management, and quick decision-making.

### FUNNEL_OPTIMIZATION_GUIDE.md
Customer acquisition funnel analysis covering:
- Complete funnel visualization (Ad → Click → ATC → Purchase → Repeat)
- Stage-by-stage conversion benchmarks
- Diagnostic checklists for each funnel stage
- Optimization priority list
- A/B testing roadmap
- Quick win checklists

**Use this for:** Diagnosing conversion issues, improving campaign performance, and optimization decisions.

### KPI_DASHBOARD_TEMPLATE.md
Daily and weekly tracking templates including:
- Daily KPI dashboard (one-page format)
- Financial snapshot calculations
- Platform performance tracking (Meta, Google, Email)
- Health check criteria (Green/Yellow/Red status)
- Weekly scorecard
- 6-week progress tracker

**Use this for:** Creating tracking spreadsheets, monitoring campaign health, and reporting.

## Key Campaign Concepts

### Primary Marketing Channels
1. **Meta Ads** (Facebook/Instagram): $150-200/day budget, cold traffic + retargeting
2. **Google Ads**: Shopping ($60/day) + Search ($40/day) campaigns
3. **Email Marketing**: Klaviyo flows (Welcome, Abandoned Cart) + campaigns

### Core Offers by Phase
- **Week 1-2 (Dec 9-15):** Free $138 pillow set with duvet purchase
- **Week 2 (Dec 16-20):** 30% off everything (final shipping deadline)
- **Week 3 (Dec 21-25):** Pivot to digital gift cards
- **Week 4 (Dec 26-31):** Boxing Day - 40% off
- **Week 5 (Jan 1-7):** New Year resolution angle - 16% off
- **Week 6 (Jan 8-14):** Final flash sale - 30% off

### Critical Success Metrics
- **Minimum ROAS:** 2.0x (break-even)
- **Target ROAS:** 3.0-4.0x (profitable)
- **Target AOV:** $280+
- **Target CAC:** <$100
- **Cart Abandonment:** <70%

### Decision Rules (ROAS-Based)
- **>4.0x:** Scale +30%, launch similar ads
- **3.0-4.0x:** Scale +20%, keep running
- **2.0-3.0x:** Hold steady, optimize
- **1.5-2.0x:** Cut budget 30%, pause worst ads
- **<1.5x:** PAUSE, diagnose, fix

## Common Tasks & Guidance

### When Analyzing Campaign Performance
1. Always start with the KPI Dashboard template structure
2. Calculate blended ROAS: Total Revenue ÷ Total Ad Spend
3. Check profit estimate: (Revenue × 0.75) - Ad Spend - (Revenue × 0.03)
4. Apply decision rules based on ROAS thresholds
5. Identify funnel stage with biggest gap vs. benchmarks

### When Creating/Modifying Plans
- Maintain the time-blocked format from DAILY_ACTION_GUIDE.md
- Include specific metrics targets (not vague goals)
- Add decision checkpoints with clear pass/fail criteria
- Reference the conversion funnel stages (Awareness → Interest → Consideration → Conversion → Loyalty)

### When Troubleshooting Issues
Refer to FUNNEL_OPTIMIZATION_GUIDE.md diagnostic checklists:
- **Low CTR (<1%):** Bad creative → change image/copy
- **Low ATC (<2%):** Bad landing page → simplify, add value clarity
- **High cart abandonment (>80%):** Checkout friction → add free shipping, trust signals
- **No sales after $200 spend:** Check pixel, clicks, ATCs → fix broken funnel stage

### When Creating Ad Copy or Landing Pages
Follow the creative principles from the execution plan:
- Lead with specific pain points ("Stop waking up hot and sweaty")
- Use specific numbers ("$138 free pillow set" not "free gift")
- Include urgency deadlines ("Order by Dec 20")
- Emphasize unique value props: OEKO-TEX certified, Made in Canada, 100-night trial

## Data & Tracking

### Tracking Spreadsheet Structure
The campaign uses a 5-tab Google Sheets structure:
1. **Daily Metrics:** Platform-level performance (Meta, Google, Email, Organic)
2. **Weekly Summary:** Week-over-week progress toward $45K goal
3. **Campaign Performance:** Individual campaign ROAS and keep/kill decisions
4. **Email Performance:** Send metrics and revenue attribution
5. **Product Performance:** SKU-level sales and margin analysis

### Key Calculations
```
ROAS = Revenue ÷ Ad Spend
CAC (Customer Acquisition Cost) = Ad Spend ÷ Orders
AOV (Average Order Value) = Revenue ÷ Orders
Profit Estimate = (Revenue × 0.75) - Ad Spend - (Revenue × 0.03)
                   [75% margin] [Ad cost] [3% transaction fees]
```

## Important Constraints

### Operational Deadlines
- **Dec 20, 11:59 PM:** Last day for Christmas shipping
- **Dec 21:** Pivot from physical products to gift cards
- **Dec 26:** Boxing Day sale launch
- **Jan 14:** Campaign end

### Budget Limits
- **Week 1:** $1,750 spend target
- **Week 2:** $2,450 spend target (peak week)
- **Total campaign:** $10,500 maximum ad spend

### Inventory Considerations
- Product bundles include duvet + free pillows
- Gift wrapping available
- Digital gift cards ($200, $300) for post-Dec 20 sales

## Best Practices for Working with This Repository

1. **Respect the campaign timeline:** All strategies are date-specific and sequential
2. **Maintain the checklist format:** Users rely on actionable, time-specific tasks
3. **Include decision criteria:** Always provide metrics thresholds for pass/fail decisions
4. **Calculate financial impact:** When suggesting changes, show revenue/profit implications
5. **Reference benchmark data:** Use the industry standards from FUNNEL_OPTIMIZATION_GUIDE.md
6. **Keep tracking templates consistent:** Maintain the 5-tab spreadsheet structure
7. **Preserve urgency mechanisms:** Countdown timers and shipping deadlines are critical conversion drivers

## Editing Guidelines

When modifying campaign documents:
- Maintain time-block format (HH:MM AM/PM ranges)
- Include both targets and actual blank fields for tracking
- Use checkbox format `□` or `- [ ]` for actionable items
- Preserve the visual separators and ASCII boxes for clarity
- Keep decision matrices in table format
- Always include "Notes" columns for context capture
